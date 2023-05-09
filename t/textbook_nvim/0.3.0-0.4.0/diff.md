# Comparing `tmp/textbook_nvim-0.3.0.tar.gz` & `tmp/textbook_nvim-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textbook_nvim-0.3.0.tar", last modified: Fri May  5 05:40:06 2023, max compression
+gzip compressed data, was "textbook_nvim-0.4.0.tar", last modified: Tue May  9 22:46:57 2023, max compression
```

## Comparing `textbook_nvim-0.3.0.tar` & `textbook_nvim-0.4.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      122 2023-05-02 15:35:59.171660 textbook_nvim-0.3.0/.gitignore
--rw-r--r--   0        0        0     1086 2023-05-02 15:35:59.171660 textbook_nvim-0.3.0/LICENSE
--rw-r--r--   0        0        0     3734 2023-05-05 05:39:30.885095 textbook_nvim-0.3.0/README.md
--rw-r--r--   0        0        0      517 2023-05-05 05:39:30.885095 textbook_nvim-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6826 2023-05-05 05:38:10.293987 textbook_nvim-0.3.0/rplugin/python3/textbook.py
--rw-r--r--   0        0        0        0 2023-05-02 15:35:59.171660 textbook_nvim-0.3.0/src/textbook_nvim/__init__.py
--rw-r--r--   0        0        0     1247 2023-05-03 19:13:19.864580 textbook_nvim-0.3.0/src/textbook_nvim/cli.py
--rw-r--r--   0        0        0     1714 2023-05-03 19:13:19.867914 textbook_nvim-0.3.0/src/textbook_nvim/parser.py
--rw-r--r--   0        0        0     6966 2023-05-05 05:39:30.885095 textbook_nvim-0.3.0/src/textbook_nvim/render.py
--rw-r--r--   0        0        0      327 1970-01-01 00:00:00.000000 textbook_nvim-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      122 2023-05-02 15:35:59.171660 textbook_nvim-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1086 2023-05-02 15:35:59.171660 textbook_nvim-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3734 2023-05-05 05:44:28.162521 textbook_nvim-0.4.0/README.md
+-rw-r--r--   0        0        0      538 2023-05-09 21:03:37.158779 textbook_nvim-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7011 2023-05-09 22:46:46.999279 textbook_nvim-0.4.0/rplugin/python3/textbook.py
+-rw-r--r--   0        0        0        0 2023-05-02 15:35:59.171660 textbook_nvim-0.4.0/src/textbook_nvim/__init__.py
+-rw-r--r--   0        0        0     1222 2023-05-09 21:04:06.559013 textbook_nvim-0.4.0/src/textbook_nvim/cli.py
+-rw-r--r--   0        0        0     1717 2023-05-09 21:04:13.735737 textbook_nvim-0.4.0/src/textbook_nvim/parser.py
+-rw-r--r--   0        0        0     6796 2023-05-09 21:04:17.389099 textbook_nvim-0.4.0/src/textbook_nvim/render.py
+-rw-r--r--   0        0        0      389 1970-01-01 00:00:00.000000 textbook_nvim-0.4.0/PKG-INFO
```

### Comparing `textbook_nvim-0.3.0/LICENSE` & `textbook_nvim-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `textbook_nvim-0.3.0/README.md` & `textbook_nvim-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `textbook_nvim-0.3.0/rplugin/python3/textbook.py` & `textbook_nvim-0.4.0/rplugin/python3/textbook.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,31 @@
 from pynvim.api import Nvim, Buffer
 from textbook_nvim.parser import Parser
 from textbook_nvim.render import Renderer
 from pathlib import Path
 
 Args = List[str]
 
+
 class TextBookConfig(BaseModel):
-    tmp_path : str 
-    cell_indicator : str
-    cell_pattern : str
-    cell_separator : str
+    tmp_path: str
+    cell_indicator: str
+    cell_pattern: str
+    cell_separator: str
     cell_text: str
     cell_color: str
     theme: str
-    comment_pattern : str
+    comment_pattern: str
+
 
 @plugin
 class TextBook:
-    buffer : Buffer
-    tb_buffer : Buffer
-    tmp_path : Path
+    buffer: Buffer
+    tb_buffer: Buffer
+    tmp_path: Path
     active_cell: int = 0
     ns_id: int
     parsed_path: Path
     rendered_path: Path
     extmark_id: Any = None
     config: TextBookConfig
 
@@ -35,102 +37,109 @@
         self.nvim = nvim
         self.parser = Parser()
         self.renderer = Renderer()
         self.load_config()
 
     def load_config(self):
         self.config = TextBookConfig(
-                tmp_path=self.nvim.vars.get("TextBookTmpPath") or "/tmp",
-                cell_indicator=self.nvim.vars.get("TextBookCellIndicator") or "◆",
-                cell_pattern=self.nvim.vars.get("TextBookCellPattern") or r"^# \%\% \[(?P<cell_type>\w+)\]",
-                cell_separator=self.nvim.vars.get("TextBookCellSeparator") or r"# %% [{}]",
-                cell_text=self.nvim.vars.get("TextBookCellText") or " Cell: {}",
-                cell_color=self.nvim.vars.get("TextBookCellColor") or r"\#5180e6",
-                theme=self.nvim.vars.get("TextBookTheme") or "gruvbox-dark",
-                comment_pattern=self.nvim.vars.get("TextBookCommentPattern") or r"^\#"
-                )
+            tmp_path=self.nvim.vars.get("TextBookTmpPath") or "/tmp",
+            cell_indicator=self.nvim.vars.get("TextBookCellIndicator") or "◆",
+            cell_pattern=(
+                self.nvim.vars.get("TextBookCellPattern") or
+                r"^# \%\% \[(?P<cell_type>\w+)\]"
+                ),
+            cell_separator=self.nvim.vars.get("TextBookCellSeparator") or r"# %% [{}]",
+            cell_text=self.nvim.vars.get("TextBookCellText") or " Cell: {}",
+            cell_color=self.nvim.vars.get("TextBookCellColor") or r"\#5180e6",
+            theme=self.nvim.vars.get("TextBookTheme") or "gruvbox-dark",
+            comment_pattern=self.nvim.vars.get("TextBookCommentPattern") or r"^\#",
+        )
 
     @command("TextBookConfig", nargs=0, range="")
     def textbook_config(self, args: Args, range=None):
         self.load_config()
 
     @command("TextBookBuffer", nargs=0, range="")
     def textbook_buffer(self, args: Args, range=None):
         self.buffer = self.nvim.current.buffer
 
     def parse(self, parsed_path: Optional[Path] = None):
-        (
-                self.parser.set_text(
-                    text = [str(i) for i in self.buffer]
-                    )
-                .set_pattern()
-                .parse()
-                )
+        (self.parser.set_text(text=[str(i) for i in self.buffer]).set_pattern().parse())
         if parsed_path is not None:
             self.parser.save(parsed_path)
 
     @command("TextBookOpen", nargs=0, range="")
-    def textbook_render(self, args: Args, range=None):
-        idx = str(uuid4()) 
+    def textbook_open(self, args: Args, range=None):
+        idx = str(uuid4())
         self.parsed_path = Path(self.config.tmp_path) / (idx + "_parsed")
         self.rendered_path = Path(self.config.tmp_path) / (idx + "_rendered")
         self.parse(self.parsed_path)
 
         row = self.nvim.current.window.cursor[0] - 1
         for i, cell in enumerate(self.parser.parsed_text.values):
             if row >= cell.cell_range[0] and row < cell.cell_range[1]:
                 self.active_cell = i
 
         lexer = self.nvim.call("nvim_buf_get_option", self.buffer.number, "filetype")
         self.tb_buffer = self.nvim.api.create_buf(False, True)
         self.nvim.api.set_current_buf(self.tb_buffer)
         self.nvim.command(
-                f"ter tbcli --parsed_path '{str(self.parsed_path)}' " +
-                f"--rendered_path '{str(self.rendered_path)}' " +
-                f"--lexer '{lexer}' --theme '{self.config.theme}' " +
-                f"--comment_pattern '{self.config.comment_pattern}' " +
-                f"--cell_text '{self.config.cell_text}' " +
-                f"--cell_color '{self.config.cell_color}'"
-                )
+            f"ter tbcli --parsed_path '{str(self.parsed_path)}' "
+            + f"--rendered_path '{str(self.rendered_path)}' "
+            + f"--lexer '{lexer}' --theme '{self.config.theme}' "
+            + f"--comment_pattern '{self.config.comment_pattern}' "
+            + f"--cell_text '{self.config.cell_text}' "
+            + f"--cell_color '{self.config.cell_color}'"
+        )
         self.ns_id = self.nvim.api.create_namespace("cell_indicator")
 
-    @command("TextBookSync", nargs="*", range="") #type: ignore
+    @command("TextBookSync", nargs="*", range="")  # type: ignore
     def textbook_sync(self, args: Args, range=None):
         self.select_cell()
 
     def select_cell(self):
         self.renderer.load(self.rendered_path)
         line = self.renderer.rendered_text.values[self.active_cell].cell_range[0]
-        
+
         if self.extmark_id is not None:
-            self.nvim.call("nvim_buf_del_extmark", self.tb_buffer.number, self.ns_id, self.extmark_id)
-        self.extmark_id = self.nvim.call(
-                "nvim_buf_set_extmark",
+            self.nvim.call(
+                "nvim_buf_del_extmark",
                 self.tb_buffer.number,
-                self.ns_id, line - 1, 0,
-                {"virt_text": [[self.config.cell_indicator]], "virt_text_pos": "overlay"}
-                )
+                self.ns_id,
+                self.extmark_id,
+            )
+        self.extmark_id = self.nvim.call(
+            "nvim_buf_set_extmark",
+            self.tb_buffer.number,
+            self.ns_id,
+            line - 1,
+            0,
+            {"virt_text": [[self.config.cell_indicator]], "virt_text_pos": "overlay"},
+        )
         self.nvim.current.window.cursor = (line, 1)
 
-    @command("TextBookSelectCell", nargs="*", range="") #type: ignore
+    @command("TextBookSelectCell", nargs="*", range="")  # type: ignore
     def textbook_select_cell(self, args: Args, range=None):
         self.renderer.load(self.rendered_path)
 
         if not args:
             row = self.nvim.current.window.cursor[0]
             for i, cell in enumerate(self.renderer.rendered_text.values):
                 if row >= cell.cell_range[0] and row < cell.cell_range[1]:
                     self.active_cell = i
         else:
             self.active_cell = int(args[0]) - 1
         self.select_cell()
 
-    @command("TextBookAddCell", nargs="*", range="")
+    @command("TextBookAddCell", nargs="*", range="") #type: ignore
     def textbook_add_cell(self, args: Args, range=None):
-        if hasattr(self, "tb_buffer") and self.nvim.current.buffer.number == self.tb_buffer.number:
+        if (
+            hasattr(self, "tb_buffer")
+            and self.nvim.current.buffer.number == self.tb_buffer.number
+        ):
             self.select_cell()
             self.close()
         if not hasattr(self, "buffer"):
             self.buffer = self.nvim.current.buffer
         self.parse()
 
         after = int(args[1])
@@ -166,7 +175,12 @@
         line = self.parser.parsed_text.values[self.active_cell].cell_range[0]
         self.nvim.current.window.cursor = (line + 1, 0)
         self.nvim.api.buf_delete(self.tb_buffer.handle, {"force": True, "unload": True})
 
     @command("TextBookClose", nargs=0, range="")
     def textbook_close(self, args: Args, range=None):
         self.close()
+
+    @command("TextBookRender", nargs=0, range="")
+    def textbook_render(self, args: Args, range=None):
+        filename = self.buffer.name
+        self.nvim.api.command(f"!jupytext -s {filename}")
```

### Comparing `textbook_nvim-0.3.0/src/textbook_nvim/cli.py` & `textbook_nvim-0.4.0/src/textbook_nvim/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 import re
 from click import command, option
 from textbook_nvim.render import Renderer
 from textbook_nvim.parser import ParsedText
 from pathlib import Path
 
+
 @command
 @option("--parsed_path", type=Path, help="Json file with the parsed text.")
 @option("--rendered_path", type=Path, help="Json file to store the rendered text.")
 @option("--lexer", type=str, help="Lexer for the programming language.")
 @option("--theme", type=str, help="Theme for color highlighting.")
 @option("--comment_pattern", type=str, help="Regex to identify comments.")
 @option("--cell_text", type=str, help="Text to show as cell separator.")
 @option("--cell_color", type=str, help="Color to display the cell separator.")
 def main(
-        parsed_path: Path,
-        rendered_path: Path,
-        lexer: str, theme: str,
-        comment_pattern: str, cell_text: str,
-        cell_color: str
-        ) -> int:
+    parsed_path: Path,
+    rendered_path: Path,
+    lexer: str,
+    theme: str,
+    comment_pattern: str,
+    cell_text: str,
+    cell_color: str,
+) -> int:
     parsed_text = ParsedText.parse_file(parsed_path)
     (
         Renderer()
         .setup(
             parsed_text,
             lexer=lexer,
             pattern=re.compile(comment_pattern),
             theme=theme,
             cell_text=cell_text,
-            cell_color=cell_color
-            )
+            cell_color=cell_color,
+        )
         .render()
         .save(rendered_path)
-        )
+    )
     return 0
```

### Comparing `textbook_nvim-0.3.0/src/textbook_nvim/parser.py` & `textbook_nvim-0.4.0/src/textbook_nvim/parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 import re
 from typing import List, Tuple
 from pydantic import BaseModel
 from pathlib import Path
 
 Text = List[str]
 
+
 class ParsedCell(BaseModel):
     text: str
     cell_type: str
     cell_range: Tuple[int, int]
 
+
 class ParsedText(BaseModel):
-    values : List[ParsedCell]
+    values: List[ParsedCell]
+
 
 class Parser:
-    text : Text
-    parsed_text : ParsedText
-    pattern : re.Pattern
+    text: Text
+    parsed_text: ParsedText
+    pattern: re.Pattern
 
     def set_text(self, text: Text) -> "Parser":
         self.text = text
         return self
 
-    def set_pattern(self, pattern: re.Pattern = re.compile(r"^# \%\% \[(?P<cell_type>\w+)\]")) -> "Parser":
+    def set_pattern(
+        self, pattern: re.Pattern = re.compile(r"^# \%\% \[(?P<cell_type>\w+)\]")
+    ) -> "Parser":
         self.pattern = pattern
         return self
 
     def parse(self) -> "Parser":
         separator_positions = []
         cell_types = []
         for i, line in enumerate(self.text):
@@ -34,22 +39,24 @@
             if match is not None:
                 separator_positions.append(i)
                 cell_types.append(match.group("cell_type"))
         if separator_positions[-1] != len(self.text):
             separator_positions.append(len(self.text))
 
         self.parsed_text = ParsedText(values=[])
-        for initial_pos, end_pos, cell_type in zip(separator_positions, separator_positions[1:], cell_types):
+        for initial_pos, end_pos, cell_type in zip(
+            separator_positions, separator_positions[1:], cell_types
+        ):
             self.parsed_text.values.append(
-                    ParsedCell(
-                        text="\n".join(self.text[initial_pos: end_pos]),
-                        cell_type=cell_type,
-                        cell_range=(initial_pos, end_pos)
-                        )
-                    )
+                ParsedCell(
+                    text="\n".join(self.text[initial_pos:end_pos]),
+                    cell_type=cell_type,
+                    cell_range=(initial_pos, end_pos),
+                )
+            )
         return self
 
     def get_parsed_text(self) -> ParsedText:
         return self.parsed_text
 
     def save(self, path: Path):
         with open(path, "w") as f:
```

### Comparing `textbook_nvim-0.3.0/src/textbook_nvim/render.py` & `textbook_nvim-0.4.0/src/textbook_nvim/render.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,42 +8,55 @@
 from rich.syntax import Syntax
 from rich.markdown import Markdown
 from rich.panel import Panel
 from rich.table import Table
 from rich.text import Text
 from pathlib import Path
 
+
 class RenderedCell(BaseModel):
     text: str
     cell_range: Tuple[int, int]
 
+
 class RenderedText(BaseModel):
     values: List[RenderedCell]
 
+
 class AbstractRender(ABC):
-    def __init__(self, lexer: str, comment_pattern: re.Pattern, cell_id:int, theme: str, cell_text: str, cell_color: str):
+    def __init__(
+        self,
+        lexer: str,
+        comment_pattern: re.Pattern,
+        cell_id: int,
+        theme: str,
+        cell_text: str,
+        cell_color: str,
+    ):
         self.lexer = lexer
         self.comment_pattern = comment_pattern
         self.cell_id = cell_id
         self.theme = theme
         self.cell_text = cell_text
         self.cell_color = cell_color
 
-    def setup(self, parsed_cell: ParsedCell, console: Console, init_pos: int) -> "AbstractRender":
+    def setup(
+        self, parsed_cell: ParsedCell, console: Console, init_pos: int
+    ) -> "AbstractRender":
         self.parsed_cell = parsed_cell
         self.console = console
         self.init_pos = init_pos
         return self
 
     @abstractmethod
     def render(self) -> RenderedCell:
         ...
 
-class CodeRender(AbstractRender):
 
+class CodeRender(AbstractRender):
     def render(self) -> RenderedCell:
         lines = self.parsed_cell.text.split("\n")[1:]
         clean_text = "\n".join(lines)
         syntax = Syntax(clean_text, self.lexer)
         text = Text(self.cell_text.format(self.cell_id))
         text.stylize(self.cell_color)
         with self.console.capture() as capture:
@@ -51,27 +64,30 @@
             self.console.print(syntax)
             self.console.print(" ")
         result = capture.get()
         self.console.print(text)
         self.console.print(syntax)
         self.console.print(" ")
         return RenderedCell(
-                text=result,
-                cell_range=(self.init_pos, self.init_pos + len(result.split("\n")) - 2)
-                )
+            text=result,
+            cell_range=(self.init_pos, self.init_pos + len(result.split("\n")) - 2),
+        )
+
 
 class MarkdownEnum(Enum):
     TEXT = "TEXT"
     TABLE = "TABLE"
 
+
 class MarkdownRow(BaseModel):
     text: str
     idx: int
     md_type: MarkdownEnum
 
+
 class MarkdownRender(AbstractRender):
     table_pattern = re.compile(r"\|.+\|")
     sep_validator = re.compile(r"[\-\s]+")
 
     def render_table(self, group: List[MarkdownRow]) -> Union[Markdown, Table]:
         if re.search(self.sep_validator, "".join(group[1].text.split("|"))) is None:
             return Markdown("\n".join(line.text for line in group))
@@ -82,26 +98,21 @@
         for row in group[2:]:
             cells = row.text.strip().split("|")
             if len(cells) != n_cols:
                 return Markdown("\n".join(line.text for line in group))
             table.add_row(*cells)
         return table
 
-    def generate_components(self, groups: List[List[MarkdownRow]]) -> List[Union[Markdown, Table]]:
+    def generate_components(
+        self, groups: List[List[MarkdownRow]]
+    ) -> List[Union[Markdown, Table]]:
         components = []
         for group in groups:
-            if (
-                    group[0].md_type == MarkdownEnum.TEXT or
-                    len(group) < 3
-                    ):
-                components.append(
-                        Markdown(
-                            "\n".join(line.text for line in group)
-                            )
-                        )
+            if group[0].md_type == MarkdownEnum.TEXT or len(group) < 3:
+                components.append(Markdown("\n".join(line.text for line in group)))
             else:
                 components.append(self.render_table(group))
         return components
 
     def render_lines(self, lines: List[str]) -> Group:
         if len(lines) < 2:
             return Group(Markdown("\n".join(lines)))
@@ -116,83 +127,86 @@
         groups = [[parsed_lines[0]]]
         for i in range(1, len(parsed_lines)):
             if parsed_lines[i].md_type == parsed_lines[i - 1].md_type:
                 groups[-1].append(parsed_lines[i])
             else:
                 groups.append([parsed_lines[i]])
 
-        
         components = self.generate_components(groups)
         return Group(*components)
 
     def render(self) -> RenderedCell:
         lines = self.parsed_cell.text.split("\n")[1:]
-        *clean_lines, = map(lambda line: re.sub(self.comment_pattern, "", line), lines)
+        (*clean_lines,) = map(
+            lambda line: re.sub(self.comment_pattern, "", line), lines
+        )
         md = Panel(self.render_lines(clean_lines), title="markdown")
         text = Text(self.cell_text.format(self.cell_id))
         text.stylize(self.cell_color)
         with self.console.capture() as capture:
             self.console.print(text)
             self.console.print(md)
         rendered_lines = capture.get().split("\n")
         self.console.print(text)
         self.console.print(md)
         return RenderedCell(
-                text="\n".join(rendered_lines),
-                cell_range=(self.init_pos, self.init_pos + len(rendered_lines) - 2)
-                )
+            text="\n".join(rendered_lines),
+            cell_range=(self.init_pos, self.init_pos + len(rendered_lines) - 2),
+        )
+
 
 class Renderer:
-    parsed_text : ParsedText
-    rendered_text : RenderedText
+    parsed_text: ParsedText
+    rendered_text: RenderedText
     lexer: str
     pattern: re.Pattern
     theme: str
     cell_text: str
     cell_color: str
     renders: Dict[str, Type[AbstractRender]] = {
-            "raw": CodeRender,
-            "markdown": MarkdownRender
-            }
+        "code": CodeRender,
+        "markdown": MarkdownRender,
+    }
 
     def __init__(self, console_kwargs: Dict = {}):
         self.console = Console(**console_kwargs)
 
     def setup(
-            self,
-            parsed_text: ParsedText,
-            lexer: str,
-            pattern: re.Pattern,
-            theme: str,
-            cell_text: str,
-            cell_color: str
-            ) -> "Renderer":
+        self,
+        parsed_text: ParsedText,
+        lexer: str,
+        pattern: re.Pattern,
+        theme: str,
+        cell_text: str,
+        cell_color: str,
+    ) -> "Renderer":
         self.parsed_text = parsed_text
         self.lexer = lexer
         self.pattern = pattern
         self.theme = theme
         self.cell_text = cell_text
         self.cell_color = cell_color
         return self
-    
+
     def render(self) -> "Renderer":
         self.rendered_text = RenderedText(values=[])
         init_pos = 1
         for i, cell in enumerate(self.parsed_text.values):
             self.rendered_text.values.append(
-                    self.renders[cell.cell_type](
-                        lexer=self.lexer, cell_id=i + 1,
-                        comment_pattern=self.pattern,
-                        cell_text=self.cell_text,
-                        cell_color=self.cell_color,
-                        theme=self.theme
-                        )
-                    .setup(cell, self.console, init_pos)
-                    .render()
-                    )
+                self.renders[cell.cell_type](
+                    lexer=self.lexer,
+                    cell_id=i + 1,
+                    comment_pattern=self.pattern,
+                    cell_text=self.cell_text,
+                    cell_color=self.cell_color,
+                    theme=self.theme,
+                )
+                .setup(cell, self.console, init_pos)
+                .render()
+            )
             init_pos = self.rendered_text.values[-1].cell_range[1] + 1
         return self
 
     def get_rendered_text(self) -> RenderedText:
         return self.rendered_text
 
     def save(self, path: Path) -> None:
```

