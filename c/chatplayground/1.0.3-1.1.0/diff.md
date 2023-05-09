# Comparing `tmp/chatplayground-1.0.3.tar.gz` & `tmp/chatplayground-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatplayground-1.0.3.tar", max compression
+gzip compressed data, was "chatplayground-1.1.0.tar", max compression
```

## Comparing `chatplayground-1.0.3.tar` & `chatplayground-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    34523 2023-05-08 19:57:46.181090 chatplayground-1.0.3/LICENSE
--rw-r--r--   0        0        0     4471 2023-05-08 19:57:46.185090 chatplayground-1.0.3/README.md
--rw-r--r--   0        0        0       17 2023-05-08 19:57:46.185090 chatplayground-1.0.3/chatplayground/.gitignore
--rw-r--r--   0        0        0       22 2023-05-08 19:57:46.185090 chatplayground-1.0.3/chatplayground/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 19:57:46.185090 chatplayground-1.0.3/chatplayground/app/__init__.py
--rw-r--r--   0        0        0   104390 2023-05-08 19:57:46.185090 chatplayground-1.0.3/chatplayground/app/app.py
--rw-r--r--   0        0        0    15406 2023-05-08 19:57:46.185090 chatplayground-1.0.3/chatplayground/assets/favicon.ico
--rw-r--r--   0        0        0     1281 2023-05-08 19:57:46.185090 chatplayground-1.0.3/chatplayground/assets/react-json-view-lite.css
--rw-r--r--   0        0        0   178190 2023-05-08 19:57:46.185090 chatplayground-1.0.3/chatplayground/message_threads/faust_in_oxford_1683330128.209918.json
--rw-r--r--   0        0        0      846 2023-05-08 19:57:46.185090 chatplayground-1.0.3/chatplayground/pcconfig.py
--rw-r--r--   0        0        0     3081 2023-05-08 19:57:46.205090 chatplayground-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     6838 1970-01-01 00:00:00.000000 chatplayground-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-09 22:48:34.566951 chatplayground-1.1.0/LICENSE
+-rw-r--r--   0        0        0     4471 2023-05-09 22:48:34.566951 chatplayground-1.1.0/README.md
+-rw-r--r--   0        0        0       17 2023-05-09 22:48:34.566951 chatplayground-1.1.0/chatplayground/.gitignore
+-rw-r--r--   0        0        0       22 2023-05-09 22:48:34.566951 chatplayground-1.1.0/chatplayground/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 22:48:34.566951 chatplayground-1.1.0/chatplayground/app/__init__.py
+-rw-r--r--   0        0        0   108083 2023-05-09 22:48:34.566951 chatplayground-1.1.0/chatplayground/app/app.py
+-rw-r--r--   0        0        0    15406 2023-05-09 22:48:34.566951 chatplayground-1.1.0/chatplayground/assets/favicon.ico
+-rw-r--r--   0        0        0     1281 2023-05-09 22:48:34.566951 chatplayground-1.1.0/chatplayground/assets/react-json-view-lite.css
+-rw-r--r--   0        0        0   178190 2023-05-09 22:48:34.570951 chatplayground-1.1.0/chatplayground/message_threads/faust_in_oxford_1683330128.209918.json
+-rw-r--r--   0        0        0      846 2023-05-09 22:48:34.570951 chatplayground-1.1.0/chatplayground/pcconfig.py
+-rw-r--r--   0        0        0     3081 2023-05-09 22:48:34.594951 chatplayground-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6838 1970-01-01 00:00:00.000000 chatplayground-1.1.0/PKG-INFO
```

### Comparing `chatplayground-1.0.3/LICENSE` & `chatplayground-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chatplayground-1.0.3/README.md` & `chatplayground-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `chatplayground-1.0.3/chatplayground/app/app.py` & `chatplayground-1.1.0/chatplayground/app/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -277,14 +277,18 @@
 
     auto_focus: Var[typing.Union[str, int, bool]]
 
 
 auto_focus_text_area = AutoFocusTextArea.create
 
 
+def render_tooltip(*args, **kwargs):
+    return pc.tooltip(*args, **kwargs, open_delay=500)
+
+
 class UID:
     """A unique ID generator that uses the current time and a counter to generate unique IDs.
 
     TODO: this is not thread safe, but that should not be a problem for now.
     TODO: ideally we should use a monotonous timer (and encode the timezone as well?)
     """
 
@@ -742,29 +746,35 @@
                 stored_message = message_uid_map.setdefault(message.uid, message)
                 assert stored_message == message
         return message_uid_map
 
 
 def render_edit_thread_button(message: StyledMessage):
     """Render the edit thread button."""
-    return pc.button(
-        pc.icon(tag="edit"),
-        size='xs',
-        variant='ghost',
-        on_click=lambda: EditableMessageState.enter_editing(message.uid),  # type: ignore
+    return render_tooltip(
+        pc.button(
+            pc.icon(tag="edit"),
+            size='xs',
+            variant='ghost',
+            on_click=lambda: EditableMessageState.enter_editing(message.uid),  # type: ignore
+        ),
+        label="Edit thread: create a new thread while preserving consecutive messages",
     )
 
 
 def render_fork_thread_button(message: StyledMessage):
     """Render the fork thread button."""
-    return pc.button(
-        pc.icon(tag="repeat_clock"),
-        size='xs',
-        variant='ghost',
-        on_click=lambda: EditableMessageState.enter_forking(message.uid),  # type: ignore
+    return render_tooltip(
+        pc.button(
+            pc.icon(tag="repeat_clock"),
+            size='xs',
+            variant='ghost',
+            on_click=lambda: EditableMessageState.enter_forking(message.uid),  # type: ignore
+        ),
+        label="Fork thread: creates a new thread while discarding consecutive messages",
     )
 
 
 @typing.no_type_check
 def render_message_toolbar(message: StyledMessage):
     """Render the message toolbar.
 
@@ -773,58 +783,73 @@
     num_threads = 1 + message.next_linked_messages.length() + message.prev_linked_messages.length()
     thread_index = 1 + message.prev_linked_messages.length()
     is_not_bot = message.role != "Bot"
     return pc.fragment(
         pc.cond(
             message.uid == EditableMessageState.editable_message_uid,
             pc.hstack(
-                pc.button(
-                    pc.icon(tag="check"), size='xs', variant='ghost', on_click=EditableMessageState.submit_editing
+                render_tooltip(
+                    pc.button(
+                        pc.icon(tag="check"), size='xs', variant='ghost', on_click=EditableMessageState.submit_editing
+                    ),
+                    label="Submit edit",
                 ),
                 pc.divider(orientation="vertical", height="1em"),
-                pc.button(
-                    pc.icon(tag="close"), size='xs', variant='ghost', on_click=EditableMessageState.cancel_editing
+                render_tooltip(
+                    pc.button(
+                        pc.icon(tag="close"), size='xs', variant='ghost', on_click=EditableMessageState.cancel_editing
+                    ),
+                    label="Cancel edit",
                 ),
                 pc.divider(orientation="vertical", height="1em"),
             ),
             pc.fragment(
                 render_message_menu(message),
                 pc.cond(is_not_bot, render_fork_thread_button(message), render_edit_thread_button(message)),
             ),
         ),
         pc.fragment(
-            pc.button(
-                pc.icon(tag="chevron_left"),
-                size='xs',
-                variant='ghost',
-                is_disabled=EditableMessageState.is_editing | (message.prev_linked_messages.length() == 0),
-                on_click=lambda: NavigationState.go_to_message_thread(
-                    message.prev_linked_messages[-1].thread_uid,
-                    message.prev_linked_messages[-1].uid,
+            render_tooltip(
+                pc.button(
+                    pc.icon(tag="chevron_left"),
+                    size='xs',
+                    variant='ghost',
+                    is_disabled=EditableMessageState.is_editing | (message.prev_linked_messages.length() == 0),
+                    on_click=lambda: NavigationState.go_to_message_thread(
+                        message.prev_linked_messages[-1].thread_uid,
+                        message.prev_linked_messages[-1].uid,
+                    ),
                 ),
+                label="Previous alternative message",
             ),
-            pc.button(
-                react_icon(as_="ImTree"),
-                size='xs',
-                variant='ghost',
-                is_disabled=(
-                    EditableMessageState.is_editing
-                    | ((message.next_linked_messages.length() + message.prev_linked_messages.length()) == 0)
+            render_tooltip(
+                pc.button(
+                    react_icon(as_="ImTree"),
+                    size='xs',
+                    variant='ghost',
+                    is_disabled=(
+                        EditableMessageState.is_editing
+                        | ((message.next_linked_messages.length() + message.prev_linked_messages.length()) == 0)
+                    ),
+                    on_click=MessageOverviewState.show_alternatives(message.uid),
                 ),
-                on_click=MessageOverviewState.show_alternatives(message.uid),
+                label="Show alternative messages in a carousel",
             ),
-            pc.button(
-                pc.icon(tag="chevron_right"),
-                size='xs',
-                variant='ghost',
-                is_disabled=EditableMessageState.is_editing | (message.next_linked_messages.length() == 0),
-                on_click=lambda: NavigationState.go_to_message_thread(
-                    message.next_linked_messages[0].thread_uid,
-                    message.next_linked_messages[0].uid,
+            render_tooltip(
+                pc.button(
+                    pc.icon(tag="chevron_right"),
+                    size='xs',
+                    variant='ghost',
+                    is_disabled=EditableMessageState.is_editing | (message.next_linked_messages.length() == 0),
+                    on_click=lambda: NavigationState.go_to_message_thread(
+                        message.next_linked_messages[0].thread_uid,
+                        message.next_linked_messages[0].uid,
+                    ),
                 ),
+                label="Next alternative message",
             ),
         ),
         pc.cond(
             num_threads > 1,
             pc.fragment(
                 pc.text(thread_index),
                 pc.text("/", color=SolarizedColors.base0),
@@ -833,78 +858,81 @@
         ),
     )
 
 
 def render_carousel_message(message: StyledMessage):
     """Render a message in the carousel of alternative messages."""
     return pc.grid_item(
-        pc.button(
-            pc.vstack(
-                pc.box(
-                    pc.flex(
-                        pc.text(message.fmt_header),
-                        pc.spacer(),
-                        pc.text(message.fmt_creation_datetime),
+        render_tooltip(
+            pc.button(
+                pc.vstack(
+                    pc.box(
+                        pc.flex(
+                            pc.text(message.fmt_header),
+                            pc.spacer(),
+                            pc.text(message.fmt_creation_datetime),
+                            width="100%",
+                        ),
+                        background_color=message.background_color,
+                        color=message.foreground_color,
+                        border_radius="15px 15px 0 0",
                         width="100%",
+                        padding="0.25em 0.25em 0 0.5em",
+                        margin_bottom="0",
                     ),
-                    background_color=message.background_color,
-                    color=message.foreground_color,
-                    border_radius="15px 15px 0 0",
-                    width="100%",
-                    padding="0.25em 0.25em 0 0.5em",
-                    margin_bottom="0",
-                ),
-                pc.cond(
-                    message.error,
-                    pc.fragment(
+                    pc.cond(
+                        message.error,
+                        pc.fragment(
+                            pc.cond(
+                                message.content,
+                                pc.box(
+                                    render_markdown(message.content),
+                                    border_radius="0 0 0 0",
+                                    color=message.foreground_color,
+                                    border_width="medium",
+                                    border_color=message.foreground_color,
+                                    width="100%",
+                                    padding="0 0.25em 0 0.25em",
+                                ),
+                            ),
+                            pc.box(
+                                render_markdown(message.error),
+                                border_radius="0 0 15px 15px",
+                                color=message.foreground_color,
+                                background_color=SolarizedColors.red,
+                                width="100%",
+                                padding="0 0.25em 0 0.25em",
+                            ),
+                        ),
                         pc.cond(
                             message.content,
                             pc.box(
                                 render_markdown(message.content),
-                                border_radius="0 0 0 0",
+                                border_radius="0 0 15px 15px",
                                 color=message.foreground_color,
                                 border_width="medium",
                                 border_color=message.foreground_color,
                                 width="100%",
                                 padding="0 0.25em 0 0.25em",
                             ),
                         ),
-                        pc.box(
-                            render_markdown(message.error),
-                            border_radius="0 0 15px 15px",
-                            color=message.foreground_color,
-                            background_color=SolarizedColors.red,
-                            width="100%",
-                            padding="0 0.25em 0 0.25em",
-                        ),
-                    ),
-                    pc.cond(
-                        message.content,
-                        pc.box(
-                            render_markdown(message.content),
-                            border_radius="0 0 15px 15px",
-                            color=message.foreground_color,
-                            border_width="medium",
-                            border_color=message.foreground_color,
-                            width="100%",
-                            padding="0 0.25em 0 0.25em",
-                        ),
                     ),
+                    width="30ch",
+                    max_width="30ch",
+                    padding_top="0.5em",
+                    padding_bottom="0.5em",
+                    spacing="0em",
                 ),
                 width="30ch",
-                max_width="30ch",
-                padding_top="0.5em",
-                padding_bottom="0.5em",
-                spacing="0em",
+                max_width="32ch",
+                height="100%",
+                on_click=lambda: MessageOverviewState.hide_alternatives(message.uid),  # type: ignore
+                variant="solid",
             ),
-            width="30ch",
-            max_width="32ch",
-            height="100%",
-            on_click=lambda: MessageOverviewState.hide_alternatives(message.uid),  # type: ignore
-            variant="solid",
+            label="Select this alternative message",
         ),
         row_start=1,
     )
 
 
 def render_markdown(content: str | None, **props):
     """Render a markdown string using sensible defaults for the styles."""
@@ -1030,36 +1058,42 @@
     return pc.foreach(message_row, render_grid_cell)
 
 
 def render_grid_column_button(thread_uid: str, index):
     """Render a button to remove a thread from the grid and a big button that covers the whole column to 'zoom in'."""
     return pc.fragment(
         pc.grid_item(
-            pc.button(pc.icon(tag="delete"), variant="outline", margin="1em"),
+            render_tooltip(
+                pc.button(pc.icon(tag="delete"), variant="outline", margin="1em"),
+                label="Remove this thread from the grid",
+            ),
             row_start=1,
             row_span=1,
             col_start=index.to(int) + 1,
             col_span=1,
             on_click=lambda: MessageGridState.remove_thread(thread_uid),  # type: ignore
         ),
         pc.grid_item(
-            pc.button(
-                width="100%",
-                height="100%",
-                on_click=lambda: MessageGridState.go_to_thread(thread_uid),  # type: ignore
-                variant="ghost",
-                opacity=0.5,
-                minWidth="30ch",
-                min_height="30ch",
+            render_tooltip(
+                pc.button(
+                    width="100%",
+                    height="100%",
+                    on_click=lambda: MessageGridState.go_to_thread(thread_uid),  # type: ignore
+                    variant="ghost",
+                    opacity=0.5,
+                    minWidth="30ch",
+                    min_height="30ch",
+                ),
+                row_start=2,
+                row_span=MessageGridState.styled_grid_cells.length(),
+                col_start=index.to(int) + 1,
+                col_span=1,
+                style={"z-index": 1},
+                label="Zoom in on this thread",
             ),
-            row_start=2,
-            row_span=MessageGridState.styled_grid_cells.length(),
-            col_start=index.to(int) + 1,
-            col_span=1,
-            style={"z-index": 1},
         ),
     )
 
 
 def render_message_grid():
     """Render the expose-style grid."""
     return pc.flex(
@@ -1087,18 +1121,19 @@
     return pc.hstack(
         pc.vstack(
             pc.box(
                 pc.flex(
                     render_message_toolbar(message),
                     pc.spacer(),
                     pc.text(message.fmt_header),
-                    pc.cond(
-                        message.role == "System",
-                        pc.button(pc.icon(tag="info"), size="xs", variant="outline"),
-                    ),
+                    # TODO: Make this collapse and show the system prompt.
+                    # pc.cond(
+                    #     message.role == "System",
+                    #     pc.button(pc.icon(tag="info"), size="xs", variant="outline"),
+                    # ),
                     pc.spacer(),
                     pc.text(message.fmt_creation_datetime),
                     width="100%",
                 ),
                 background_color=message.background_color,
                 color=message.foreground_color,
                 border_radius="15px 0 0 0",
@@ -1266,19 +1301,22 @@
     """Render the error message of an editable message."""
     return pc.box(
         pc.flex(
             pc.box(
                 render_markdown(message.error),
             ),
             pc.spacer(),
-            pc.button(
-                pc.icon(tag="delete"),
-                size='xs',
-                variant='ghost',
-                on_click=EditableMessageState.clear_editable_message_error,
+            render_tooltip(
+                pc.button(
+                    pc.icon(tag="delete"),
+                    size='xs',
+                    variant='ghost',
+                    on_click=EditableMessageState.clear_editable_message_error,
+                ),
+                label="Clear error (duplicates the message thread)",
             ),
             height="100%",
         ),
         border_radius="0 0 15px 0",
         color=message.foreground_color,
         background_color=SolarizedColors.red,
         width="100%",
@@ -1300,26 +1338,34 @@
     )
 
 
 def render_message_menu(message: StyledMessage):
     """Render the menu of a message."""
     return pc.popover(
         pc.popover_trigger(
-            pc.button(pc.icon(tag="hamburger"), size='xs', variant='ghost', is_disabled=EditableMessageState.is_editing)
+            render_tooltip(
+                pc.button(
+                    pc.icon(tag="hamburger"), size='xs', variant='ghost', is_disabled=EditableMessageState.is_editing
+                ),
+                label="Show the message menu with more available actions",
+            )
         ),
         pc.popover_content(
             pc.popover_arrow(),
             pc.popover_body(
                 pc.hstack(
                     # pc.button(pc.icon(tag="add"), size='xs', variant='ghost'),
-                    pc.button(
-                        pc.icon(tag="delete"),
-                        size='xs',
-                        variant='ghost',
-                        on_click=EditableMessageState.delete_message(message.uid),
+                    render_tooltip(
+                        pc.button(
+                            pc.icon(tag="delete"),
+                            size='xs',
+                            variant='ghost',
+                            on_click=EditableMessageState.delete_message(message.uid),
+                        ),
+                        label="Delete this message (duplicates the message thread)",
                     ),
                     pc.divider(orientation="vertical", height="1em"),
                     render_edit_thread_button(message),
                     render_fork_thread_button(message),  # type: ignore
                 )
             ),
             pc.popover_close_button(),
@@ -1368,45 +1414,58 @@
 
 
 def render_app_drawer():
     """Render the sidebar that contains all the explorations we have saved."""
 
     def render_exploration_buttons(message_exploration: MessageExploration):
         return pc.hstack(
-            pc.button(
-                pc.cond(
-                    message_exploration.title != "",
-                    pc.text(message_exploration.title),
-                    pc.text("Untitled", as_="i", color=SolarizedColors.base1),
+            render_tooltip(
+                pc.button(
+                    pc.cond(
+                        message_exploration.title != "",
+                        pc.text(message_exploration.title),
+                        pc.text("Untitled", as_="i", color=SolarizedColors.base1),
+                    ),
+                    width="100%",
+                    variant=pc.cond(message_exploration.uid == State.message_exploration_uid, "solid", "outline"),
+                    on_click=State.select_message_exploration(message_exploration.uid),  # type: ignore
+                ),
+                label=pc.cond(
+                    message_exploration.uid == State.message_exploration_uid,
+                    "Return to active exploration",
+                    "Select exploration",
                 ),
-                width="100%",
-                variant=pc.cond(message_exploration.uid == State.message_exploration_uid, "solid", "outline"),
-                on_click=State.select_message_exploration(message_exploration.uid),  # type: ignore
             ),
-            pc.button(
-                pc.icon(tag="delete"),
-                size='xs',
-                variant='ghost',
-                on_click=RemoveExplorationModalState.ask_to_remove(message_exploration.uid),  # type: ignore
+            render_tooltip(
+                pc.button(
+                    pc.icon(tag="delete"),
+                    size='xs',
+                    variant='ghost',
+                    on_click=RemoveExplorationModalState.ask_to_remove(message_exploration.uid),  # type: ignore
+                ),
+                label="Remove exploration",
             ),
         )
 
     return pc.drawer(
         pc.drawer_overlay(
             pc.drawer_content(
                 pc.drawer_header(
                     pc.hstack(
                         pc.text("ChatPlayground"),
                         pc.spacer(),
-                        pc.button(
-                            pc.icon(tag="close"),
-                            on_click=State.set_drawer_visible(False),
-                            float="right",
-                            size='xs',
-                            variant='ghost',
+                        render_tooltip(
+                            pc.button(
+                                pc.icon(tag="close"),
+                                on_click=State.set_drawer_visible(False),
+                                float="right",
+                                size='xs',
+                                variant='ghost',
+                            ),
+                            label="Close the sidebar",
                         ),
                     )
                 ),
                 pc.drawer_body(
                     pc.divider(margin="0.5em"),
                     pc.vstack(
                         pc.foreach(State.get_available_message_explorations, render_exploration_buttons),
@@ -1574,69 +1633,90 @@
 
     The request UI contains the model options and the request button (and the chat UI if chat mode is enabled).
     """
     return pc.cond(
         ~ModelRequestsState.active_generation,
         pc.fragment(
             pc.divider(margin="0.5em"),
-            pc.button(
-                "Request Continuation",
-                on_click=ModelRequestsState.request_chat_model_completion,
+            render_tooltip(
+                pc.button(
+                    "Request Continuation",
+                    on_click=ModelRequestsState.request_chat_model_completion,
+                ),
+                label="Request a continuation from the model given the current messages",
             ),
             pc.cond(
                 ModelRequestsState.chat_mode,
                 pc.fragment(
                     pc.divider(margin="0.5em"),
                     pc.hstack(
                         pc.text_area(
                             placeholder="Write a message...",
                             default_value=ModelRequestsState.user_message_text,
                             width="100%",
                             min_height="5em",
                             on_blur=ModelRequestsState.set_user_message_text,
                         ),
-                        pc.button(
-                            react_icon(as_="TbSend"),
-                            size="lg",
-                            variant="outline",
-                            float="right",
-                            on_click=ModelRequestsState.submit_message,
+                        render_tooltip(
+                            pc.button(
+                                react_icon(as_="TbSend"),
+                                size="lg",
+                                variant="outline",
+                                float="right",
+                                on_click=ModelRequestsState.submit_message,
+                            ),
+                            label="Send message and request a continuation from the model",
                         ),
                     ),
                 ),
             ),
         ),
         pc.fragment(
-            pc.button(
-                pc.spinner(color="blue", size="xs"),
-                pc.text("Cancel", margin_left="1em", on_click=ModelRequestsState.cancel_active_chat_completion),
+            render_tooltip(
+                pc.button(
+                    pc.spinner(color="blue", size="xs"),
+                    pc.text("Cancel", margin_left="1em", on_click=ModelRequestsState.cancel_active_chat_completion),
+                ),
+                label="Cancel the current request and stop the model for generating more text",
             ),
         ),
     )
 
 
 def render_message_exploration(message_thread: MessageThread):
     """Render the overall message exploration UI which includes its title."""
     return pc.box(
         pc.hstack(
             pc.fragment(
-                pc.button(
-                    react_icon(as_="RiSideBarFill"),
-                    size='xs',
-                    variant=pc.cond(State.drawer_visible, 'solid', 'ghost'),
-                    on_click=State.set_drawer_visible(~State.drawer_visible),
+                render_tooltip(
+                    pc.button(
+                        react_icon(as_="RiSideBarFill"),
+                        size='xs',
+                        variant=pc.cond(State.drawer_visible, 'solid', 'ghost'),
+                        on_click=State.set_drawer_visible(~State.drawer_visible),
+                    ),
+                    label="Toggle the drawer to explore other chats",
                 ),
-                pc.button(
-                    react_icon(as_="RiChatNewLine"), variant="ghost", size="xs", on_click=State.new_message_exploration
+                render_tooltip(
+                    pc.button(
+                        react_icon(as_="RiChatNewLine"),
+                        variant="ghost",
+                        size="xs",
+                        on_click=State.new_message_exploration,
+                    ),
+                    label="Start a new chat (the old one is saved)",
                 ),
-                pc.button(
-                    react_icon(as_="BsFillGrid3X3GapFill"),
-                    size='xs',
-                    variant=pc.cond(MessageGridState.is_grid_visible, 'solid', 'ghost'),
-                    on_click=MessageGridState.toggle_grid,
+                render_tooltip(
+                    pc.button(
+                        react_icon(as_="BsFillGrid3X3GapFill"),
+                        size='xs',
+                        variant=pc.cond(MessageGridState.is_grid_visible, 'solid', 'ghost'),
+                        on_click=MessageGridState.toggle_grid,
+                    ),
+                    label="Toggle the expose-like message grid",
                 ),
             ),
             pc.heading(
                 pc.editable(
                     pc.editable_preview(),
                     pc.editable_input(),
                     value=State.title_text,
```

### Comparing `chatplayground-1.0.3/chatplayground/assets/favicon.ico` & `chatplayground-1.1.0/chatplayground/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `chatplayground-1.0.3/chatplayground/assets/react-json-view-lite.css` & `chatplayground-1.1.0/chatplayground/assets/react-json-view-lite.css`

 * *Files identical despite different names*

### Comparing `chatplayground-1.0.3/chatplayground/message_threads/faust_in_oxford_1683330128.209918.json` & `chatplayground-1.1.0/chatplayground/message_threads/faust_in_oxford_1683330128.209918.json`

 * *Files identical despite different names*

### Comparing `chatplayground-1.0.3/chatplayground/pcconfig.py` & `chatplayground-1.1.0/chatplayground/pcconfig.py`

 * *Files identical despite different names*

### Comparing `chatplayground-1.0.3/pyproject.toml` & `chatplayground-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "chatplayground"
-version = "1.0.3"
+version = "1.1.0"
 homepage = "https://github.com/blackhc/chatplayground"
 description = "ChatPlayground for LLMs"
 authors = ["Andreas Kirsch <blackhc@gmail.com>"]
 readme = "README.md"
 license =  "GPL-3.0-only"
 classifiers=[
     'Development Status :: 4 - Beta',
```

### Comparing `chatplayground-1.0.3/PKG-INFO` & `chatplayground-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatplayground
-Version: 1.0.3
+Version: 1.1.0
 Summary: ChatPlayground for LLMs
 Home-page: https://github.com/blackhc/chatplayground
 License: GPL-3.0-only
 Author: Andreas Kirsch
 Author-email: blackhc@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

