# Comparing `tmp/ScraperFC-2.6.5.tar.gz` & `tmp/ScraperFC-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ScraperFC-2.6.5.tar", last modified: Sun Apr  2 03:04:45 2023, max compression
+gzip compressed data, was "ScraperFC-2.7.0.tar", last modified: Wed May 10 03:21:09 2023, max compression
```

## Comparing `ScraperFC-2.6.5.tar` & `ScraperFC-2.7.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-02 03:04:45.625730 ScraperFC-2.6.5/
--rw-rw-rw-   0        0        0    35823 2022-11-23 23:34:52.000000 ScraperFC-2.6.5/LICENSE
--rw-rw-rw-   0        0        0     3168 2023-04-02 03:04:45.624733 ScraperFC-2.6.5/PKG-INFO
--rw-rw-rw-   0        0        0     2498 2023-03-26 16:06:29.000000 ScraperFC-2.6.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-02 03:04:45.596879 ScraperFC-2.6.5/ScraperFC/
--rw-rw-rw-   0        0        0     6732 2022-12-04 23:17:54.000000 ScraperFC-2.6.5/ScraperFC/Capology.py
--rw-rw-rw-   0        0        0     1684 2022-11-23 23:34:52.000000 ScraperFC-2.6.5/ScraperFC/ClubElo.py
--rw-rw-rw-   0        0        0    34737 2023-04-02 02:55:08.000000 ScraperFC-2.6.5/ScraperFC/FBRef.py
--rw-rw-rw-   0        0        0     4706 2023-03-26 16:06:29.000000 ScraperFC-2.6.5/ScraperFC/FiveThirtyEight.py
--rw-rw-rw-   0        0        0     5939 2022-12-04 23:17:54.000000 ScraperFC-2.6.5/ScraperFC/SofaScore.py
--rw-rw-rw-   0        0        0    13349 2023-04-02 02:55:08.000000 ScraperFC-2.6.5/ScraperFC/Transfermarkt.py
--rw-rw-rw-   0        0        0    40942 2023-04-02 02:55:08.000000 ScraperFC-2.6.5/ScraperFC/Understat.py
--rw-rw-rw-   0        0        0      277 2023-04-02 02:55:08.000000 ScraperFC-2.6.5/ScraperFC/__init__.py
--rw-rw-rw-   0        0        0    18391 2023-04-02 02:55:51.000000 ScraperFC-2.6.5/ScraperFC/shared_functions.py
-drwxrwxrwx   0        0        0        0 2023-04-02 03:04:45.621744 ScraperFC-2.6.5/ScraperFC.egg-info/
--rw-rw-rw-   0        0        0     3168 2023-04-02 03:04:44.000000 ScraperFC-2.6.5/ScraperFC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2023-04-02 03:04:45.000000 ScraperFC-2.6.5/ScraperFC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-02 03:04:44.000000 ScraperFC-2.6.5/ScraperFC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2023-04-02 03:04:44.000000 ScraperFC-2.6.5/ScraperFC.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-02 03:04:44.000000 ScraperFC-2.6.5/ScraperFC.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-02 03:04:45.625730 ScraperFC-2.6.5/setup.cfg
--rw-rw-rw-   0        0        0     1197 2023-04-02 02:59:13.000000 ScraperFC-2.6.5/setup.py
+drwxrwxr-x   0 oseymour  (1000) oseymour  (1000)        0 2023-05-10 03:21:09.797895 ScraperFC-2.7.0/
+-rw-rw-r--   0 oseymour  (1000) oseymour  (1000)    35149 2023-05-02 22:58:52.000000 ScraperFC-2.7.0/LICENSE
+-rw-rw-r--   0 oseymour  (1000) oseymour  (1000)     3124 2023-05-10 03:21:09.793895 ScraperFC-2.7.0/PKG-INFO
+-rw-rw-r--   0 oseymour  (1000) oseymour  (1000)     2468 2023-05-02 22:58:52.000000 ScraperFC-2.7.0/README.md
+drwxrwxr-x   0 oseymour  (1000) oseymour  (1000)        0 2023-05-10 03:21:09.793895 ScraperFC-2.7.0/ScraperFC/
+-rw-rw-r--   0 oseymour  (1000) oseymour  (1000)     6548 2023-05-02 22:58:52.000000 ScraperFC-2.7.0/ScraperFC/Capology.py
+-rw-rw-r--   0 oseymour  (1000) oseymour  (1000)     1635 2023-05-02 22:58:52.000000 ScraperFC-2.7.0/ScraperFC/ClubElo.py
+-rw-rw-r--   0 oseymour  (1000) oseymour  (1000)    37482 2023-05-10 03:16:38.000000 ScraperFC-2.7.0/ScraperFC/FBRef.py
+-rw-rw-r--   0 oseymour  (1000) oseymour  (1000)     4584 2023-05-02 22:58:52.000000 ScraperFC-2.7.0/ScraperFC/FiveThirtyEight.py
+-rw-rw-r--   0 oseymour  (1000) oseymour  (1000)     5795 2023-05-02 22:58:52.000000 ScraperFC-2.7.0/ScraperFC/SofaScore.py
+-rw-rw-r--   0 oseymour  (1000) oseymour  (1000)    13070 2023-05-02 22:58:52.000000 ScraperFC-2.7.0/ScraperFC/Transfermarkt.py
+-rw-rw-r--   0 oseymour  (1000) oseymour  (1000)    39921 2023-05-02 22:58:52.000000 ScraperFC-2.7.0/ScraperFC/Understat.py
+-rw-rw-r--   0 oseymour  (1000) oseymour  (1000)      270 2023-05-02 22:58:52.000000 ScraperFC-2.7.0/ScraperFC/__init__.py
+-rw-rw-r--   0 oseymour  (1000) oseymour  (1000)    17942 2023-05-10 03:19:15.000000 ScraperFC-2.7.0/ScraperFC/shared_functions.py
+drwxrwxr-x   0 oseymour  (1000) oseymour  (1000)        0 2023-05-10 03:21:09.793895 ScraperFC-2.7.0/ScraperFC.egg-info/
+-rw-rw-r--   0 oseymour  (1000) oseymour  (1000)     3124 2023-05-10 03:21:09.000000 ScraperFC-2.7.0/ScraperFC.egg-info/PKG-INFO
+-rw-rw-r--   0 oseymour  (1000) oseymour  (1000)      406 2023-05-10 03:21:09.000000 ScraperFC-2.7.0/ScraperFC.egg-info/SOURCES.txt
+-rw-rw-r--   0 oseymour  (1000) oseymour  (1000)        1 2023-05-10 03:21:09.000000 ScraperFC-2.7.0/ScraperFC.egg-info/dependency_links.txt
+-rw-rw-r--   0 oseymour  (1000) oseymour  (1000)       80 2023-05-10 03:21:09.000000 ScraperFC-2.7.0/ScraperFC.egg-info/requires.txt
+-rw-rw-r--   0 oseymour  (1000) oseymour  (1000)       10 2023-05-10 03:21:09.000000 ScraperFC-2.7.0/ScraperFC.egg-info/top_level.txt
+-rw-rw-r--   0 oseymour  (1000) oseymour  (1000)       38 2023-05-10 03:21:09.797895 ScraperFC-2.7.0/setup.cfg
+-rw-rw-r--   0 oseymour  (1000) oseymour  (1000)     1165 2023-05-10 03:19:30.000000 ScraperFC-2.7.0/setup.py
```

### Comparing `ScraperFC-2.6.5/LICENSE` & `ScraperFC-2.7.0/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `ScraperFC-2.6.5/PKG-INFO` & `ScraperFC-2.7.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-Metadata-Version: 2.1
-Name: ScraperFC
-Version: 2.6.5
-Summary: Package for scraping soccer data from a variety of sources.
-Home-page: https://github.com/oseymour/ScraperFC
-Author: Owen Seymour
-Author-email: osmour043@gmail.com
-Keywords: soccer,football,Premier League,Serie A,La Liga,Bundesliga,Ligue 1,web scraping,soccer data,soccer stats,football data,football stats,web scraping soccer stats,web scraping football stats,web scraping soccer data,web scraping football data
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<p align="center">
-  <img src="https://github.com/oseymour/ScraperFC/blob/main/scraperfc_logo.png?raw=true" alt="ScraperFC logo. The underlined text ScraperFC, where the circle of the p is a soccer ball.">
-</p>
-<p align="center">
-  <a href="https://pypi.org/project/ScraperFC/"><img src="https://img.shields.io/pypi/v/scraperfc.svg", alt="pypi version badge"></a>
-  <a href="https://pypi.org/project/ScraperFC/"><img src="https://static.pepy.tech/badge/scraperfc" alt="total pypi downloads badge"/></a>
-  <a href="https://pypi.org/project/ScraperFC/"><img src="https://img.shields.io/pypi/dm/ScraperFC.svg" alt="monthly pypi downloads badge"/></a>
-  <a href="https://pypi.org/project/ScraperFC/"><img src="https://img.shields.io/pypi/dw/ScraperFC.svg" alt="weekly pypi downloads badge"/></a>
-  <a href="https://pypi.org/project/ScraperFC/"><img src="https://img.shields.io/pypi/dd/ScraperFC.svg" alt="dailypypi downloads badge"/></a>
-  <a href="https://scraperfc.readthedocs.io/en/latest/"><img src="https://readthedocs.org/projects/nrc4d/badge/?version=latest" alt="documentation status badge"/></a>
-  <a href="https://github.com/oseymour/ScraperFC"><img src="http://hits.dwyl.com/oseymour/scraperfc.svg?style=flat"></a>
-</p>
-
-This is ScraperFC, a Python package that I hope will give more people access to soccer data. Gone are the days of downloading spreadsheets one-by-one, copy-pasting, or entering data into spreadsheets by hand. I try to make ScraperFC as easy-to-use as possible so that anybody with a bit of Python experience can use it.
-
-To install ScraperFC, run ```pip install ScraperFC``` from the command line.
-
-Data can be scraped from the following sources:
-* [FBRef](https://fbref.com/en/)
-* [Understat](https://understat.com/)
-* [FiveThirtyEight](https://projects.fivethirtyeight.com/soccer-predictions/)
-* [ClubELO](http://clubelo.com/)
-* [Capology](https://www.capology.com/)
-* [Transfermarkt](https://www.transfermarkt.us/)
-
-For documentation, head over to the [Read the Docs page](https://scraperfc.readthedocs.io).
-
-For usage examples, look at Examples.ipynb in the top level directory or some of my example analyses in the analytics_examples folder.
-
-I'd love to hear your feedback, bugs you find, or new features you want! The best way is to open an issue on this repository and I can respond to it there. Otherwise, you can reach me via email at osmour043@gmail.com or my Twitter handle is [@owen_seymour](https://twitter.com/owen_seymour).
+Metadata-Version: 2.1
+Name: ScraperFC
+Version: 2.7.0
+Summary: Package for scraping soccer data from a variety of sources.
+Home-page: https://github.com/oseymour/ScraperFC
+Author: Owen Seymour
+Author-email: osmour043@gmail.com
+Keywords: soccer,football,Premier League,Serie A,La Liga,Bundesliga,Ligue 1,web scraping,soccer data,soccer stats,football data,football stats,web scraping soccer stats,web scraping football stats,web scraping soccer data,web scraping football data
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="center">
+  <img src="https://github.com/oseymour/ScraperFC/blob/main/scraperfc_logo.png?raw=true" alt="ScraperFC logo. The underlined text ScraperFC, where the circle of the p is a soccer ball.">
+</p>
+<p align="center">
+  <a href="https://pypi.org/project/ScraperFC/"><img src="https://img.shields.io/pypi/v/scraperfc.svg", alt="pypi version badge"></a>
+  <a href="https://pypi.org/project/ScraperFC/"><img src="https://static.pepy.tech/badge/scraperfc" alt="total pypi downloads badge"/></a>
+  <a href="https://pypi.org/project/ScraperFC/"><img src="https://img.shields.io/pypi/dm/ScraperFC.svg" alt="monthly pypi downloads badge"/></a>
+  <a href="https://pypi.org/project/ScraperFC/"><img src="https://img.shields.io/pypi/dw/ScraperFC.svg" alt="weekly pypi downloads badge"/></a>
+  <a href="https://pypi.org/project/ScraperFC/"><img src="https://img.shields.io/pypi/dd/ScraperFC.svg" alt="dailypypi downloads badge"/></a>
+  <a href="https://scraperfc.readthedocs.io/en/latest/"><img src="https://readthedocs.org/projects/nrc4d/badge/?version=latest" alt="documentation status badge"/></a>
+  <a href="https://github.com/oseymour/ScraperFC"><img src="http://hits.dwyl.com/oseymour/scraperfc.svg?style=flat"></a>
+</p>
+
+This is ScraperFC, a Python package that I hope will give more people access to soccer data. Gone are the days of downloading spreadsheets one-by-one, copy-pasting, or entering data into spreadsheets by hand. I try to make ScraperFC as easy-to-use as possible so that anybody with a bit of Python experience can use it.
+
+To install ScraperFC, run ```pip install ScraperFC``` from the command line.
+
+Data can be scraped from the following sources:
+* [FBRef](https://fbref.com/en/)
+* [Understat](https://understat.com/)
+* [FiveThirtyEight](https://projects.fivethirtyeight.com/soccer-predictions/)
+* [ClubELO](http://clubelo.com/)
+* [Capology](https://www.capology.com/)
+* [Transfermarkt](https://www.transfermarkt.us/)
+
+For documentation, head over to the [Read the Docs page](https://scraperfc.readthedocs.io).
+
+For usage examples, look at Examples.ipynb in the top level directory or some of my example analyses in the analytics_examples folder.
+
+I'd love to hear your feedback, bugs you find, or new features you want! The best way is to open an issue on this repository and I can respond to it there. Otherwise, you can reach me via email at osmour043@gmail.com or my Twitter handle is [@owen_seymour](https://twitter.com/owen_seymour).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ScraperFC Version: 2.6.5 Summary: Package for
+Metadata-Version: 2.1 Name: ScraperFC Version: 2.7.0 Summary: Package for
 scraping soccer data from a variety of sources. Home-page: https://github.com/
 oseymour/ScraperFC Author: Owen Seymour Author-email: osmour043@gmail.com
 Keywords: soccer,football,Premier League,Serie A,La Liga,Bundesliga,Ligue 1,web
 scraping,soccer data,soccer stats,football data,football stats,web scraping
 soccer stats,web scraping football stats,web scraping soccer data,web scraping
 football data Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
```

### Comparing `ScraperFC-2.6.5/README.md` & `ScraperFC-2.7.0/README.md`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-<p align="center">
-  <img src="https://github.com/oseymour/ScraperFC/blob/main/scraperfc_logo.png?raw=true" alt="ScraperFC logo. The underlined text ScraperFC, where the circle of the p is a soccer ball.">
-</p>
-<p align="center">
-  <a href="https://pypi.org/project/ScraperFC/"><img src="https://img.shields.io/pypi/v/scraperfc.svg", alt="pypi version badge"></a>
-  <a href="https://pypi.org/project/ScraperFC/"><img src="https://static.pepy.tech/badge/scraperfc" alt="total pypi downloads badge"/></a>
-  <a href="https://pypi.org/project/ScraperFC/"><img src="https://img.shields.io/pypi/dm/ScraperFC.svg" alt="monthly pypi downloads badge"/></a>
-  <a href="https://pypi.org/project/ScraperFC/"><img src="https://img.shields.io/pypi/dw/ScraperFC.svg" alt="weekly pypi downloads badge"/></a>
-  <a href="https://pypi.org/project/ScraperFC/"><img src="https://img.shields.io/pypi/dd/ScraperFC.svg" alt="dailypypi downloads badge"/></a>
-  <a href="https://scraperfc.readthedocs.io/en/latest/"><img src="https://readthedocs.org/projects/nrc4d/badge/?version=latest" alt="documentation status badge"/></a>
-  <a href="https://github.com/oseymour/ScraperFC"><img src="http://hits.dwyl.com/oseymour/scraperfc.svg?style=flat"></a>
-</p>
-
-This is ScraperFC, a Python package that I hope will give more people access to soccer data. Gone are the days of downloading spreadsheets one-by-one, copy-pasting, or entering data into spreadsheets by hand. I try to make ScraperFC as easy-to-use as possible so that anybody with a bit of Python experience can use it.
-
-To install ScraperFC, run ```pip install ScraperFC``` from the command line.
-
-Data can be scraped from the following sources:
-* [FBRef](https://fbref.com/en/)
-* [Understat](https://understat.com/)
-* [FiveThirtyEight](https://projects.fivethirtyeight.com/soccer-predictions/)
-* [ClubELO](http://clubelo.com/)
-* [Capology](https://www.capology.com/)
-* [Transfermarkt](https://www.transfermarkt.us/)
-
-For documentation, head over to the [Read the Docs page](https://scraperfc.readthedocs.io).
-
-For usage examples, look at Examples.ipynb in the top level directory or some of my example analyses in the analytics_examples folder.
-
-I'd love to hear your feedback, bugs you find, or new features you want! The best way is to open an issue on this repository and I can respond to it there. Otherwise, you can reach me via email at osmour043@gmail.com or my Twitter handle is [@owen_seymour](https://twitter.com/owen_seymour).
+<p align="center">
+  <img src="https://github.com/oseymour/ScraperFC/blob/main/scraperfc_logo.png?raw=true" alt="ScraperFC logo. The underlined text ScraperFC, where the circle of the p is a soccer ball.">
+</p>
+<p align="center">
+  <a href="https://pypi.org/project/ScraperFC/"><img src="https://img.shields.io/pypi/v/scraperfc.svg", alt="pypi version badge"></a>
+  <a href="https://pypi.org/project/ScraperFC/"><img src="https://static.pepy.tech/badge/scraperfc" alt="total pypi downloads badge"/></a>
+  <a href="https://pypi.org/project/ScraperFC/"><img src="https://img.shields.io/pypi/dm/ScraperFC.svg" alt="monthly pypi downloads badge"/></a>
+  <a href="https://pypi.org/project/ScraperFC/"><img src="https://img.shields.io/pypi/dw/ScraperFC.svg" alt="weekly pypi downloads badge"/></a>
+  <a href="https://pypi.org/project/ScraperFC/"><img src="https://img.shields.io/pypi/dd/ScraperFC.svg" alt="dailypypi downloads badge"/></a>
+  <a href="https://scraperfc.readthedocs.io/en/latest/"><img src="https://readthedocs.org/projects/nrc4d/badge/?version=latest" alt="documentation status badge"/></a>
+  <a href="https://github.com/oseymour/ScraperFC"><img src="http://hits.dwyl.com/oseymour/scraperfc.svg?style=flat"></a>
+</p>
+
+This is ScraperFC, a Python package that I hope will give more people access to soccer data. Gone are the days of downloading spreadsheets one-by-one, copy-pasting, or entering data into spreadsheets by hand. I try to make ScraperFC as easy-to-use as possible so that anybody with a bit of Python experience can use it.
+
+To install ScraperFC, run ```pip install ScraperFC``` from the command line.
+
+Data can be scraped from the following sources:
+* [FBRef](https://fbref.com/en/)
+* [Understat](https://understat.com/)
+* [FiveThirtyEight](https://projects.fivethirtyeight.com/soccer-predictions/)
+* [ClubELO](http://clubelo.com/)
+* [Capology](https://www.capology.com/)
+* [Transfermarkt](https://www.transfermarkt.us/)
+
+For documentation, head over to the [Read the Docs page](https://scraperfc.readthedocs.io).
+
+For usage examples, look at Examples.ipynb in the top level directory or some of my example analyses in the analytics_examples folder.
+
+I'd love to hear your feedback, bugs you find, or new features you want! The best way is to open an issue on this repository and I can respond to it there. Otherwise, you can reach me via email at osmour043@gmail.com or my Twitter handle is [@owen_seymour](https://twitter.com/owen_seymour).
```

### Comparing `ScraperFC-2.6.5/ScraperFC/Capology.py` & `ScraperFC-2.7.0/ScraperFC/Capology.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,184 +1,184 @@
-from selenium import webdriver
-from selenium.webdriver.chrome.options import Options
-from selenium.webdriver.support.ui import WebDriverWait
-from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.common.by import By
-from selenium.common.exceptions import StaleElementReferenceException
-from webdriver_manager.chrome import ChromeDriverManager
-import pandas as pd
-from IPython.display import clear_output
-
-from ScraperFC.shared_functions import *
-
-class Capology():
-
-    ############################################################################
-    def __init__(self):
-        options = Options()
-        options.add_argument('--headless')
-        options.add_argument('window-size=700,600')
-        # Use proxy
-        # don't load images
-        prefs = {'profile.managed_default_content_settings.images': 2}
-        options.add_experimental_option('prefs', prefs)
-        # create driver
-        self.driver = webdriver.Chrome(ChromeDriverManager().install(), options=options)
-        clear_output()
-
-        self.leagues = {
-            'Bundesliga': 'de/1-bundesliga',
-            '2.Bundesliga': '/de/2-bundesliga',
-            'EPL': 'uk/premier-league',
-            'EFL Championship': '/uk/championship',
-            'Serie A': 'it/serie-a',
-            'Serie B': 'it/serie-b',
-            'La Liga': 'es/la-liga',
-            'La Liga 2': 'es/la-liga-2',
-            'Ligue 1': 'fr/ligue-1',
-            'Ligue 2': 'fr/ligue-2',
-            'Eredivisie': '/ne/eredivisie',
-            'Primeira Liga': '/pt/primeira-liga',
-            'Scottish PL': '/uk/scottish-premiership',
-            'Super Lig': '/tr/super-lig',
-            'Belgian 1st Division': 'be/first-division-a'
-        }
-
-        self.valid_currencies = ['eur', 'gbp', 'usd']
-
-
-    ############################################################################
-    def close(self):
-        """ Closes and quits the Selenium WebDriver instance.
-        """
-        self.driver.close()
-        self.driver.quit()
-
-    
-    ############################################################################
-    def scrape_salaries(self, year, league, currency):
-        """ Scrapes player salaries for the given league season.
-        
-        Args
-        ----
-        year : int
-            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
-        league : str
-            League. Look in shared_functions.py for the available leagues for each\
-            module.
-        currency : str
-            The currency for the returned salaries. Options are "eur" for Euro,\
-            "gbp" for British Pount, and "USD" for US Dollar
-        Returns
-        -------
-        : Pandas DataFrame
-            The salaries of all players in the given league season
-        """
-        check_season(year, league, 'Capology')
-        if currency not in self.valid_currencies:
-            raise InvalidCurrencyException()
-
-        
-        league_url = f'https://www.capology.com/{self.leagues[league]}/salaries/{year-1}-{year}'
-
-        self.driver.get(league_url)
-
-        # show all players on one page
-        done = False
-        while not done:
-            try:
-                all_btn = WebDriverWait(
-                    self.driver, 
-                    10,
-                ).until(EC.element_to_be_clickable(
-                    (By.LINK_TEXT, 'All')
-                ))
-                all_btn.click()
-                done = True
-            except StaleElementReferenceException:
-                pass
-
-        # select the currency
-        currency_btn = WebDriverWait(
-            self.driver, 
-            10,
-        ).until(EC.element_to_be_clickable(
-            (By.ID, 'btn_{}'.format(currency))
-        ))
-        self.driver.execute_script('arguments[0].click()', currency_btn)
-
-        # table to pandas df
-        tbody_html = self.driver.find_element(By.ID, 'table')\
-                .find_element(By.TAG_NAME, 'tbody')\
-                .get_attribute('outerHTML')
-        table_html = '<table>' + tbody_html + '</table>'
-        df = pd.read_html(table_html)[0]
-        if df.shape[1] == 13:
-            df = df.drop(columns=[1])
-            df.columns = [
-                'Player', 'Weekly Gross', 'Annual Gross', 'Expiration', 'Length', 
-                'Total Gross', 'Status', 'Pos. group', 'Pos.', 'Age', 'Country', 
-                'Club'
-            ]
-        else:
-            df.columns = [
-                'Player', 'Weekly Gross', 'Annual Gross', 'Adj. Gross', 'Pos. group', 
-                'Age', 'Country', 'Club'
-            ]
-
-        return df
-
-    
-    ############################################################################
-    def scrape_payrolls(self, year, league, currency):
-        """ Scrapes team payrolls for the given league season.
-        
-        Args
-        ----
-        year : int
-            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
-        league : str
-            League. Look in shared_functions.py for the available leagues for each\
-            module.
-        currency : str
-            The currency for the returned salaries. Options are "eur" for Euro,\
-            "gbp" for British Pount, and "USD" for US Dollar
-        Returns
-        -------
-        : Pandas DataFrame
-            The payrolls of all teams in the given league season
-        """
-        check_season(year, league, 'Capology')
-        if currency not in self.valid_currencies:
-            raise InvalidCurrencyException()
-
-        
-        league_url = 'https://www.capology.com/{}/payrolls/{}-{}'.format(self.leagues[league], year-1, year)
-
-        self.driver.get(league_url)
-
-        # select the currency
-        currency_btn = WebDriverWait(
-            self.driver, 
-            10,
-        ).until(EC.element_to_be_clickable(
-            (By.ID, 'btn_{}'.format(currency))
-        ))
-        self.driver.execute_script('arguments[0].click()', currency_btn)
-
-        # table to pandas df
-        table = WebDriverWait(
-            self.driver, 
-            10,
-        ).until(EC.element_to_be_clickable(
-            (By.ID, 'table')
-        ))
-        done = False
-        while not done:
-            df = pd.read_html(table.get_attribute('outerHTML'))[0]
-            done = True if df.shape[0]>0 else False
-        # df.columns = [
-        #     'Club', 'Weekly Gross (000s)', 'Annual Gross (000s)', 'Inflcation-Adj. Gross (000s)',
-        #     'Keeper (000s)', 'Defense (000s)', 'Midfield (000s)', 'Forward (000s)'
-        # ]
-
-        return df
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
+from selenium.webdriver.support.ui import WebDriverWait
+from selenium.webdriver.support import expected_conditions as EC
+from selenium.webdriver.common.by import By
+from selenium.common.exceptions import StaleElementReferenceException
+from webdriver_manager.chrome import ChromeDriverManager
+import pandas as pd
+from IPython.display import clear_output
+
+from ScraperFC.shared_functions import *
+
+class Capology():
+
+    ############################################################################
+    def __init__(self):
+        options = Options()
+        options.add_argument('--headless')
+        options.add_argument('window-size=700,600')
+        # Use proxy
+        # don't load images
+        prefs = {'profile.managed_default_content_settings.images': 2}
+        options.add_experimental_option('prefs', prefs)
+        # create driver
+        self.driver = webdriver.Chrome(ChromeDriverManager().install(), options=options)
+        clear_output()
+
+        self.leagues = {
+            'Bundesliga': 'de/1-bundesliga',
+            '2.Bundesliga': '/de/2-bundesliga',
+            'EPL': 'uk/premier-league',
+            'EFL Championship': '/uk/championship',
+            'Serie A': 'it/serie-a',
+            'Serie B': 'it/serie-b',
+            'La Liga': 'es/la-liga',
+            'La Liga 2': 'es/la-liga-2',
+            'Ligue 1': 'fr/ligue-1',
+            'Ligue 2': 'fr/ligue-2',
+            'Eredivisie': '/ne/eredivisie',
+            'Primeira Liga': '/pt/primeira-liga',
+            'Scottish PL': '/uk/scottish-premiership',
+            'Super Lig': '/tr/super-lig',
+            'Belgian 1st Division': 'be/first-division-a'
+        }
+
+        self.valid_currencies = ['eur', 'gbp', 'usd']
+
+
+    ############################################################################
+    def close(self):
+        """ Closes and quits the Selenium WebDriver instance.
+        """
+        self.driver.close()
+        self.driver.quit()
+
+    
+    ############################################################################
+    def scrape_salaries(self, year, league, currency):
+        """ Scrapes player salaries for the given league season.
+        
+        Args
+        ----
+        year : int
+            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
+        league : str
+            League. Look in shared_functions.py for the available leagues for each\
+            module.
+        currency : str
+            The currency for the returned salaries. Options are "eur" for Euro,\
+            "gbp" for British Pount, and "USD" for US Dollar
+        Returns
+        -------
+        : Pandas DataFrame
+            The salaries of all players in the given league season
+        """
+        check_season(year, league, 'Capology')
+        if currency not in self.valid_currencies:
+            raise InvalidCurrencyException()
+
+        
+        league_url = f'https://www.capology.com/{self.leagues[league]}/salaries/{year-1}-{year}'
+
+        self.driver.get(league_url)
+
+        # show all players on one page
+        done = False
+        while not done:
+            try:
+                all_btn = WebDriverWait(
+                    self.driver, 
+                    10,
+                ).until(EC.element_to_be_clickable(
+                    (By.LINK_TEXT, 'All')
+                ))
+                all_btn.click()
+                done = True
+            except StaleElementReferenceException:
+                pass
+
+        # select the currency
+        currency_btn = WebDriverWait(
+            self.driver, 
+            10,
+        ).until(EC.element_to_be_clickable(
+            (By.ID, 'btn_{}'.format(currency))
+        ))
+        self.driver.execute_script('arguments[0].click()', currency_btn)
+
+        # table to pandas df
+        tbody_html = self.driver.find_element(By.ID, 'table')\
+                .find_element(By.TAG_NAME, 'tbody')\
+                .get_attribute('outerHTML')
+        table_html = '<table>' + tbody_html + '</table>'
+        df = pd.read_html(table_html)[0]
+        if df.shape[1] == 13:
+            df = df.drop(columns=[1])
+            df.columns = [
+                'Player', 'Weekly Gross', 'Annual Gross', 'Expiration', 'Length', 
+                'Total Gross', 'Status', 'Pos. group', 'Pos.', 'Age', 'Country', 
+                'Club'
+            ]
+        else:
+            df.columns = [
+                'Player', 'Weekly Gross', 'Annual Gross', 'Adj. Gross', 'Pos. group', 
+                'Age', 'Country', 'Club'
+            ]
+
+        return df
+
+    
+    ############################################################################
+    def scrape_payrolls(self, year, league, currency):
+        """ Scrapes team payrolls for the given league season.
+        
+        Args
+        ----
+        year : int
+            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
+        league : str
+            League. Look in shared_functions.py for the available leagues for each\
+            module.
+        currency : str
+            The currency for the returned salaries. Options are "eur" for Euro,\
+            "gbp" for British Pount, and "USD" for US Dollar
+        Returns
+        -------
+        : Pandas DataFrame
+            The payrolls of all teams in the given league season
+        """
+        check_season(year, league, 'Capology')
+        if currency not in self.valid_currencies:
+            raise InvalidCurrencyException()
+
+        
+        league_url = 'https://www.capology.com/{}/payrolls/{}-{}'.format(self.leagues[league], year-1, year)
+
+        self.driver.get(league_url)
+
+        # select the currency
+        currency_btn = WebDriverWait(
+            self.driver, 
+            10,
+        ).until(EC.element_to_be_clickable(
+            (By.ID, 'btn_{}'.format(currency))
+        ))
+        self.driver.execute_script('arguments[0].click()', currency_btn)
+
+        # table to pandas df
+        table = WebDriverWait(
+            self.driver, 
+            10,
+        ).until(EC.element_to_be_clickable(
+            (By.ID, 'table')
+        ))
+        done = False
+        while not done:
+            df = pd.read_html(table.get_attribute('outerHTML'))[0]
+            done = True if df.shape[0]>0 else False
+        # df.columns = [
+        #     'Club', 'Weekly Gross (000s)', 'Annual Gross (000s)', 'Inflcation-Adj. Gross (000s)',
+        #     'Keeper (000s)', 'Defense (000s)', 'Midfield (000s)', 'Forward (000s)'
+        # ]
+
+        return df
```

### Comparing `ScraperFC-2.6.5/ScraperFC/ClubElo.py` & `ScraperFC-2.7.0/ScraperFC/ClubElo.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-from datetime import datetime
-from io import StringIO
-from IPython.display import clear_output
-import pandas as pd
-import requests
-import time
-
-class ClubElo:        
-        
-    def scrape_team_on_date(self, team, date):
-        """ Scrapes a team's ELO score on a given date.
-
-        Args
-        ----
-        team : str
-            To get the appropriate team name, go to clubelo.com and find the\
-            team you're looking for. Copy and past the team's name as it\
-            appears in the URL.
-        date : str
-            Must be formatted as YYYY-MM-DD
-        Returns
-        -------
-        elo : int
-            ELO score of the given team on the given date
-        -1 : int
-            -1 if the team has no score on the given date
-        """
-        date = datetime.strptime(date, '%Y-%m-%d')
-        
-        # use ClubElo API to get team data as Pandas DataFrame
-        url = 'http://api.clubelo.com/{}'.format(team)
-        done = False
-        while not done:
-            try:
-                r = requests.get(url)
-                done = True
-            except requests.exceptions.ConnectionError:
-                done = False
-        df = pd.read_csv(StringIO(r.text), sep=',')
-        
-        # find row that given date falls in
-        for i in df.index:
-            from_date = datetime.strptime(df.loc[i,'From'], '%Y-%m-%d')
-            to_date = datetime.strptime(df.loc[i,'To'], '%Y-%m-%d')
-            if (date>from_date and date<to_date) or date==from_date or date==to_date:
-                return df.loc[i,'Elo']
-        
-        return -1 # return -1 if ELO not found for given date
-        
+from datetime import datetime
+from io import StringIO
+from IPython.display import clear_output
+import pandas as pd
+import requests
+import time
+
+class ClubElo:        
+        
+    def scrape_team_on_date(self, team, date):
+        """ Scrapes a team's ELO score on a given date.
+
+        Args
+        ----
+        team : str
+            To get the appropriate team name, go to clubelo.com and find the\
+            team you're looking for. Copy and past the team's name as it\
+            appears in the URL.
+        date : str
+            Must be formatted as YYYY-MM-DD
+        Returns
+        -------
+        elo : int
+            ELO score of the given team on the given date
+        -1 : int
+            -1 if the team has no score on the given date
+        """
+        date = datetime.strptime(date, '%Y-%m-%d')
+        
+        # use ClubElo API to get team data as Pandas DataFrame
+        url = 'http://api.clubelo.com/{}'.format(team)
+        done = False
+        while not done:
+            try:
+                r = requests.get(url)
+                done = True
+            except requests.exceptions.ConnectionError:
+                done = False
+        df = pd.read_csv(StringIO(r.text), sep=',')
+        
+        # find row that given date falls in
+        for i in df.index:
+            from_date = datetime.strptime(df.loc[i,'From'], '%Y-%m-%d')
+            to_date = datetime.strptime(df.loc[i,'To'], '%Y-%m-%d')
+            if (date>from_date and date<to_date) or date==from_date or date==to_date:
+                return df.loc[i,'Elo']
+        
+        return -1 # return -1 if ELO not found for given date
+
```

### Comparing `ScraperFC-2.6.5/ScraperFC/FBRef.py` & `ScraperFC-2.7.0/ScraperFC/FBRef.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,736 +1,802 @@
-from IPython.display import clear_output
-import numpy as np
-import pandas as pd
-from ScraperFC.shared_functions import check_season, xpath_soup, sources, UnavailableSeasonException, \
-    NoMatchLinksException
-from selenium import webdriver
-from selenium.webdriver.chrome.options import Options
-from selenium.webdriver.common.by import By
-from webdriver_manager.chrome import ChromeDriverManager
-from selenium.webdriver.chrome.service import Service as ChromeService
-from urllib.request import urlopen
-import requests
-from bs4 import BeautifulSoup
-from tqdm.auto import tqdm
-import time
-import re
-from datetime import datetime
-
-
-class FBRef:
-    """ ScraperFC module for FBRef
-    """
-    
-    ####################################################################################################################
-    def __init__(self):
- 
-        self.wait_time = 6 # in seconds, as of 30-Oct-2022 FBRef blocks if requesting more than 20 requests/minute
-
-        options = Options()
-#         options.headless = True
-        options.add_argument(
-            'user-agent=Mozilla/5.0 (Windows NT 10.0; Win64; x64) '+\
-            'AppleWebKit/537.36 (KHTML, like Gecko) Chrome/87.0.4280.88 '+\
-            'Safari/537.36'
-        )
-        options.add_argument('window-size=1400,600')
-        options.add_argument('--incognito')
-        prefs = {'profile.managed_default_content_settings.images': 2} # don't load images
-        options.add_experimental_option('prefs', prefs)
-        options.add_argument('--log-level=3')
-        self.driver = webdriver.Chrome(
-            service=ChromeService(ChromeDriverManager().install()),
-            options=options
-        )
-
-        self.stats_categories = {
-            'standard': {'url': 'stats', 'html': 'standard',},
-            'goalkeeping': {'url': 'keepers', 'html': 'keeper',},
-            'advanced goalkeeping': {'url': 'keepersadv','html': 'keeper_adv',},
-            'shooting': {'url': 'shooting', 'html': 'shooting',},
-            'passing': {'url': 'passing', 'html': 'passing',},
-            'pass types': {'url': 'passing_types', 'html': 'passing_types',},
-            'goal and shot creation': {'url': 'gca', 'html': 'gca',},
-            'defensive': {'url': 'defense', 'html': 'defense',},
-            'possession':  {'url': 'possession', 'html': 'possession',},
-            'playing time': {'url': 'playingtime', 'html': 'playing_time',},
-            'misc': {'url': 'misc', 'html': 'misc',},
-        }
-      
-    ####################################################################################################################
-    def close(self):
-        """ Closes and quits the Selenium WebDriver instance.
-        """
-        self.driver.close()
-        self.driver.quit()
-
-    ####################################################################################################################
-    def get(self, url):
-        """ Custom get function just for the FBRef module. 
-        
-        Calls .get() from the Selenium WebDriver and then waits in order to avoid a Too Many Requests HTTPError from \
-        FBRef. 
-        
-        Args
-        ----
-        url : str
-            The URL to get
-        Returns
-        -------
-        None
-        """
-        self.driver.get(url)
-        time.sleep(self.wait_time)
-        
-    ####################################################################################################################
-    def requests_get(self, url):
-        """ Custom requests.get function for the FBRef module
-        
-        Calls requests.get() until the status code is 200.
-
-        Args
-        ----
-        url : Str
-            The URL to get
-        Returns
-        -------
-        : requests.Response
-            The response
-        """
-        got_link = False 
-        while not got_link:
-            # Don't proceed until we've successfully retrieved the page
-            response = requests.get(url)
-            time.sleep(5)
-            if response.status_code == 200:
-                # 200 - OK
-                # 403 - file not found
-                # 500 - server error
-                got_link = True
-        return response
-        
-
-    ####################################################################################################################
-    def get_season_link(self, year, league):
-        """ Returns the URL for the chosen league season.
-
-        Args
-        ----
-        year : int
-            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
-        league : str
-            League. Look in shared_functions.py for the available leagues for each module.
-        Returns
-        -------
-        : str
-            URL to the FBRef page of the chosen league season 
-        """
-        check_season(year,league,"FBRef")
-        
-        url = sources["FBRef"][league]["url"]
-        finder = sources["FBRef"][league]["finder"]
-        
-        # go to the league's history page
-        response = self.requests_get(url)
-        soup = BeautifulSoup(response.content, "html.parser")
-        
-        calendar_years = [str(year-1)+'-'+str(year), str(year)] # list of 1- and 2-calendar years strings to work for any competition
-           
-        # Get url to season
-        for tag in soup.find_all("th", {"data-stat": ["year", "year_id"]}):
-            finder_found = np.any([f in tag.find("a")["href"] for f in finder if tag.find("a")]) # bool, if any finders are found in tag
-            season_found = np.any([tag.getText()==s for s in calendar_years]) # bool, if 1- or 2-calendar years are found in tag
-            if tag.find("a") and finder_found and season_found:
-                return "https://fbref.com"+tag.find("a")["href"]
-        
-        raise UnavailableSeasonException(year, league, "FBRef")
-    
-    ####################################################################################################################
-    def get_match_links(self, year, league):
-        """ Gets all match links for the chosen league season.
-
-        Args
-        ----
-        year : int
-            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
-        league : str
-            League. Look in shared_functions.py for the available leagues for each module.
-        Returns
-        -------
-        : list
-            FBRef links to all matches for the chosen league season
-        """
-        check_season(year,league,'FBRef')
-
-        print('Gathering match links.')
-        season_link = self.get_season_link(year, league)
-        if season_link == -1:
-            return None
-        
-        # go to the scores and fixtures page
-        split = season_link.split('/')
-        first_half = '/'.join(split[:-1])
-        second_half = split[-1].split('-')
-        second_half = '-'.join(second_half[:-1])+'-Score-and-Fixtures'
-        fixtures_url = first_half+'/schedule/'+second_half
-        response = self.requests_get(fixtures_url)
-        soup = BeautifulSoup(response.content, 'html.parser')
-
-        # check if there are any scores elements with links. if not, no match links are present
-        scores_links = [t.find(href=True) for t in soup.find_all("td", {"data-stat": "score"}) if t.find(href=True)]
-        if len(scores_links) == 0:
-            raise NoMatchLinksException(fixtures_url, year, league)
-        
-        # find all of the match links from the scores and fixtures page that have the sources finder
-        finders = sources["FBRef"][league]["finder"]
-        match_links = [
-            "https://fbref.com"+t["href"] 
-            for t in scores_links 
-            if t and np.any([f in t["href"] for f in finders])
-        ]
-        
-        return match_links
-
-    ####################################################################################################################
-    def scrape_league_table(self, year, league):
-        """ Scrapes the league table of the chosen league season
-
-        Args
-        ----
-        year : int
-            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
-        league : str
-            League. Look in shared_functions.py for the available leagues for each module.
-        Returns
-        -------
-        : Pandas DataFrame
-            If league is not MLS, dataframe of the scraped league table
-        : tuple
-            If the league is MLS, a tuple of (west conference table, east conference table). Both tables are \
-            dataframes.
-        """
-        check_season(year,league,'FBRef')
-
-        print('Scraping {} {} league table'.format(year, league))
-        
-        season_url = self.get_season_link(year, league)
-        response = self.requests_get(season_url)
-        soup = BeautifulSoup(response.content, 'html.parser')
-        
-        lg_table_html = soup.find_all('table', {'id': re.compile('overall')})
-
-        if league != 'MLS':
-            assert len(lg_table_html) == 1
-            lg_table_html = lg_table_html[0]
-            lg_table = pd.read_html(str(lg_table_html))[0]
-            return lg_table
-
-        else:
-            assert len(lg_table_html) == 2
-            east_table = pd.read_html(str(lg_table_html[0]))[0]
-            west_table = pd.read_html(str(lg_table_html[1]))[0]
-            return (east_table, west_table)
-        
-    ####################################################################################################################
-    def scrape_stats(self, year, league, stat_category, normalize=False):
-        """ Scrapes a single stats category
-        
-        Adds team and player ID columns to the stats tables
-        
-        Args
-        ----
-        year : int
-            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
-        league : str
-            League. Look in shared_functions.py for the available leagues for each module.
-        stat_cateogry : str
-            The stat category to scrape.
-        normalize : bool
-            OPTIONAL, default is False. If True, will normalize all stats to Per90.
-        Returns
-        -------
-        : tuple
-            tuple of 3 Pandas DataFrames, (squad_stats, opponent_stats, player_stats).
-        """
-        check_season(year,league,'FBRef')
-        
-        # Verify valid stat category
-        if stat_category not in self.stats_categories.keys():
-            raise Exception(
-                f'"{stat_category}" is not a valid FBRef stats category. '+\
-                f'Must be one of {list(self.stats_categories.keys())}.'
-            )
-        
-        # Get URL to stat category
-        season_url = self.get_season_link(year, league)
-        old_suffix = season_url.split('/')[-1]
-        new_suffix = f'{self.stats_categories[stat_category]["url"]}/{old_suffix}'
-        new_url = season_url.replace(old_suffix, new_suffix)
-
-        self.get(new_url) # webdrive to link
-        soup = BeautifulSoup(self.driver.page_source, 'html.parser') # get initial soup
-
-        # Normalize button, if requested
-        if normalize:
-            # click all per90 toggles on the page
-            per90_toggles = soup.find_all('button', {'id': re.compile('per_match_toggle')})
-            for toggle in per90_toggles:
-                xpath = xpath_soup(toggle)
-                button_el = self.driver.find_element(By.XPATH, xpath)
-                self.driver.execute_script('arguments[0].click()', button_el)
-            # update the soup
-            soup = BeautifulSoup(self.driver.page_source, 'html.parser')
-
-        # Gather stats table tags
-        squad_stats_tag = soup.find('table', {'id': re.compile('for')})
-        opponent_stats_tag = soup.find('table', {'id': re.compile('against')})
-        player_stats_tag = soup.find(
-            'table', 
-            {'id': re.compile(f'stats_{self.stats_categories[stat_category]["html"]}')}
-        )
-        
-        # Get stats dataframes
-        squad_stats = pd.read_html(str(squad_stats_tag))[0] if squad_stats_tag is not None else None
-        opponent_stats = pd.read_html(str(opponent_stats_tag))[0] if opponent_stats_tag is not None else None
-        player_stats = pd.read_html(str(player_stats_tag))[0] if player_stats_tag is not None else None
-
-        # Drop rows that contain duplicated table headers
-        squad_stats = squad_stats[
-            (~squad_stats[('Unnamed: 0_level_0','Squad')].isna()) 
-            & (squad_stats[('Unnamed: 0_level_0','Squad')]!="Squad")
-        ].reset_index(drop=True)
-        opponent_stats = opponent_stats[
-            (~opponent_stats[('Unnamed: 0_level_0','Squad')].isna()) 
-            & (opponent_stats[('Unnamed: 0_level_0','Squad')]!="Squad")
-        ].reset_index(drop=True)
-        player_stats = player_stats[player_stats[('Unnamed: 0_level_0','Rk')] != 'Rk'].reset_index(drop=True)
-        
-        # Add team ID's
-        if squad_stats is not None:
-            squad_stats['Team ID'] = [
-                tag.find('a')['href'].split('/')[3] 
-                for tag 
-                in squad_stats_tag.find_all('th', {'data-stat': 'team'})[1:]
-                if tag and tag.find('a')
-            ]
-        if opponent_stats is not None:
-            opponent_stats['Team ID'] = [
-                tag.find('a')['href'].split('/')[3] 
-                for tag 
-                in opponent_stats_tag.find_all('th', {'data-stat': 'team'})[1:]
-                if tag and tag.find('a')
-            ]
-        
-        # Add player links and ID's
-        if player_stats is not None:
-            player_links = [
-                'https://fbref.com' + tag.find('a')['href']
-                for tag 
-                in player_stats_tag.find_all('td', {'data-stat': 'player'})
-                if tag and tag.find('a')
-            ]
-            player_stats['Player Link'] = player_links
-            player_stats['Player ID'] = [l.split('/')[-2] for l in player_links]
-        
-        return squad_stats, opponent_stats, player_stats
-    
-    ####################################################################################################################
-    def scrape_all_stats(self, year, league, normalize=False):
-        """ Scrapes all stat categories
-        
-        Runs scrape_stats() for each stats category on dumps the returned tuple of dataframes into a dict.
-        
-        Args
-        ----
-        year : int
-            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
-        league : str
-            League. Look in shared_functions.py for the available leagues for each module.
-        normalize : bool
-            OPTIONAL, default is False. If True, will normalize all stats to Per90.
-        Returns
-        -------
-        : dict
-            Keys are stat category names, values are tuples of 3 dataframes, (squad_stats, opponent_stats, player_stats)
-        """
-        check_season(year,league,'FBRef')
-        
-        return_package = dict()
-        for stat_category in tqdm(self.stats_categories):
-            stats = self.scrape_stats(year, league, stat_category, normalize)
-            return_package[stat_category] = stats
-            
-        return return_package
-
-    ####################################################################################################################
-    def scrape_matches(self, year, league, save=False):
-        """ Scrapes the FBRef standard stats page of the chosen league season.
-            
-        Works by gathering all of the match URL's from the homepage of the chosen league season on FBRef and then \
-        calling scrape_match() on each one.
-
-        Args
-        ----
-        year : int
-            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
-        league : str
-            League. Look in shared_functions.py for the available leagues for each module.
-        save : bool
-            OPTIONAL, default is False. If True, will save the returned DataFrame to a CSV file.
-        Returns
-        -------
-        : Pandas DataFrame
-            If save is False, will return the Pandas DataFrame with the the stats. 
-        filename : str
-            If save is True, will return the filename the CSV was saved to.
-        """
-        check_season(year,league,'FBRef')
-        
-        season = str(year-1)+'-'+str(year)
-        links = self.get_match_links(year,league)
-        
-        matches = pd.DataFrame() # initialize df
-        
-        # scrape match data
-        print('Scraping matches.')
-        time.sleep(1)
-        for link in tqdm(links):
-            try:
-                match = self.scrape_match(link)
-                matches = pd.concat([matches, match], ignore_index=True)
-            except Exception as E:
-                print(f'Failed scraping match {link}')
-                raise E
-            
-        # sort df by match date
-        matches = matches.sort_values(by='Date').reset_index(drop=True)
-        
-        # save to CSV if requested by user
-        if save:
-            filename = f'{season}_{league.replace(" ","_")}_FBRef_matches.csv'
-            matches.to_csv(path_or_buf=filename, index=False)
-            print('Matches dataframe saved to ' + filename)
-            return filename
-        else:
-            return matches
-        
-    ####################################################################################################################
-    def scrape_match(self, link):
-        """ Scrapes an FBRef match page.
-        
-        Args
-        ----
-        link : str
-            URL to the FBRef match page
-        Returns
-        -------
-        : Pandas DataFrame
-            DataFrame containing most parts of the match page if they're available (e.g. formations, lineups, scores, \
-            player stats, etc.). The fields that are available vary by competition and year.
-        """
-        response = self.requests_get(link)
-        soup = BeautifulSoup(response.content, 'html.parser')
-        
-        # Matchweek/stage ==============================================================================================
-        stage_el = list(soup.find('a', {'href': re.compile('-Stats')}, string=True).parents)[0]
-        stage_text = stage_el.getText().split("(")[1].split(")")[0].strip()
-        if "matchweek" in stage_text:
-            stage = int(stage_text.lower().replace("matchweek","").strip())
-        else:
-            stage = stage_text
-
-        # Team names and ids ===========================================================================================
-        team_els = [
-            el.find('a') \
-            for el 
-            in soup.find('div', {'class': 'scorebox'}).find_all('strong') \
-            if el.find('a', href=True) is not None
-        ][:2]
-        home_team_name = team_els[0].getText()
-        home_team_id   = team_els[0]['href'].split('/')[3]
-        away_team_name = team_els[1].getText()
-        away_team_id   = team_els[1]['href'].split('/')[3]
-        
-        # Scores =======================================================================================================
-        scores = soup.find('div', {'class': 'scorebox'}).find_all('div', {'class': 'score'})
-
-        # Formations ===================================================================================================
-        lineup_tags = [tag.find('table') for tag in soup.find_all('div', {'class': 'lineup'})]
-        
-        # Player stats =================================================================================================
-        # Use table ID's to find the appropriate table. More flexible than xpath
-        player_stats = dict()
-        for i, (team, team_id) in enumerate([('Home',home_team_id), ('Away',away_team_id)]):
-
-            summary_tag = soup.find_all('table', {'id': re.compile(f'stats_{team_id}_summary')})
-            assert len(summary_tag) < 2
-            summary_df = pd.read_html(str(summary_tag[0]))[0] if len(summary_tag)==1 else None
-
-            gk_tag = soup.find_all('table', {'id': re.compile(f'keeper_stats_{team_id}')})
-            assert len(gk_tag) < 2
-            gk_df = pd.read_html(str(gk_tag[0]))[0] if len(gk_tag)==1 else None
-
-            passing_tag = soup.find_all('table', {'id': re.compile(f'stats_{team_id}_passing$')})
-            assert len(passing_tag) < 2
-            passing_df = pd.read_html(str(passing_tag[0]))[0] if len(passing_tag)==1 else None
-
-            pass_types_tag = soup.find_all('table', {'id': re.compile(f'stats_{team_id}_passing_types')})
-            assert len(pass_types_tag) < 2
-            pass_types_df = pd.read_html(str(pass_types_tag[0]))[0] if len(pass_types_tag)==1 else None
-
-            defense_tag = soup.find_all('table', {'id': re.compile(f'stats_{team_id}_defense')})
-            assert len(defense_tag) < 2
-            defense_df = pd.read_html(str(defense_tag[0]))[0] if len(defense_tag)==1 else None
-
-            possession_tag = soup.find_all('table', {'id': re.compile(f'stats_{team_id}_possession')})
-            assert len(possession_tag) < 2
-            possession_df = pd.read_html(str(possession_tag[0]))[0] if len(possession_tag)==1 else None
-
-            misc_tag = soup.find_all('table', {'id': re.compile(f'stats_{team_id}_misc')})
-            assert len(misc_tag) < 2
-            misc_df = pd.read_html(str(misc_tag[0]))[0] if len(misc_tag)==1 else None
-            
-            lineup_df = pd.read_html(str(lineup_tags[i]))[0] if len(lineup_tags)!=0 else None
-            
-            # Field player ID's for the stats tables -------------------------------------------------------------------
-            # Note: if a coach gets a yellow/red card, they appear in the player stats tables, in their own row, at the 
-            # bottom.
-            if summary_df is not None:
-                player_ids = list()
-                # Iterate across all els that are player/coach names in the summary stats table
-                for tag in summary_tag[0].find_all('th', {'data-stat':'player', 'scope':'row', 'class':'left'}):
-                    if tag.find('a'):
-                        # if th el has an a subel, it should contain an href link to the player
-                        player_id = tag.find('a')['href'].split('/')[3]
-                    else:
-                        # coaches and the summary row have now a subel (and no player id)
-                        player_id = ''
-                    player_ids.append(player_id)
-                
-                summary_df['Player ID'] = player_ids
-                if passing_df is not None:
-                    passing_df['Player ID'] = player_ids
-                if pass_types_df is not None:
-                    pass_types_df['Player ID'] = player_ids
-                if defense_df is not None:
-                    defense_df['Player ID'] = player_ids
-                if possession_df is not None:
-                    possession_df['Player ID'] = player_ids
-                if misc_df is not None:
-                    misc_df['Player ID'] = player_ids
-
-            # GK ID's --------------------------------------------------------------------------------------------------
-            if gk_df is not None:
-                gk_ids = [
-                    tag.find('a')['href'].split('/')[3]
-                    for tag 
-                    in gk_tag[0].find_all('th', {'data-stat': 'player'})
-                    if tag.find('a')
-                ]
-                
-                gk_df['Player ID'] = gk_ids
-
-            # Build player stats dict ----------------------------------------------------------------------------------
-            # This will be turned into a Series and then put into the match dataframe
-            player_stats[team] = {
-                'Team Sheet': lineup_df,
-                'Summary': summary_df,
-                'GK': gk_df,
-                'Passing': passing_df,
-                'Pass Types': pass_types_df,
-                'Defense': defense_df,
-                'Possession': possession_df,
-                'Misc': misc_df,
-            }
-            
-        # Shots ========================================================================================================
-        both_shots = soup.find_all('table', {'id': 'shots_all'})
-        if len(both_shots) == 1:
-            both_shots = pd.read_html(str(both_shots[0]))[0]
-            both_shots = both_shots[~both_shots.isna().all(axis=1)]
-        else:
-            both_shots = None
-        home_shots = soup.find_all('table', {'id': f'shots_{home_team_id}'})
-        if len(home_shots) == 1:
-            home_shots = pd.read_html(str(home_shots[0]))[0]
-            home_shots = home_shots[~home_shots.isna().all(axis=1)]
-        else:
-            home_shots = None
-        away_shots = soup.find_all('table', {'id': f'shots_{away_team_id}'})
-        if len(away_shots) == 1:
-            away_shots = pd.read_html(str(away_shots[0]))[0]
-            away_shots = away_shots[~away_shots.isna().all(axis=1)]
-        else:
-            away_shots = None
-            
-        # Expected stats flag ==========================================================================================
-        expected = 'Expected' in player_stats['Home']['Summary'].columns.get_level_values(0)
-
-        # Build match series ===========================================================================================
-        match = pd.Series(dtype=object)
-        match['Link'] = link
-        match['Date'] = datetime.strptime(
-            str(soup.find('h1'))
-                .split('<br/>')[0]
-                .split('–')[-1] # not a normal dash
-                .replace('</h1>','')
-                .split('(')[0]
-                .strip(),
-            '%A %B %d, %Y'
-        ).date()
-        match['Stage'] = stage
-        match['Home Team'] = home_team_name
-        match['Away Team'] = away_team_name
-        match['Home Team ID'] = home_team_id
-        match['Away Team ID'] = away_team_id
-        match['Home Formation'] = (
-            player_stats['Home']['Team Sheet'].columns[0].split('(')[-1].replace(')','').strip()
-            if player_stats['Home']['Team Sheet'] is not None else None
-        )
-        match['Away Formation'] = (
-            player_stats['Away']['Team Sheet'].columns[0].split('(')[-1].replace(')','').strip()
-            if player_stats['Away']['Team Sheet'] is not None else None
-        )
-        match['Home Goals'] = int(scores[0].getText()) if scores[0].getText().isdecimal() else None
-        match['Away Goals'] = int(scores[1].getText()) if scores[1].getText().isdecimal() else None
-        match['Home Ast'] = player_stats['Home']['Summary'][('Performance','Ast')].values[-1]
-        match['Away Ast'] = player_stats['Away']['Summary'][('Performance','Ast')].values[-1]
-        match['Home xG'] = player_stats['Home']['Summary'][('Expected','xG')].values[-1] if expected else None
-        match['Away xG'] = player_stats['Away']['Summary'][('Expected','xG')].values[-1] if expected else None
-        match['Home npxG'] = player_stats['Home']['Summary'][('Expected','npxG')].values[-1] if expected else None
-        match['Away npxG'] = player_stats['Away']['Summary'][('Expected','npxG')].values[-1] if expected else None
-        match['Home xAG'] = player_stats['Home']['Summary'][('Expected','xAG')].values[-1] if expected else None
-        match['Away xAG'] = player_stats['Away']['Summary'][('Expected','xAG')].values[-1] if expected else None
-        match['Home Player Stats'] = pd.Series(player_stats['Home']).to_frame().T
-        match['Away Player Stats'] = pd.Series(player_stats['Away']).to_frame().T
-        match['Shots'] = pd.Series({'Both': both_shots, 'Home': home_shots, 'Away': away_shots,}).to_frame().T
-        
-        match = match.to_frame().T # series to dataframe
-        
-        return match
-    
-    ####################################################################################################################
-    def scrape_complete_scouting_reports(self, year, league, goalkeepers=False):
-        """ Scrapes the FBRef scouting reports for all players in the chosen league season.
-
-        Args
-        ----
-        year : int
-            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
-        league : str
-            League. Look in shared_functions.py for the available leagues for each module.
-        goalkeepers : bool
-            OPTIONAL, default is False. If True, will scrape reports for only goalkeepers. If False, will scrape \
-            reports for only outfield players.
-        Returns
-        -------
-        per90 : Pandas DataFrame
-            DataFrame of reports with Per90 stats.
-        percentiles : Pandas DataFrame
-            DataFrame of reports with stats percentiles (versus other players in the top 5 leagues)
-        """
-        # Get the player links
-        if goalkeepers:
-            player_links = self.scrape_stats(year, league, 'goalkeeping')[2]['Player Link'].values
-        else:
-            player_links = self.scrape_stats(year, league, 'standard')[2]['Player Link'].values
-        
-        # initialize dataframes
-        per90_df = pd.DataFrame()
-        percentiles_df = pd.DataFrame()
-        
-        # gather complete reports and append to dataframes
-        for player_link in tqdm(player_links):
-            report, name, pos, mins = self.complete_report_from_player_link(player_link)
-            # skip players without reports
-            if type(report) is int and report==-1:
-                continue
-            
-            # separate per90 and percentiles and add player name, position, and minutes
-            per90 = report['Per 90'].to_frame().T
-            percentile = report['Percentile'].to_frame().T
-            for col, val in [('Name',name), ('Position',pos), ('Minutes',mins)]:
-                per90[col] = val
-                percentile[col] = val
-            
-            # skip players who don't have a complete report or goalkeepers if scraping goalkeeper stats
-            if (type(report) is int) or (not goalkeepers and per90['Position'].values[0]=='Goalkeepers'):
-                continue
-                
-            # append
-            per90_df = pd.concat([per90_df, per90], ignore_index=True)
-            percentiles_df = pd.concat([percentiles_df, percentile], ignore_index=True)
-        
-        return per90_df, percentiles_df
-    
-    ####################################################################################################################
-    def complete_report_from_player_link(self, player_link):
-        """ Scrapes the FBRef scouting reports for a player.
-        
-        Args
-        ----
-        player_link : str
-            URL to an FBRef player page
-        Returns
-        -------
-        cleaned_complete_report : Pandas DataFrame
-            Complete report with a MultiIndex of stats categories and statistics. Columns for per90 and percentile values.
-        player_name : str
-        player_pos : str
-        minutes : int
-        """
-        # return -1 if the player has no scouting report
-        player_link_html = urlopen(player_link).read().decode('utf8')
-        if 'view complete scouting report' not in player_link_html.lower():
-            return -1, -1, -1, -1
-
-        #### Get link to complete report ####
-        soup = BeautifulSoup(requests.get(player_link).content, 'lxml')
-        complete_report_link = soup\
-            .find('div', {'id': 'all_scout'})\
-            .find('div', {'class': 'section_heading_text'})\
-            .find('a', href=True)['href']
-        complete_report_link = 'https://fbref.com' + complete_report_link
-        self.get(complete_report_link)
-
-        #### Load and prelim clean of complete report ####
-        soup = BeautifulSoup(requests.get(complete_report_link).content, 'lxml')
-        complete_report = pd.read_html(str(soup.find('table', {'id': re.compile(f'scout_full')})))[0] # load report
-        complete_report.columns = complete_report.columns.get_level_values(1) # drop top level column name
-        complete_report.dropna(axis=0, inplace=True) # drop nan rows
-        complete_report.reset_index(inplace=True, drop=True) # reset index
-
-        # Row masks
-        header_row_mask = complete_report.eq(complete_report.iloc[:,0], axis=0).all(1) # rows with stats category header names
-
-        #### Create multiindex column names broken down by stats category ####
-        cleaned_complete_report = pd.DataFrame()
-        stats_categories = ('Standard',) + tuple(complete_report[header_row_mask]['Statistic'].values)
-        category_starts = [0,] + list(np.where(header_row_mask)[0]+2) # 2 to skip past category name row and col name row
-        category_ends = list(np.where(header_row_mask)[0]-1) + [complete_report.shape[0]-1]
-        for i in range(len(stats_categories)):
-            temp = complete_report.loc[category_starts[i]:category_ends[i],:]
-            temp.index = pd.MultiIndex.from_product([
-                (stats_categories[i],),
-                temp['Statistic'],
-            ])
-            cleaned_complete_report = pd.concat([cleaned_complete_report,temp])
-        # drop statistic name column, it's in the multiindex now
-        cleaned_complete_report.drop(columns='Statistic', inplace=True)
-        cleaned_complete_report['Per 90'] = cleaned_complete_report['Per 90'].str.rstrip('%').astype('float')
-        cleaned_complete_report['Percentile'] = cleaned_complete_report['Percentile'].astype(int)
-        
-        #### Get player names, positions, and minutes played ####
-        player_name = ' '.join(complete_report_link.split('/')[-1].split('-')[:-2])
-        player_pos = soup.find('div', {'id': 'all_scout'}).find('div', {'class': 'current'}).text.split('vs.')[-1].strip()
-        minutes = int(
-            soup.find('div', {'id': 'all_scout'})\
-                .find('div', {'class': 'footer no_hide_long'})\
-                .find('div')\
-                .text\
-                .split(' minutes')[0]\
-                .split(' ')[-1]
-        )
-
-        return cleaned_complete_report, player_name, player_pos, minutes
+from IPython.display import clear_output
+import numpy as np
+import pandas as pd
+from ScraperFC.shared_functions import check_season, xpath_soup, sources, UnavailableSeasonException, \
+    NoMatchLinksException
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
+from selenium.webdriver.common.by import By
+from webdriver_manager.chrome import ChromeDriverManager
+from selenium.webdriver.chrome.service import Service as ChromeService
+from urllib.request import urlopen
+import requests
+from bs4 import BeautifulSoup
+from tqdm.auto import tqdm
+import time
+import re
+from datetime import datetime
+
+
+class FBRef:
+    """ ScraperFC module for FBRef
+    """
+    
+    ####################################################################################################################
+    def __init__(self):
+ 
+        self.wait_time = 6 # in seconds, as of 30-Oct-2022 FBRef blocks if requesting more than 20 requests/minute
+
+        options = Options()
+#         options.headless = True
+        options.add_argument(
+            'user-agent=Mozilla/5.0 (Windows NT 10.0; Win64; x64) '+\
+            'AppleWebKit/537.36 (KHTML, like Gecko) Chrome/87.0.4280.88 '+\
+            'Safari/537.36'
+        )
+        options.add_argument('window-size=1400,600')
+        options.add_argument('--incognito')
+        prefs = {'profile.managed_default_content_settings.images': 2} # don't load images
+        options.add_experimental_option('prefs', prefs)
+        options.add_argument('--log-level=3')
+        chromedriver_path = ChromeDriverManager().install()
+        chrome_service = ChromeService(chromedriver_path)
+        self.driver = webdriver.Chrome(service=chrome_service, options=options)
+
+        self.stats_categories = {
+            'standard': {'url': 'stats', 'html': 'standard',},
+            'goalkeeping': {'url': 'keepers', 'html': 'keeper',},
+            'advanced goalkeeping': {'url': 'keepersadv','html': 'keeper_adv',},
+            'shooting': {'url': 'shooting', 'html': 'shooting',},
+            'passing': {'url': 'passing', 'html': 'passing',},
+            'pass types': {'url': 'passing_types', 'html': 'passing_types',},
+            'goal and shot creation': {'url': 'gca', 'html': 'gca',},
+            'defensive': {'url': 'defense', 'html': 'defense',},
+            'possession':  {'url': 'possession', 'html': 'possession',},
+            'playing time': {'url': 'playingtime', 'html': 'playing_time',},
+            'misc': {'url': 'misc', 'html': 'misc',},
+        }
+      
+    ####################################################################################################################
+    def close(self):
+        """ Closes and quits the Selenium WebDriver instance.
+        """
+        self.driver.close()
+        self.driver.quit()
+
+    ####################################################################################################################
+    def get(self, url):
+        """ Custom get function just for the FBRef module. 
+        
+        Calls .get() from the Selenium WebDriver and then waits in order to avoid a Too Many Requests HTTPError from \
+        FBRef. 
+        
+        Args
+        ----
+        url : str
+            The URL to get
+        Returns
+        -------
+        None
+        """
+        self.driver.get(url)
+        time.sleep(self.wait_time)
+        
+    ####################################################################################################################
+    def requests_get(self, url):
+        """ Custom requests.get function for the FBRef module
+        
+        Calls requests.get() until the status code is 200.
+
+        Args
+        ----
+        url : Str
+            The URL to get
+        Returns
+        -------
+        : requests.Response
+            The response
+        """
+        got_link = False 
+        while not got_link:
+            # Don't proceed until we've successfully retrieved the page
+            response = requests.get(url)
+            time.sleep(5)
+            if response.status_code == 200:
+                # 200 - OK
+                # 403 - file not found
+                # 500 - server error
+                got_link = True
+        return response
+        
+
+    ####################################################################################################################
+    def get_season_link(self, year, league):
+        """ Returns the URL for the chosen league season.
+
+        Args
+        ----
+        year : int
+            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
+        league : str
+            League. Look in shared_functions.py for the available leagues for each module.
+        Returns
+        -------
+        : str
+            URL to the FBRef page of the chosen league season 
+        """
+        check_season(year,league,"FBRef")
+        
+        url = sources["FBRef"][league]["url"]
+        finder = sources["FBRef"][league]["finder"]
+        
+        # go to the league's history page
+        response = self.requests_get(url)
+        soup = BeautifulSoup(response.content, "html.parser")
+        
+        calendar_years = [str(year-1)+'-'+str(year), str(year)] # list of 1- and 2-calendar years strings to work for any competition
+           
+        # Get url to season
+        for tag in soup.find_all("th", {"data-stat": ["year", "year_id"]}):
+            finder_found = np.any([f in tag.find("a")["href"] for f in finder if tag.find("a")]) # bool, if any finders are found in tag
+            season_found = np.any([tag.getText()==s for s in calendar_years]) # bool, if 1- or 2-calendar years are found in tag
+            if tag.find("a") and finder_found and season_found:
+                return "https://fbref.com"+tag.find("a")["href"]
+        
+        raise UnavailableSeasonException(year, league, "FBRef")
+    
+    ####################################################################################################################
+    def get_match_links(self, year, league):
+        """ Gets all match links for the chosen league season.
+
+        Args
+        ----
+        year : int
+            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
+        league : str
+            League. Look in shared_functions.py for the available leagues for each module.
+        Returns
+        -------
+        : list
+            FBRef links to all matches for the chosen league season
+        """
+        check_season(year,league,'FBRef')
+
+        print('Gathering match links.')
+        season_link = self.get_season_link(year, league)
+        if season_link == -1:
+            return None
+        
+        # go to the scores and fixtures page
+        split = season_link.split('/')
+        first_half = '/'.join(split[:-1])
+        second_half = split[-1].split('-')
+        second_half = '-'.join(second_half[:-1])+'-Score-and-Fixtures'
+        fixtures_url = first_half+'/schedule/'+second_half
+        response = self.requests_get(fixtures_url)
+        soup = BeautifulSoup(response.content, 'html.parser')
+
+        # check if there are any scores elements with links. if not, no match links are present
+        scores_links = [t.find(href=True) for t in soup.find_all("td", {"data-stat": "score"}) if t.find(href=True)]
+        if len(scores_links) == 0:
+            raise NoMatchLinksException(fixtures_url, year, league)
+        
+        # find all of the match links from the scores and fixtures page that have the sources finder
+        finders = sources["FBRef"][league]["finder"]
+        match_links = [
+            "https://fbref.com"+t["href"] 
+            for t in scores_links 
+            if t and np.any([f in t["href"] for f in finders])
+        ]
+        
+        return match_links
+
+    ####################################################################################################################
+    def scrape_league_table(self, year, league):
+        """ Scrapes the league table of the chosen league season
+
+        Args
+        ----
+        year : int
+            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
+        league : str
+            League. Look in shared_functions.py for the available leagues for each module.
+        Returns
+        -------
+        : Pandas DataFrame
+            If league is not MLS, dataframe of the scraped league table
+        : tuple
+            If the league is MLS, a tuple of (west conference table, east conference table). Both tables are \
+            dataframes.
+        """
+        check_season(year,league,'FBRef')
+
+        print('Scraping {} {} league table'.format(year, league))
+        
+        season_url = self.get_season_link(year, league)
+        response = self.requests_get(season_url)
+        soup = BeautifulSoup(response.content, 'html.parser')
+        
+        lg_table_html = soup.find_all('table', {'id': re.compile('overall')})
+
+        if league != 'MLS':
+            assert len(lg_table_html) == 1
+            lg_table_html = lg_table_html[0]
+            lg_table = pd.read_html(str(lg_table_html))[0]
+            return lg_table
+
+        else:
+            assert len(lg_table_html) == 2
+            east_table = pd.read_html(str(lg_table_html[0]))[0]
+            west_table = pd.read_html(str(lg_table_html[1]))[0]
+            return (east_table, west_table)
+        
+    ####################################################################################################################
+    def scrape_stats(self, year, league, stat_category, normalize=False):
+        """ Scrapes a single stats category
+        
+        Adds team and player ID columns to the stats tables
+        
+        Args
+        ----
+        year : int
+            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
+        league : str
+            League. Look in shared_functions.py for the available leagues for each module.
+        stat_cateogry : str
+            The stat category to scrape.
+        normalize : bool
+            OPTIONAL, default is False. If True, will normalize all stats to Per90.
+        Returns
+        -------
+        : tuple
+            tuple of 3 Pandas DataFrames, (squad_stats, opponent_stats, player_stats).
+        """
+        check_season(year,league,'FBRef')
+        
+        # Verify valid stat category
+        if stat_category not in self.stats_categories.keys():
+            raise Exception(
+                f'"{stat_category}" is not a valid FBRef stats category. '+\
+                f'Must be one of {list(self.stats_categories.keys())}.'
+            )
+        
+        season_url = self.get_season_link(year, league)
+        
+        if league == 'Big 5 combined':
+            # Big 5 combined has separate pages for squad and player stats
+            # Make the URLs to these pages
+            first_half = '/'.join(season_url.split('/')[:-1])
+            second_half = season_url.split('/')[-1]
+            stats_category_url_filler = self.stats_categories[stat_category]['url']
+            players_stats_url = '/'.join([first_half, stats_category_url_filler, 'players', second_half])
+            squads_stats_url  = '/'.join([first_half, stats_category_url_filler, 'squads', second_half])
+            
+            # Get the soups from the 2 pages
+            self.get(players_stats_url)
+            players_soup = BeautifulSoup(self.driver.page_source, 'html.parser')
+            self.get(squads_stats_url)
+            squads_soup = BeautifulSoup(self.driver.page_source, 'html.parser')
+
+            # Press normalize buttons, if requested
+            if normalize:
+                # click all per90 toggles on the SQUAD page first, since it's already loaded
+                per90_toggles = squads_soup.find_all('button', {'id': re.compile('per_match_toggle')})
+                for toggle in per90_toggles:
+                    xpath = xpath_soup(toggle)
+                    button_el = self.driver.find_element(By.XPATH, xpath)
+                    self.driver.execute_script('arguments[0].click()', button_el)
+                # update the soup
+                squads_soup = BeautifulSoup(self.driver.page_source, 'html.parser')
+
+                # Now do PLAYERS page
+                self.get(players_stats_url)
+                per90_toggles = players_soup.find_all('button', {'id': re.compile('per_match_toggle')})
+                for toggle in per90_toggles:
+                    xpath = xpath_soup(toggle)
+                    button_el = self.driver.find_element(By.XPATH, xpath)
+                    self.driver.execute_script('arguments[0].click()', button_el)
+                # update the soup
+                players_soup = BeautifulSoup(self.driver.page_source, 'html.parser')
+
+            # Gather stats table tags
+            squad_stats_tag = squads_soup.find('table', {'id': re.compile('for')})
+            opponent_stats_tag = squads_soup.find('table', {'id': re.compile('against')})
+            player_stats_tag = players_soup.find(
+                'table', 
+                {'id': re.compile(f'stats_{self.stats_categories[stat_category]["html"]}')}
+            )
+
+            # Gather squad and opponent squad IDs
+            # These are 'td' elements for Big 5
+            squad_ids = [
+                tag.find('a')['href'].split('/')[3] 
+                for tag 
+                in squad_stats_tag.find_all('td', {'data-stat': 'team'})
+                if tag and tag.find('a')
+            ]
+            opponent_ids = [
+                tag.find('a')['href'].split('/')[3] 
+                for tag 
+                in opponent_stats_tag.find_all('td', {'data-stat': 'team'})
+                if tag and tag.find('a')
+            ]
+
+        else:
+            # Get URL to stat category
+            old_suffix = season_url.split('/')[-1] # suffix is last element 202X-202X-divider-stats
+            new_suffix = f'{self.stats_categories[stat_category]["url"]}/{old_suffix}'
+            new_url = season_url.replace(old_suffix, new_suffix)
+
+            self.get(new_url) # webdrive to link
+            soup = BeautifulSoup(self.driver.page_source, 'html.parser') # get initial soup
+
+            # Normalize button, if requested
+            if normalize:
+                # click all per90 toggles on the page
+                per90_toggles = soup.find_all('button', {'id': re.compile('per_match_toggle')})
+                for toggle in per90_toggles:
+                    xpath = xpath_soup(toggle)
+                    button_el = self.driver.find_element(By.XPATH, xpath)
+                    self.driver.execute_script('arguments[0].click()', button_el)
+                # update the soup
+                soup = BeautifulSoup(self.driver.page_source, 'html.parser')
+
+            # Gather stats table tags
+            squad_stats_tag = soup.find('table', {'id': re.compile('for')})
+            opponent_stats_tag = soup.find('table', {'id': re.compile('against')})
+            player_stats_tag = soup.find(
+                'table', 
+                {'id': re.compile(f'stats_{self.stats_categories[stat_category]["html"]}')}
+            )
+
+            # Gather squad and opponent squad IDs
+            # These are 'th' elements for all other leagues
+            squad_ids = [
+                tag.find('a')['href'].split('/')[3] 
+                for tag 
+                in squad_stats_tag.find_all('th', {'data-stat': 'team'})[1:]
+                if tag and tag.find('a')
+            ]
+            opponent_ids = [
+                tag.find('a')['href'].split('/')[3] 
+                for tag 
+                in opponent_stats_tag.find_all('th', {'data-stat': 'team'})[1:]
+                if tag and tag.find('a')
+            ]
+            
+        # Get stats dataframes
+        squad_stats = pd.read_html(str(squad_stats_tag))[0] if squad_stats_tag is not None else None
+        opponent_stats = pd.read_html(str(opponent_stats_tag))[0] if opponent_stats_tag is not None else None
+        player_stats = pd.read_html(str(player_stats_tag))[0] if player_stats_tag is not None else None
+
+        # Drop rows that contain duplicated table headers
+        squad_stats = squad_stats[
+            (~squad_stats.loc[:, (slice(None), 'Squad')].isna()) 
+            & (squad_stats.loc[:, (slice(None), 'Squad')] != 'Squad')
+        ].reset_index(drop=True)
+        opponent_stats = opponent_stats[
+            (~opponent_stats.loc[:, (slice(None), 'Squad')].isna()) 
+            & (opponent_stats.loc[:, (slice(None), 'Squad')] != 'Squad')
+        ].reset_index(drop=True)
+        keep_players_mask = (player_stats.loc[:, (slice(None), 'Rk')] != 'Rk').values
+        player_stats = player_stats.loc[keep_players_mask, :].reset_index(drop=True)
+
+        # Add team IDs
+        if squad_stats is not None:
+            squad_stats['Team ID'] = squad_ids
+        if opponent_stats is not None:
+            opponent_stats['Team ID'] = opponent_ids
+        
+        # Add player links and ID's
+        if player_stats is not None:
+            player_links = [
+                'https://fbref.com' + tag.find('a')['href']
+                for tag 
+                in player_stats_tag.find_all('td', {'data-stat': 'player'})
+                if tag and tag.find('a')
+            ]
+            player_stats['Player Link'] = player_links
+            player_stats['Player ID'] = [l.split('/')[-2] for l in player_links]
+        
+        return squad_stats, opponent_stats, player_stats
+    
+    ####################################################################################################################
+    def scrape_all_stats(self, year, league, normalize=False):
+        """ Scrapes all stat categories
+        
+        Runs scrape_stats() for each stats category on dumps the returned tuple of dataframes into a dict.
+        
+        Args
+        ----
+        year : int
+            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
+        league : str
+            League. Look in shared_functions.py for the available leagues for each module.
+        normalize : bool
+            OPTIONAL, default is False. If True, will normalize all stats to Per90.
+        Returns
+        -------
+        : dict
+            Keys are stat category names, values are tuples of 3 dataframes, (squad_stats, opponent_stats, player_stats)
+        """
+        check_season(year,league,'FBRef')
+        
+        return_package = dict()
+        for stat_category in tqdm(self.stats_categories):
+            stats = self.scrape_stats(year, league, stat_category, normalize)
+            return_package[stat_category] = stats
+            
+        return return_package
+
+    ####################################################################################################################
+    def scrape_matches(self, year, league, save=False):
+        """ Scrapes the FBRef standard stats page of the chosen league season.
+            
+        Works by gathering all of the match URL's from the homepage of the chosen league season on FBRef and then \
+        calling scrape_match() on each one.
+
+        Args
+        ----
+        year : int
+            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
+        league : str
+            League. Look in shared_functions.py for the available leagues for each module.
+        save : bool
+            OPTIONAL, default is False. If True, will save the returned DataFrame to a CSV file.
+        Returns
+        -------
+        : Pandas DataFrame
+            If save is False, will return the Pandas DataFrame with the the stats. 
+        filename : str
+            If save is True, will return the filename the CSV was saved to.
+        """
+        check_season(year,league,'FBRef')
+        
+        season = str(year-1)+'-'+str(year)
+        links = self.get_match_links(year,league)
+        
+        matches = pd.DataFrame() # initialize df
+        
+        # scrape match data
+        print('Scraping matches.')
+        time.sleep(1)
+        for link in tqdm(links):
+            try:
+                match = self.scrape_match(link)
+                matches = pd.concat([matches, match], ignore_index=True)
+            except Exception as E:
+                print(f'Failed scraping match {link}')
+                raise E
+            
+        # sort df by match date
+        matches = matches.sort_values(by='Date').reset_index(drop=True)
+        
+        # save to CSV if requested by user
+        if save:
+            filename = f'{season}_{league.replace(" ","_")}_FBRef_matches.csv'
+            matches.to_csv(path_or_buf=filename, index=False)
+            print('Matches dataframe saved to ' + filename)
+            return filename
+        else:
+            return matches
+        
+    ####################################################################################################################
+    def scrape_match(self, link):
+        """ Scrapes an FBRef match page.
+        
+        Args
+        ----
+        link : str
+            URL to the FBRef match page
+        Returns
+        -------
+        : Pandas DataFrame
+            DataFrame containing most parts of the match page if they're available (e.g. formations, lineups, scores, \
+            player stats, etc.). The fields that are available vary by competition and year.
+        """
+        response = self.requests_get(link)
+        soup = BeautifulSoup(response.content, 'html.parser')
+        
+        # Matchweek/stage ==============================================================================================
+        stage_el = list(soup.find('a', {'href': re.compile('-Stats')}, string=True).parents)[0]
+        stage_text = stage_el.getText().split("(")[1].split(")")[0].strip()
+        if "matchweek" in stage_text:
+            stage = int(stage_text.lower().replace("matchweek","").strip())
+        else:
+            stage = stage_text
+
+        # Team names and ids ===========================================================================================
+        team_els = [
+            el.find('a') \
+            for el 
+            in soup.find('div', {'class': 'scorebox'}).find_all('strong') \
+            if el.find('a', href=True) is not None
+        ][:2]
+        home_team_name = team_els[0].getText()
+        home_team_id   = team_els[0]['href'].split('/')[3]
+        away_team_name = team_els[1].getText()
+        away_team_id   = team_els[1]['href'].split('/')[3]
+        
+        # Scores =======================================================================================================
+        scores = soup.find('div', {'class': 'scorebox'}).find_all('div', {'class': 'score'})
+
+        # Formations ===================================================================================================
+        lineup_tags = [tag.find('table') for tag in soup.find_all('div', {'class': 'lineup'})]
+        
+        # Player stats =================================================================================================
+        # Use table ID's to find the appropriate table. More flexible than xpath
+        player_stats = dict()
+        for i, (team, team_id) in enumerate([('Home',home_team_id), ('Away',away_team_id)]):
+
+            summary_tag = soup.find_all('table', {'id': re.compile(f'stats_{team_id}_summary')})
+            assert len(summary_tag) < 2
+            summary_df = pd.read_html(str(summary_tag[0]))[0] if len(summary_tag)==1 else None
+
+            gk_tag = soup.find_all('table', {'id': re.compile(f'keeper_stats_{team_id}')})
+            assert len(gk_tag) < 2
+            gk_df = pd.read_html(str(gk_tag[0]))[0] if len(gk_tag)==1 else None
+
+            passing_tag = soup.find_all('table', {'id': re.compile(f'stats_{team_id}_passing$')})
+            assert len(passing_tag) < 2
+            passing_df = pd.read_html(str(passing_tag[0]))[0] if len(passing_tag)==1 else None
+
+            pass_types_tag = soup.find_all('table', {'id': re.compile(f'stats_{team_id}_passing_types')})
+            assert len(pass_types_tag) < 2
+            pass_types_df = pd.read_html(str(pass_types_tag[0]))[0] if len(pass_types_tag)==1 else None
+
+            defense_tag = soup.find_all('table', {'id': re.compile(f'stats_{team_id}_defense')})
+            assert len(defense_tag) < 2
+            defense_df = pd.read_html(str(defense_tag[0]))[0] if len(defense_tag)==1 else None
+
+            possession_tag = soup.find_all('table', {'id': re.compile(f'stats_{team_id}_possession')})
+            assert len(possession_tag) < 2
+            possession_df = pd.read_html(str(possession_tag[0]))[0] if len(possession_tag)==1 else None
+
+            misc_tag = soup.find_all('table', {'id': re.compile(f'stats_{team_id}_misc')})
+            assert len(misc_tag) < 2
+            misc_df = pd.read_html(str(misc_tag[0]))[0] if len(misc_tag)==1 else None
+            
+            lineup_df = pd.read_html(str(lineup_tags[i]))[0] if len(lineup_tags)!=0 else None
+            
+            # Field player ID's for the stats tables -------------------------------------------------------------------
+            # Note: if a coach gets a yellow/red card, they appear in the player stats tables, in their own row, at the 
+            # bottom.
+            if summary_df is not None:
+                player_ids = list()
+                # Iterate across all els that are player/coach names in the summary stats table
+                for tag in summary_tag[0].find_all('th', {'data-stat':'player', 'scope':'row', 'class':'left'}):
+                    if tag.find('a'):
+                        # if th el has an a subel, it should contain an href link to the player
+                        player_id = tag.find('a')['href'].split('/')[3]
+                    else:
+                        # coaches and the summary row have now a subel (and no player id)
+                        player_id = ''
+                    player_ids.append(player_id)
+                
+                summary_df['Player ID'] = player_ids
+                if passing_df is not None:
+                    passing_df['Player ID'] = player_ids
+                if pass_types_df is not None:
+                    pass_types_df['Player ID'] = player_ids
+                if defense_df is not None:
+                    defense_df['Player ID'] = player_ids
+                if possession_df is not None:
+                    possession_df['Player ID'] = player_ids
+                if misc_df is not None:
+                    misc_df['Player ID'] = player_ids
+
+            # GK ID's --------------------------------------------------------------------------------------------------
+            if gk_df is not None:
+                gk_ids = [
+                    tag.find('a')['href'].split('/')[3]
+                    for tag 
+                    in gk_tag[0].find_all('th', {'data-stat': 'player'})
+                    if tag.find('a')
+                ]
+                
+                gk_df['Player ID'] = gk_ids
+
+            # Build player stats dict ----------------------------------------------------------------------------------
+            # This will be turned into a Series and then put into the match dataframe
+            player_stats[team] = {
+                'Team Sheet': lineup_df,
+                'Summary': summary_df,
+                'GK': gk_df,
+                'Passing': passing_df,
+                'Pass Types': pass_types_df,
+                'Defense': defense_df,
+                'Possession': possession_df,
+                'Misc': misc_df,
+            }
+            
+        # Shots ========================================================================================================
+        both_shots = soup.find_all('table', {'id': 'shots_all'})
+        if len(both_shots) == 1:
+            both_shots = pd.read_html(str(both_shots[0]))[0]
+            both_shots = both_shots[~both_shots.isna().all(axis=1)]
+        else:
+            both_shots = None
+        home_shots = soup.find_all('table', {'id': f'shots_{home_team_id}'})
+        if len(home_shots) == 1:
+            home_shots = pd.read_html(str(home_shots[0]))[0]
+            home_shots = home_shots[~home_shots.isna().all(axis=1)]
+        else:
+            home_shots = None
+        away_shots = soup.find_all('table', {'id': f'shots_{away_team_id}'})
+        if len(away_shots) == 1:
+            away_shots = pd.read_html(str(away_shots[0]))[0]
+            away_shots = away_shots[~away_shots.isna().all(axis=1)]
+        else:
+            away_shots = None
+            
+        # Expected stats flag ==========================================================================================
+        expected = 'Expected' in player_stats['Home']['Summary'].columns.get_level_values(0)
+
+        # Build match series ===========================================================================================
+        match = pd.Series(dtype=object)
+        match['Link'] = link
+        match['Date'] = datetime.strptime(
+            str(soup.find('h1'))
+                .split('<br/>')[0]
+                .split('–')[-1] # not a normal dash
+                .replace('</h1>','')
+                .split('(')[0]
+                .strip(),
+            '%A %B %d, %Y'
+        ).date()
+        match['Stage'] = stage
+        match['Home Team'] = home_team_name
+        match['Away Team'] = away_team_name
+        match['Home Team ID'] = home_team_id
+        match['Away Team ID'] = away_team_id
+        match['Home Formation'] = (
+            player_stats['Home']['Team Sheet'].columns[0].split('(')[-1].replace(')','').strip()
+            if player_stats['Home']['Team Sheet'] is not None else None
+        )
+        match['Away Formation'] = (
+            player_stats['Away']['Team Sheet'].columns[0].split('(')[-1].replace(')','').strip()
+            if player_stats['Away']['Team Sheet'] is not None else None
+        )
+        match['Home Goals'] = int(scores[0].getText()) if scores[0].getText().isdecimal() else None
+        match['Away Goals'] = int(scores[1].getText()) if scores[1].getText().isdecimal() else None
+        match['Home Ast'] = player_stats['Home']['Summary'][('Performance','Ast')].values[-1]
+        match['Away Ast'] = player_stats['Away']['Summary'][('Performance','Ast')].values[-1]
+        match['Home xG'] = player_stats['Home']['Summary'][('Expected','xG')].values[-1] if expected else None
+        match['Away xG'] = player_stats['Away']['Summary'][('Expected','xG')].values[-1] if expected else None
+        match['Home npxG'] = player_stats['Home']['Summary'][('Expected','npxG')].values[-1] if expected else None
+        match['Away npxG'] = player_stats['Away']['Summary'][('Expected','npxG')].values[-1] if expected else None
+        match['Home xAG'] = player_stats['Home']['Summary'][('Expected','xAG')].values[-1] if expected else None
+        match['Away xAG'] = player_stats['Away']['Summary'][('Expected','xAG')].values[-1] if expected else None
+        match['Home Player Stats'] = pd.Series(player_stats['Home']).to_frame().T
+        match['Away Player Stats'] = pd.Series(player_stats['Away']).to_frame().T
+        match['Shots'] = pd.Series({'Both': both_shots, 'Home': home_shots, 'Away': away_shots,}).to_frame().T
+        
+        match = match.to_frame().T # series to dataframe
+        
+        return match
+    
+    ####################################################################################################################
+    def scrape_complete_scouting_reports(self, year, league, goalkeepers=False):
+        """ Scrapes the FBRef scouting reports for all players in the chosen league season.
+
+        Args
+        ----
+        year : int
+            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
+        league : str
+            League. Look in shared_functions.py for the available leagues for each module.
+        goalkeepers : bool
+            OPTIONAL, default is False. If True, will scrape reports for only goalkeepers. If False, will scrape \
+            reports for only outfield players.
+        Returns
+        -------
+        per90 : Pandas DataFrame
+            DataFrame of reports with Per90 stats.
+        percentiles : Pandas DataFrame
+            DataFrame of reports with stats percentiles (versus other players in the top 5 leagues)
+        """
+        # Get the player links
+        if goalkeepers:
+            player_links = self.scrape_stats(year, league, 'goalkeeping')[2]['Player Link'].values
+        else:
+            player_links = self.scrape_stats(year, league, 'standard')[2]['Player Link'].values
+        
+        # initialize dataframes
+        per90_df = pd.DataFrame()
+        percentiles_df = pd.DataFrame()
+        
+        # gather complete reports and append to dataframes
+        for player_link in tqdm(player_links):
+            report, name, pos, mins = self.complete_report_from_player_link(player_link)
+            # skip players without reports
+            if type(report) is int and report==-1:
+                continue
+            
+            # separate per90 and percentiles and add player name, position, and minutes
+            per90 = report['Per 90'].to_frame().T
+            percentile = report['Percentile'].to_frame().T
+            for col, val in [('Name',name), ('Position',pos), ('Minutes',mins)]:
+                per90[col] = val
+                percentile[col] = val
+            
+            # skip players who don't have a complete report or goalkeepers if scraping goalkeeper stats
+            if (type(report) is int) or (not goalkeepers and per90['Position'].values[0]=='Goalkeepers'):
+                continue
+                
+            # append
+            per90_df = pd.concat([per90_df, per90], ignore_index=True)
+            percentiles_df = pd.concat([percentiles_df, percentile], ignore_index=True)
+        
+        return per90_df, percentiles_df
+    
+    ####################################################################################################################
+    def complete_report_from_player_link(self, player_link):
+        """ Scrapes the FBRef scouting reports for a player.
+        
+        Args
+        ----
+        player_link : str
+            URL to an FBRef player page
+        Returns
+        -------
+        cleaned_complete_report : Pandas DataFrame
+            Complete report with a MultiIndex of stats categories and statistics. Columns for per90 and percentile values.
+        player_name : str
+        player_pos : str
+        minutes : int
+        """
+        # return -1 if the player has no scouting report
+        player_link_html = urlopen(player_link).read().decode('utf8')
+        if 'view complete scouting report' not in player_link_html.lower():
+            return -1, -1, -1, -1
+
+        #### Get link to complete report ####
+        soup = BeautifulSoup(requests.get(player_link).content, 'lxml')
+        complete_report_link = soup\
+            .find('div', {'id': 'all_scout'})\
+            .find('div', {'class': 'section_heading_text'})\
+            .find('a', href=True)['href']
+        complete_report_link = 'https://fbref.com' + complete_report_link
+        self.get(complete_report_link)
+
+        #### Load and prelim clean of complete report ####
+        soup = BeautifulSoup(requests.get(complete_report_link).content, 'lxml')
+        complete_report = pd.read_html(str(soup.find('table', {'id': re.compile(f'scout_full')})))[0] # load report
+        complete_report.columns = complete_report.columns.get_level_values(1) # drop top level column name
+        complete_report.dropna(axis=0, inplace=True) # drop nan rows
+        complete_report.reset_index(inplace=True, drop=True) # reset index
+
+        # Row masks
+        header_row_mask = complete_report.eq(complete_report.iloc[:,0], axis=0).all(1) # rows with stats category header names
+
+        #### Create multiindex column names broken down by stats category ####
+        cleaned_complete_report = pd.DataFrame()
+        stats_categories = ('Standard',) + tuple(complete_report[header_row_mask]['Statistic'].values)
+        category_starts = [0,] + list(np.where(header_row_mask)[0]+2) # 2 to skip past category name row and col name row
+        category_ends = list(np.where(header_row_mask)[0]-1) + [complete_report.shape[0]-1]
+        for i in range(len(stats_categories)):
+            temp = complete_report.loc[category_starts[i]:category_ends[i],:]
+            temp.index = pd.MultiIndex.from_product([
+                (stats_categories[i],),
+                temp['Statistic'],
+            ])
+            cleaned_complete_report = pd.concat([cleaned_complete_report,temp])
+        # drop statistic name column, it's in the multiindex now
+        cleaned_complete_report.drop(columns='Statistic', inplace=True)
+        cleaned_complete_report['Per 90'] = cleaned_complete_report['Per 90'].str.rstrip('%').astype('float')
+        cleaned_complete_report['Percentile'] = cleaned_complete_report['Percentile'].astype(int)
+        
+        #### Get player names, positions, and minutes played ####
+        player_name = ' '.join(complete_report_link.split('/')[-1].split('-')[:-2])
+        player_pos = soup.find('div', {'id': 'all_scout'}).find('div', {'class': 'current'}).text.split('vs.')[-1].strip()
+        minutes = int(
+            soup.find('div', {'id': 'all_scout'})\
+                .find('div', {'class': 'footer no_hide_long'})\
+                .find('div')\
+                .text\
+                .split(' minutes')[0]\
+                .split(' ')[-1]
+        )
+
+        return cleaned_complete_report, player_name, player_pos, minutes
```

### Comparing `ScraperFC-2.6.5/ScraperFC/FiveThirtyEight.py` & `ScraperFC-2.7.0/ScraperFC/FiveThirtyEight.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,123 +1,123 @@
-from selenium import webdriver
-from selenium.webdriver.chrome.options import Options
-from selenium.webdriver.common.by import By
-from selenium.webdriver.support.ui import WebDriverWait
-from selenium.webdriver.support import expected_conditions as EC
-from webdriver_manager.chrome import ChromeDriverManager
-import os
-import pandas as pd
-import numpy as np
-from IPython.display import clear_output
-from zipfile import ZipFile
-from ScraperFC.shared_functions import check_season, xpath_soup
-import time
-from bs4 import BeautifulSoup
-
-class FiveThirtyEight:
-    
-    ############################################################################
-    def __init__(self):
-        options = Options()
-        options.headless = True
-        prefs = {"download.default_directory" : os.getcwd()}
-        options.add_experimental_option("prefs",prefs)
-        self.driver = webdriver.Chrome(ChromeDriverManager().install(), options=options)
-        
-    ############################################################################    
-    def close(self):
-        """ Closes and quits the Selenium WebDriver instance.
-        """
-        self.driver.close()
-        self.driver.quit()
-        
-    ############################################################################    
-    def up_season(self, string):
-        """ Increments a string of the season year
-        
-        Args
-        ----
-        string : str
-            String of a calendar year (e.g. "2022")
-        Returns
-        -------
-        : str
-            Incremented calendar year
-        """
-        return str(int(string) + 1)
-        
-    ############################################################################  
-    def scrape_matches(self, year, league, save=False):
-        """ Scrapes matches for the given league season
-
-        Args
-        ----
-        year : int
-            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
-        league : str
-            League. Look in shared_functions.py for the available leagues for each\
-            module.
-        save : bool
-            OPTIONAL, default is False. If True, output will be saved to a CSV file.
-        Returns
-        -------
-        : Pandas DataFrame
-            If save=False, FiveThirtyEight stats for all matches of the given\
-            league season
-        filename : str
-            If save=True, filename of the CSV that the stats were saved to 
-        """
-        # if not check_season(year,league,'FiveThirtyEight'):
-        #     return -1
-        check_season(year,league,'FiveThirtyEight')
-        
-        # Load URL
-        self.driver.get('https://data.fivethirtyeight.com/#soccer-spi')
-        
-        # Wait for data index to be available
-        WebDriverWait(self.driver, 10).until(EC.element_to_be_clickable((By.ID, 'dataIndex')))
-
-        # Click download button
-        soup = BeautifulSoup(self.driver.page_source, 'html.parser')
-        button_xpath = xpath_soup(soup.find('div', {'dataset-name': 'soccer-spi'}))
-        button = self.driver.find_element(By.XPATH, button_xpath)
-        self.driver.execute_script('arguments[0].click();', button)
-                
-        # Wait for download to complete
-        while not os.path.exists('soccer-spi.zip'):
-            time.sleep(1)
-        
-        # Get data table
-        with ZipFile('soccer-spi.zip') as zf:
-            with zf.open('soccer-spi/spi_matches.csv') as f:
-                df = pd.read_csv(f)
-                
-        # Delete downloaded folder
-        os.remove('soccer-spi.zip')
-        
-        # Pick the chosen league
-        if league == "EPL":
-            df = df[df['league'] == 'Barclays Premier League']
-        elif league == "La Liga":
-            df = df[df['league'] == 'Spanish Primera Division']
-        elif league == "Bundesliga":
-            df = df[df['league'] == 'German Bundesliga']
-        elif league == "Serie A":
-            df = df[df['league'] == 'Italy Serie A']
-        elif league == "Ligue 1":
-            df = df[df['league'] == 'French Ligue 1']
-        
-        # Add one to season column
-        df['season'] = df['season'].apply(self.up_season)
-        
-        # Only keep the season requested
-        df = df[df['season']==str(year)].reset_index(drop=True)
-        
-        # Save to CSV if requested by user
-        if save:
-            filename = f'{year}_{league}_FiveThirtyEight_matches.csv'
-            df.to_csv(path_or_buf=filename, index=False)
-            print('Matches dataframe saved to ' + filename)
-            return filename
-        else:
-            return df
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
+from selenium.webdriver.common.by import By
+from selenium.webdriver.support.ui import WebDriverWait
+from selenium.webdriver.support import expected_conditions as EC
+from webdriver_manager.chrome import ChromeDriverManager
+import os
+import pandas as pd
+import numpy as np
+from IPython.display import clear_output
+from zipfile import ZipFile
+from ScraperFC.shared_functions import check_season, xpath_soup
+import time
+from bs4 import BeautifulSoup
+
+class FiveThirtyEight:
+    
+    ############################################################################
+    def __init__(self):
+        options = Options()
+        options.headless = True
+        prefs = {"download.default_directory" : os.getcwd()}
+        options.add_experimental_option("prefs",prefs)
+        self.driver = webdriver.Chrome(ChromeDriverManager().install(), options=options)
+        
+    ############################################################################    
+    def close(self):
+        """ Closes and quits the Selenium WebDriver instance.
+        """
+        self.driver.close()
+        self.driver.quit()
+        
+    ############################################################################    
+    def up_season(self, string):
+        """ Increments a string of the season year
+        
+        Args
+        ----
+        string : str
+            String of a calendar year (e.g. "2022")
+        Returns
+        -------
+        : str
+            Incremented calendar year
+        """
+        return str(int(string) + 1)
+        
+    ############################################################################  
+    def scrape_matches(self, year, league, save=False):
+        """ Scrapes matches for the given league season
+
+        Args
+        ----
+        year : int
+            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
+        league : str
+            League. Look in shared_functions.py for the available leagues for each\
+            module.
+        save : bool
+            OPTIONAL, default is False. If True, output will be saved to a CSV file.
+        Returns
+        -------
+        : Pandas DataFrame
+            If save=False, FiveThirtyEight stats for all matches of the given\
+            league season
+        filename : str
+            If save=True, filename of the CSV that the stats were saved to 
+        """
+        # if not check_season(year,league,'FiveThirtyEight'):
+        #     return -1
+        check_season(year,league,'FiveThirtyEight')
+        
+        # Load URL
+        self.driver.get('https://data.fivethirtyeight.com/#soccer-spi')
+        
+        # Wait for data index to be available
+        WebDriverWait(self.driver, 10).until(EC.element_to_be_clickable((By.ID, 'dataIndex')))
+
+        # Click download button
+        soup = BeautifulSoup(self.driver.page_source, 'html.parser')
+        button_xpath = xpath_soup(soup.find('div', {'dataset-name': 'soccer-spi'}))
+        button = self.driver.find_element(By.XPATH, button_xpath)
+        self.driver.execute_script('arguments[0].click();', button)
+                
+        # Wait for download to complete
+        while not os.path.exists('soccer-spi.zip'):
+            time.sleep(1)
+        
+        # Get data table
+        with ZipFile('soccer-spi.zip') as zf:
+            with zf.open('soccer-spi/spi_matches.csv') as f:
+                df = pd.read_csv(f)
+                
+        # Delete downloaded folder
+        os.remove('soccer-spi.zip')
+        
+        # Pick the chosen league
+        if league == "EPL":
+            df = df[df['league'] == 'Barclays Premier League']
+        elif league == "La Liga":
+            df = df[df['league'] == 'Spanish Primera Division']
+        elif league == "Bundesliga":
+            df = df[df['league'] == 'German Bundesliga']
+        elif league == "Serie A":
+            df = df[df['league'] == 'Italy Serie A']
+        elif league == "Ligue 1":
+            df = df[df['league'] == 'French Ligue 1']
+        
+        # Add one to season column
+        df['season'] = df['season'].apply(self.up_season)
+        
+        # Only keep the season requested
+        df = df[df['season']==str(year)].reset_index(drop=True)
+        
+        # Save to CSV if requested by user
+        if save:
+            filename = f'{year}_{league}_FiveThirtyEight_matches.csv'
+            df.to_csv(path_or_buf=filename, index=False)
+            print('Matches dataframe saved to ' + filename)
+            return filename
+        else:
+            return df
```

### Comparing `ScraperFC-2.6.5/ScraperFC/SofaScore.py` & `ScraperFC-2.7.0/ScraperFC/SofaScore.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,144 +1,144 @@
-from selenium import webdriver
-from selenium.webdriver.chrome.options import Options
-from selenium.webdriver.common.by import By
-from webdriver_manager.chrome import ChromeDriverManager
-from ScraperFC.shared_functions import *
-from IPython.display import clear_output
-import time
-
-class SofaScore:
-    """ NOT IMPLEMENTED
-    """
-
-    ############################################################################
-    def __init__(self):
-        raise NotImplementedError()
-        # options = Options()
-        # # options.headless = True
-        # options.add_argument("window-size=1400,600")
-        # self.driver = webdriver.Chrome(ChromeDriverManager().install(), options=options)
-        # clear_output()
-
-    ############################################################################
-    def close(self):
-        raise NotImplementedError()
-        # """ Closes and quits the Selenium WebDriver instance.
-        # """
-        # self.driver.close()
-        # self.driver.quit()
-
-    ############################################################################
-    def scrape_team_stats(self, year, league, normalize=True):
-        """ NOT IMPLEMENTED Scrape team stats.
-
-        Args
-        ----
-        year : int
-            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
-        league : str
-            League. Look in shared_functions.py for the available leagues for each\
-            module.
-        normalize : bool
-            OPTIONAL, default is False. If True, will normalize all stats to Per90.
-        Returns
-        -------
-        """
-        raise NotImplementedError()
-        # check_season(year, league, "SofaScore")
-        
-        # url = "https://www.sofascore.com/tournament/football/usa/usl-league-one/13362"
-        # self.driver.get(url)
-
-        # # Click button for right season
-        # for el in self.driver.find_elements(By.TAG_NAME, "li"):
-        #     if str(year) in el.get_attribute("outerHTML"):
-        #         button = el
-        #         break
-        # self.driver.execute_script("arguments[0].click()",button)
-        # time.sleep(3)
-
-        # # Get links to the teams in the tables
-        # team_links = list()
-        # for el in self.driver.find_elements(By.TAG_NAME, "a"):
-        #     href = el.get_attribute("href")
-        #     if href and ("team" in href):
-        #         team_links.append(href)
-
-        # # Scrape stats for each team
-        # for team_link in team_links[:1]:
-        #     self.driver.get(team_link) # Go to team's page
-
-        #     # Click to season stats for the chosen season
-        #     buttons = list()
-        #     for el in self.driver.find_elements(By.TAG_NAME, "li"):
-        #         time.sleep(0.1)
-        #         if str(year) in el.get_attribute("outerHTML"):
-        #             buttons.append(el)
-        #     self.driver.execute_script("arguments[0].click()",buttons[1])
-
-        #     matches = None
-        #     team_stats = {
-        #         "Team name": team_link.split("/")[-2].replace("-"," "),
-        #         "Avg. rating": self.driver.find_element(By.XPATH, "/html/body/div[1]/main/div/div[2]/div[1]/div[2]/div/div[4]/div/div[2]/div[2]").text,
-        #         "Matches": matches,
-        #         "GF": None,
-        #         "GA": None,
-        #         "A": None,
-        #         "Goal conversion": None,
-        #         "PK goals": None,
-        #         "FK goals": None,
-        #         "Goals from inside the box": None,
-        #         "Goals from outside the box": None,
-        #         "Left foot goals": None,
-        #         "Right foot goals": None,
-        #         "Headed goals": None,
-        #         "Big chances": round(None*matches),
-        #         "Big chances missed": round(None*matches),
-        #         "Shots": round(None*matches),
-        #         "Shots on target": round(None*matches),
-        #         "Shots off target": round(None*matches),
-        #         "Succ. dribbles": round(None*matches),
-        #         "Corners": round(None*matches),
-        #         "Hit woodwork": None,
-        #         "Counter attacks": None,
-        #         "Avg. possession": None,
-        #         "Acc. passes": round(None*matches),
-        #         "Pass acc.": None,
-        #         "Comp. passes own half": None,
-        #         "Pass acc. own half": None,
-        #         "Comp. passes opp. half": None,
-        #         "Pass acc. opp. half": None,
-        #         "Comp. long balls": None,
-        #         "Long ball acc.": None,
-        #         "Comp. crosses": None,
-        #         "Cross acc.": None,
-        #         "CS": None,
-        #         "Tackles": round(None*matches),
-        #         "Interceptions": round(None*matches),
-        #         "Clearances": round(None*matches),
-        #         "Saves": round(None*matches),
-        #         "Err. leading to shot": None,
-        #         "Err leading to goal": None,
-        #         "PK conceded": None,
-        #         "PK goals conceded": None,
-        #         "Clearances off line": None,
-        #         "Last man tackles": None,
-        #         "Duels won": round(None*matches),
-        #         "Duels win %": None,
-        #         "Ground duels won": round(None*matches),
-        #         "Ground duels win %": None,
-        #         "Aerial duels won": round(None*matches),
-        #         "Aerial duels win %": None,
-        #         "Poss. lost": round(None*matches),
-        #         "Offsides": round(None*matches),
-        #         "Fouls": round(None*matches),
-        #         "YC": round(None*matches),
-        #         "RC": None,
-        #         "Squad size": None
-        #     }
-
-        # if normalize:
-        #     pass
-
-        # return 999
-
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
+from selenium.webdriver.common.by import By
+from webdriver_manager.chrome import ChromeDriverManager
+from ScraperFC.shared_functions import *
+from IPython.display import clear_output
+import time
+
+class SofaScore:
+    """ NOT IMPLEMENTED
+    """
+
+    ############################################################################
+    def __init__(self):
+        raise NotImplementedError()
+        # options = Options()
+        # # options.headless = True
+        # options.add_argument("window-size=1400,600")
+        # self.driver = webdriver.Chrome(ChromeDriverManager().install(), options=options)
+        # clear_output()
+
+    ############################################################################
+    def close(self):
+        raise NotImplementedError()
+        # """ Closes and quits the Selenium WebDriver instance.
+        # """
+        # self.driver.close()
+        # self.driver.quit()
+
+    ############################################################################
+    def scrape_team_stats(self, year, league, normalize=True):
+        """ NOT IMPLEMENTED Scrape team stats.
+
+        Args
+        ----
+        year : int
+            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
+        league : str
+            League. Look in shared_functions.py for the available leagues for each\
+            module.
+        normalize : bool
+            OPTIONAL, default is False. If True, will normalize all stats to Per90.
+        Returns
+        -------
+        """
+        raise NotImplementedError()
+        # check_season(year, league, "SofaScore")
+        
+        # url = "https://www.sofascore.com/tournament/football/usa/usl-league-one/13362"
+        # self.driver.get(url)
+
+        # # Click button for right season
+        # for el in self.driver.find_elements(By.TAG_NAME, "li"):
+        #     if str(year) in el.get_attribute("outerHTML"):
+        #         button = el
+        #         break
+        # self.driver.execute_script("arguments[0].click()",button)
+        # time.sleep(3)
+
+        # # Get links to the teams in the tables
+        # team_links = list()
+        # for el in self.driver.find_elements(By.TAG_NAME, "a"):
+        #     href = el.get_attribute("href")
+        #     if href and ("team" in href):
+        #         team_links.append(href)
+
+        # # Scrape stats for each team
+        # for team_link in team_links[:1]:
+        #     self.driver.get(team_link) # Go to team's page
+
+        #     # Click to season stats for the chosen season
+        #     buttons = list()
+        #     for el in self.driver.find_elements(By.TAG_NAME, "li"):
+        #         time.sleep(0.1)
+        #         if str(year) in el.get_attribute("outerHTML"):
+        #             buttons.append(el)
+        #     self.driver.execute_script("arguments[0].click()",buttons[1])
+
+        #     matches = None
+        #     team_stats = {
+        #         "Team name": team_link.split("/")[-2].replace("-"," "),
+        #         "Avg. rating": self.driver.find_element(By.XPATH, "/html/body/div[1]/main/div/div[2]/div[1]/div[2]/div/div[4]/div/div[2]/div[2]").text,
+        #         "Matches": matches,
+        #         "GF": None,
+        #         "GA": None,
+        #         "A": None,
+        #         "Goal conversion": None,
+        #         "PK goals": None,
+        #         "FK goals": None,
+        #         "Goals from inside the box": None,
+        #         "Goals from outside the box": None,
+        #         "Left foot goals": None,
+        #         "Right foot goals": None,
+        #         "Headed goals": None,
+        #         "Big chances": round(None*matches),
+        #         "Big chances missed": round(None*matches),
+        #         "Shots": round(None*matches),
+        #         "Shots on target": round(None*matches),
+        #         "Shots off target": round(None*matches),
+        #         "Succ. dribbles": round(None*matches),
+        #         "Corners": round(None*matches),
+        #         "Hit woodwork": None,
+        #         "Counter attacks": None,
+        #         "Avg. possession": None,
+        #         "Acc. passes": round(None*matches),
+        #         "Pass acc.": None,
+        #         "Comp. passes own half": None,
+        #         "Pass acc. own half": None,
+        #         "Comp. passes opp. half": None,
+        #         "Pass acc. opp. half": None,
+        #         "Comp. long balls": None,
+        #         "Long ball acc.": None,
+        #         "Comp. crosses": None,
+        #         "Cross acc.": None,
+        #         "CS": None,
+        #         "Tackles": round(None*matches),
+        #         "Interceptions": round(None*matches),
+        #         "Clearances": round(None*matches),
+        #         "Saves": round(None*matches),
+        #         "Err. leading to shot": None,
+        #         "Err leading to goal": None,
+        #         "PK conceded": None,
+        #         "PK goals conceded": None,
+        #         "Clearances off line": None,
+        #         "Last man tackles": None,
+        #         "Duels won": round(None*matches),
+        #         "Duels win %": None,
+        #         "Ground duels won": round(None*matches),
+        #         "Ground duels win %": None,
+        #         "Aerial duels won": round(None*matches),
+        #         "Aerial duels win %": None,
+        #         "Poss. lost": round(None*matches),
+        #         "Offsides": round(None*matches),
+        #         "Fouls": round(None*matches),
+        #         "YC": round(None*matches),
+        #         "RC": None,
+        #         "Squad size": None
+        #     }
+
+        # if normalize:
+        #     pass
+
+        # return 999
+
```

### Comparing `ScraperFC-2.6.5/ScraperFC/Transfermarkt.py` & `ScraperFC-2.7.0/ScraperFC/Transfermarkt.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,280 +1,280 @@
-from selenium import webdriver
-from selenium.webdriver.chrome.options import Options
-from selenium.webdriver.support.ui import WebDriverWait
-from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.common.by import By
-from selenium.common.exceptions import TimeoutException
-from webdriver_manager.chrome import ChromeDriverManager
-from ScraperFC.shared_functions import *
-from tqdm import tqdm
-import requests
-from bs4 import BeautifulSoup
-import pandas as pd
-
-
-class Transfermarkt():
-    
-    ############################################################################
-    def __init__(self):
-        options = Options()
-        prefs = {'profile.managed_default_content_settings.images': 2} # don't load images
-        options.add_experimental_option('prefs', prefs)
-        self.driver = webdriver.Chrome(ChromeDriverManager().install(), options=options) # create driver
-
-        
-    ############################################################################
-    def close(self):
-        """ Closes and quits the Selenium WebDriver instance.
-        """
-        self.driver.close()
-        self.driver.quit()
-        
-        
-    ############################################################################
-    def get_club_links(self, year, league):
-        """ Gathers all Transfermarkt club URL's for the chosen league season.
-        
-        Args
-        ----
-        year : int
-            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
-        league : str
-            League. Look in shared_functions.py for the available leagues for each\
-            module.
-        Returns
-        -------
-        : list
-            List of the club URL's
-        """
-        print("Gathering club links.")
-        check_season(year, league, 'Transfermarkt')
-        
-        competition_links = {
-            'EPL': 'https://www.transfermarkt.us/premier-league/startseite/wettbewerb/GB1',
-            'EFL Championship': 'https://www.transfermarkt.us/championship/startseite/wettbewerb/GB2',
-            'EFL1': 'https://www.transfermarkt.us/league-one/startseite/wettbewerb/GB3',
-            'EFL2': 'https://www.transfermarkt.us/league-two/startseite/wettbewerb/GB4',
-            'Bundesliga': 'https://www.transfermarkt.us/bundesliga/startseite/wettbewerb/L1',
-            '2.Bundesliga': 'https://www.transfermarkt.us/2-bundesliga/startseite/wettbewerb/L2',
-            'Serie A': 'https://www.transfermarkt.us/serie-a/startseite/wettbewerb/IT1',
-            'Serie B': 'https://www.transfermarkt.us/serie-b/startseite/wettbewerb/IT2',
-            'La Liga': 'https://www.transfermarkt.us/laliga/startseite/wettbewerb/ES1',
-            'La Liga 2': 'https://www.transfermarkt.us/laliga2/startseite/wettbewerb/ES2',
-            'Ligue 1': 'https://www.transfermarkt.us/ligue-1/startseite/wettbewerb/FR1',
-            'Ligue 2': 'https://www.transfermarkt.us/ligue-2/startseite/wettbewerb/FR2',
-            'Eredivisie': 'https://www.transfermarkt.us/eredivisie/startseite/wettbewerb/NL1',
-            'Scottish PL': 'https://www.transfermarkt.us/scottish-premiership/startseite/wettbewerb/SC1',
-            'Super Lig': 'https://www.transfermarkt.us/super-lig/startseite/wettbewerb/TR1',
-            'Jupiler Pro League': 'https://www.transfermarkt.us/jupiler-pro-league/startseite/wettbewerb/BE1',
-            'Liga Nos': 'https://www.transfermarkt.us/liga-nos/startseite/wettbewerb/PO1',
-            'Russian Premier League': 'https://www.transfermarkt.us/premier-liga/startseite/wettbewerb/RU1',
-            'Brasileirao': 'https://www.transfermarkt.us/campeonato-brasileiro-serie-a/startseite/wettbewerb/BRA1',
-            'Argentina Liga Profesional': 'https://www.transfermarkt.us/superliga/startseite/wettbewerb/AR1N',
-            'MLS': 'https://www.transfermarkt.us/major-league-soccer/startseite/wettbewerb/MLS1'
-        }
-        
-        # go to the selected year
-        url = '{}/plus/?saison_id={}'.format(competition_links[league], year-1)
-        self.driver.get(url)
-        
-        # get the club links
-        club_links = set()
-        table = self.driver.find_elements(By.CLASS_NAME, 'items')[0]
-        for el in table.find_elements(By.TAG_NAME, 'td'):
-            if 'hauptlink no-border-links' in el.get_attribute('class'):
-                href = el.find_element(By.TAG_NAME, 'a').get_attribute('href')
-                club_links.add(href)
-            
-        return list(club_links)
-    
-    
-    ############################################################################
-    def get_player_links(self, year, league):
-        """ Gathers all Transfermarkt player URL's for the chosen league season.
-        
-        Args
-        ----
-        year : int
-            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
-        league : str
-            League. Look in shared_functions.py for the available leagues for each\
-            module.
-        Returns
-        -------
-        : list
-            List of the player URL's
-        """
-        print("Gathering player links.")
-        check_season(year, league, 'Transfermarkt')
-        
-        player_links = set()
-        club_links = self.get_club_links(year, league)
-        for club_link in tqdm(club_links):
-            self.driver.get(club_link)
-            
-            # get players from the table on the club page
-            table = self.driver.find_elements(By.CLASS_NAME, 'items')[0]
-            for el in table.find_elements(By.CLASS_NAME, 'hauptlink'):
-                try:
-                    subel = WebDriverWait(el, 10).until(EC.element_to_be_clickable((By.TAG_NAME, 'a')))
-                except TimeoutException:
-                    # Ben White f*cked everything up. For some reason, this works
-                    continue
-                href = subel.get_attribute('href')
-                if 'profil' in href:
-                    player_links.add(href)
-                
-        return list(player_links)
-    
-    ############################################################################
-    def get_players(self, year, league):
-        """ Gathers all player info for the chosen league season.
-        
-        Args
-        ----
-        year : int
-            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
-        league : str
-            League. Look in shared_functions.py for the available leagues for each\
-            module.
-        Returns
-        -------
-        : Pandas DataFrame
-            Each row is a player and contains some of the information from their\
-            Transfermarkt player profile.
-        """
-        check_season(year, league, 'Transfermarkt')
-        
-        player_links = self.get_player_links(year, league)
-        df = pd.DataFrame()
-        for player_link in tqdm(player_links):
-            player = TransfermarktPlayer(player_link)
-            new_row = pd.Series(dtype=object)
-            new_row["Name"] = player.name
-            new_row["Value"] = player.value
-            new_row["Value last updated"] = player.value_last_updated
-            new_row["DOB"] = player.dob
-            new_row["Age"] = player.age
-            new_row["Height (m)"] = player.height_meters
-            new_row["Nationality"] = player.nationality
-            new_row["Citizenship"] = player.citizenship
-            new_row["Position"] = player.position
-            if player.other_positions is None:
-                new_row["Other positions"] = None
-            else:
-                new_row["Other positions"] = pd.DataFrame(player.other_positions)
-            new_row["Team"] = player.team
-            new_row["Joined"] = player.joined
-            new_row["Contract expires"] = player.contract_expires
-            new_row["Market value history"] = player.market_value_history
-            new_row["Transfer history"] = player.transfer_history
-            df = df.append(new_row, ignore_index=True)
-        return df
-    
-
-################################################################################
-class TransfermarktPlayer():
-    """ Class to represent Transfermarkt player profiles.
-    
-    Initialize with the URL to a player's Transfermarkt profile page.
-    """
-    
-    def __init__(self, url):
-        self.url = url
-        headers = {
-            'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) '+\
-                'AppleWebKit/537.36 (KHTML, like Gecko) '+\
-                'Chrome/55.0.2883.87 Safari/537.36'
-        }
-        response = requests.get(url, headers=headers)
-        soup = BeautifulSoup(response.content, 'html.parser')
-        
-        #### Name ####
-        data_header_el = soup.find("h1", {"class": "data-header__headline-wrapper"})
-        self.name = data_header_el.getText().split('\n')[-1].strip()
-        
-        #### Value ####
-        try:
-            self.value = soup.find("a", {"class": "data-header__market-value-wrapper"}).text.split(" ")[0]
-            self.value_last_updated = soup.find("a", {"class": "data-header__market-value-wrapper"}).text.split("Last update: ")[-1]
-        except AttributeError:
-            self.value = None
-            self.value_last_updated = None
-            
-        #### DOB and age ####
-        dob_el = soup.find("span", {"itemprop": "birthDate"})
-        self.dob = ' '.join(dob_el.getText().strip().split(' ')[:3])
-        self.age = int(dob_el.getText().strip().split(' ')[-1].replace('(','').replace(')',''))
-        
-        #### Height ####
-        height_el = soup.find("span", {"itemprop": "height"})
-        try:
-            self.height_meters = float(height_el.getText().replace("m", "").replace(",", "."))
-        except AttributeError:
-            self.height_meters = None
-       
-        #### Citizenship ####
-        nationality_el = soup.find("span", {"itemprop": "nationality"})
-        self.nationality = nationality_el.getText().replace("\n","").strip()
-        citizenship_els = soup.find_all("span", {"class": "info-table__content info-table__content--bold"})
-        flag_els = [flag_el for el in citizenship_els\
-            for flag_el in el.find_all("img", {"class": "flaggenrahmen"})]
-        self.citizenship = list(set([el["title"] for el in flag_els]))
-        
-        #### Position ####
-        self.position = soup.find("dd", {"class": "detail-position__position"}).getText()
-        try:
-            self.other_positions = [el.getText() for el in soup.find("div", {"class": "detail-position__position"}).find_all("dd")]
-        except AttributeError:
-            self.other_positions = None
-        
-        #### Team & Contract ####
-        try:
-            self.team = soup.find("span", {"class": "data-header__club"}).find("a")["title"]
-        except TypeError:
-            self.team = "Retired"
-        if self.team in ["Without Club", "Retired"]:
-            self.joined = None
-            self.contract_expires = None
-        else:
-            self.joined = [el.text.split(": ")[-1] \
-                for el in soup.find_all("span", {"class": "data-header__label"}) \
-                if "joined" in el.text.lower()][0]
-            self.contract_expires = [el.text.split(": ")[-1] \
-                for el in soup.find_all("span", {"class": "data-header__label"}) \
-                if "expires" in el.text.lower()][0]
-        
-        #### Market value history ####
-        try:
-            script = [s for s in soup.find_all("script", {"type": "text/javascript"}) \
-                      if "var chart = new Highcharts.Chart" in str(s)][0]
-            values = [int(s.split(",")[0]) for s in str(script).split("y':")[2:-2]]
-            dates = [s.split("datum_mw':")[-1].split(",'x")[0].replace("\\x20"," ").replace("'", "") \
-                     for s in str(script).split("y':")[2:-2]]
-            self.market_value_history = pd.DataFrame({"date": dates, "value": values})
-        except IndexError:
-            self.market_value_history = None
-        
-        #### Transfer History ####
-        rows = soup.find_all("div", {"class": "tm-player-transfer-history-grid"})
-        self.transfer_history = pd.DataFrame(columns=["Season", "Date", "Left", "Joined", "MV", "Fee"])
-        reached_prev_transfers = True # Assume we've reached past transfers
-        for row in rows[1:-1]:
-            fields = [s.strip() for s in row.getText().split("\n\n") if s!=""]
-            if "Upcoming transfer" in fields:
-                # The next row will be a future transfer
-                reached_prev_transfers = False
-            if reached_prev_transfers:
-                new_row = pd.Series({
-                    "Season": fields[0],
-                    "Date": fields[1],
-                    "Left": fields[2],
-                    "Joined": fields[3],
-                    "MV": fields[4],
-                    "Fee": fields[5]
-                })
-                self.transfer_history = self.transfer_history.append(new_row, ignore_index=True)
-            if "Transfer history" in fields:
-                # Now we've reached past transfers
-                reached_prev_transfers = True
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
+from selenium.webdriver.support.ui import WebDriverWait
+from selenium.webdriver.support import expected_conditions as EC
+from selenium.webdriver.common.by import By
+from selenium.common.exceptions import TimeoutException
+from webdriver_manager.chrome import ChromeDriverManager
+from ScraperFC.shared_functions import *
+from tqdm import tqdm
+import requests
+from bs4 import BeautifulSoup
+import pandas as pd
+
+
+class Transfermarkt():
+    
+    ############################################################################
+    def __init__(self):
+        options = Options()
+        prefs = {'profile.managed_default_content_settings.images': 2} # don't load images
+        options.add_experimental_option('prefs', prefs)
+        self.driver = webdriver.Chrome(ChromeDriverManager().install(), options=options) # create driver
+
+        
+    ############################################################################
+    def close(self):
+        """ Closes and quits the Selenium WebDriver instance.
+        """
+        self.driver.close()
+        self.driver.quit()
+        
+        
+    ############################################################################
+    def get_club_links(self, year, league):
+        """ Gathers all Transfermarkt club URL's for the chosen league season.
+        
+        Args
+        ----
+        year : int
+            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
+        league : str
+            League. Look in shared_functions.py for the available leagues for each\
+            module.
+        Returns
+        -------
+        : list
+            List of the club URL's
+        """
+        print("Gathering club links.")
+        check_season(year, league, 'Transfermarkt')
+        
+        competition_links = {
+            'EPL': 'https://www.transfermarkt.us/premier-league/startseite/wettbewerb/GB1',
+            'EFL Championship': 'https://www.transfermarkt.us/championship/startseite/wettbewerb/GB2',
+            'EFL1': 'https://www.transfermarkt.us/league-one/startseite/wettbewerb/GB3',
+            'EFL2': 'https://www.transfermarkt.us/league-two/startseite/wettbewerb/GB4',
+            'Bundesliga': 'https://www.transfermarkt.us/bundesliga/startseite/wettbewerb/L1',
+            '2.Bundesliga': 'https://www.transfermarkt.us/2-bundesliga/startseite/wettbewerb/L2',
+            'Serie A': 'https://www.transfermarkt.us/serie-a/startseite/wettbewerb/IT1',
+            'Serie B': 'https://www.transfermarkt.us/serie-b/startseite/wettbewerb/IT2',
+            'La Liga': 'https://www.transfermarkt.us/laliga/startseite/wettbewerb/ES1',
+            'La Liga 2': 'https://www.transfermarkt.us/laliga2/startseite/wettbewerb/ES2',
+            'Ligue 1': 'https://www.transfermarkt.us/ligue-1/startseite/wettbewerb/FR1',
+            'Ligue 2': 'https://www.transfermarkt.us/ligue-2/startseite/wettbewerb/FR2',
+            'Eredivisie': 'https://www.transfermarkt.us/eredivisie/startseite/wettbewerb/NL1',
+            'Scottish PL': 'https://www.transfermarkt.us/scottish-premiership/startseite/wettbewerb/SC1',
+            'Super Lig': 'https://www.transfermarkt.us/super-lig/startseite/wettbewerb/TR1',
+            'Jupiler Pro League': 'https://www.transfermarkt.us/jupiler-pro-league/startseite/wettbewerb/BE1',
+            'Liga Nos': 'https://www.transfermarkt.us/liga-nos/startseite/wettbewerb/PO1',
+            'Russian Premier League': 'https://www.transfermarkt.us/premier-liga/startseite/wettbewerb/RU1',
+            'Brasileirao': 'https://www.transfermarkt.us/campeonato-brasileiro-serie-a/startseite/wettbewerb/BRA1',
+            'Argentina Liga Profesional': 'https://www.transfermarkt.us/superliga/startseite/wettbewerb/AR1N',
+            'MLS': 'https://www.transfermarkt.us/major-league-soccer/startseite/wettbewerb/MLS1'
+        }
+        
+        # go to the selected year
+        url = '{}/plus/?saison_id={}'.format(competition_links[league], year-1)
+        self.driver.get(url)
+        
+        # get the club links
+        club_links = set()
+        table = self.driver.find_elements(By.CLASS_NAME, 'items')[0]
+        for el in table.find_elements(By.TAG_NAME, 'td'):
+            if 'hauptlink no-border-links' in el.get_attribute('class'):
+                href = el.find_element(By.TAG_NAME, 'a').get_attribute('href')
+                club_links.add(href)
+            
+        return list(club_links)
+    
+    
+    ############################################################################
+    def get_player_links(self, year, league):
+        """ Gathers all Transfermarkt player URL's for the chosen league season.
+        
+        Args
+        ----
+        year : int
+            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
+        league : str
+            League. Look in shared_functions.py for the available leagues for each\
+            module.
+        Returns
+        -------
+        : list
+            List of the player URL's
+        """
+        print("Gathering player links.")
+        check_season(year, league, 'Transfermarkt')
+        
+        player_links = set()
+        club_links = self.get_club_links(year, league)
+        for club_link in tqdm(club_links):
+            self.driver.get(club_link)
+            
+            # get players from the table on the club page
+            table = self.driver.find_elements(By.CLASS_NAME, 'items')[0]
+            for el in table.find_elements(By.CLASS_NAME, 'hauptlink'):
+                try:
+                    subel = WebDriverWait(el, 10).until(EC.element_to_be_clickable((By.TAG_NAME, 'a')))
+                except TimeoutException:
+                    # Ben White f*cked everything up. For some reason, this works
+                    continue
+                href = subel.get_attribute('href')
+                if 'profil' in href:
+                    player_links.add(href)
+                
+        return list(player_links)
+    
+    ############################################################################
+    def get_players(self, year, league):
+        """ Gathers all player info for the chosen league season.
+        
+        Args
+        ----
+        year : int
+            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
+        league : str
+            League. Look in shared_functions.py for the available leagues for each\
+            module.
+        Returns
+        -------
+        : Pandas DataFrame
+            Each row is a player and contains some of the information from their\
+            Transfermarkt player profile.
+        """
+        check_season(year, league, 'Transfermarkt')
+        
+        player_links = self.get_player_links(year, league)
+        df = pd.DataFrame()
+        for player_link in tqdm(player_links):
+            player = TransfermarktPlayer(player_link)
+            new_row = pd.Series(dtype=object)
+            new_row["Name"] = player.name
+            new_row["Value"] = player.value
+            new_row["Value last updated"] = player.value_last_updated
+            new_row["DOB"] = player.dob
+            new_row["Age"] = player.age
+            new_row["Height (m)"] = player.height_meters
+            new_row["Nationality"] = player.nationality
+            new_row["Citizenship"] = player.citizenship
+            new_row["Position"] = player.position
+            if player.other_positions is None:
+                new_row["Other positions"] = None
+            else:
+                new_row["Other positions"] = pd.DataFrame(player.other_positions)
+            new_row["Team"] = player.team
+            new_row["Joined"] = player.joined
+            new_row["Contract expires"] = player.contract_expires
+            new_row["Market value history"] = player.market_value_history
+            new_row["Transfer history"] = player.transfer_history
+            df = df.append(new_row, ignore_index=True)
+        return df
+    
+
+################################################################################
+class TransfermarktPlayer():
+    """ Class to represent Transfermarkt player profiles.
+    
+    Initialize with the URL to a player's Transfermarkt profile page.
+    """
+    
+    def __init__(self, url):
+        self.url = url
+        headers = {
+            'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) '+\
+                'AppleWebKit/537.36 (KHTML, like Gecko) '+\
+                'Chrome/55.0.2883.87 Safari/537.36'
+        }
+        response = requests.get(url, headers=headers)
+        soup = BeautifulSoup(response.content, 'html.parser')
+        
+        #### Name ####
+        data_header_el = soup.find("h1", {"class": "data-header__headline-wrapper"})
+        self.name = data_header_el.getText().split('\n')[-1].strip()
+        
+        #### Value ####
+        try:
+            self.value = soup.find("a", {"class": "data-header__market-value-wrapper"}).text.split(" ")[0]
+            self.value_last_updated = soup.find("a", {"class": "data-header__market-value-wrapper"}).text.split("Last update: ")[-1]
+        except AttributeError:
+            self.value = None
+            self.value_last_updated = None
+            
+        #### DOB and age ####
+        dob_el = soup.find("span", {"itemprop": "birthDate"})
+        self.dob = ' '.join(dob_el.getText().strip().split(' ')[:3])
+        self.age = int(dob_el.getText().strip().split(' ')[-1].replace('(','').replace(')',''))
+        
+        #### Height ####
+        height_el = soup.find("span", {"itemprop": "height"})
+        try:
+            self.height_meters = float(height_el.getText().replace("m", "").replace(",", "."))
+        except AttributeError:
+            self.height_meters = None
+       
+        #### Citizenship ####
+        nationality_el = soup.find("span", {"itemprop": "nationality"})
+        self.nationality = nationality_el.getText().replace("\n","").strip()
+        citizenship_els = soup.find_all("span", {"class": "info-table__content info-table__content--bold"})
+        flag_els = [flag_el for el in citizenship_els\
+            for flag_el in el.find_all("img", {"class": "flaggenrahmen"})]
+        self.citizenship = list(set([el["title"] for el in flag_els]))
+        
+        #### Position ####
+        self.position = soup.find("dd", {"class": "detail-position__position"}).getText()
+        try:
+            self.other_positions = [el.getText() for el in soup.find("div", {"class": "detail-position__position"}).find_all("dd")]
+        except AttributeError:
+            self.other_positions = None
+        
+        #### Team & Contract ####
+        try:
+            self.team = soup.find("span", {"class": "data-header__club"}).find("a")["title"]
+        except TypeError:
+            self.team = "Retired"
+        if self.team in ["Without Club", "Retired"]:
+            self.joined = None
+            self.contract_expires = None
+        else:
+            self.joined = [el.text.split(": ")[-1] \
+                for el in soup.find_all("span", {"class": "data-header__label"}) \
+                if "joined" in el.text.lower()][0]
+            self.contract_expires = [el.text.split(": ")[-1] \
+                for el in soup.find_all("span", {"class": "data-header__label"}) \
+                if "expires" in el.text.lower()][0]
+        
+        #### Market value history ####
+        try:
+            script = [s for s in soup.find_all("script", {"type": "text/javascript"}) \
+                      if "var chart = new Highcharts.Chart" in str(s)][0]
+            values = [int(s.split(",")[0]) for s in str(script).split("y':")[2:-2]]
+            dates = [s.split("datum_mw':")[-1].split(",'x")[0].replace("\\x20"," ").replace("'", "") \
+                     for s in str(script).split("y':")[2:-2]]
+            self.market_value_history = pd.DataFrame({"date": dates, "value": values})
+        except IndexError:
+            self.market_value_history = None
+        
+        #### Transfer History ####
+        rows = soup.find_all("div", {"class": "tm-player-transfer-history-grid"})
+        self.transfer_history = pd.DataFrame(columns=["Season", "Date", "Left", "Joined", "MV", "Fee"])
+        reached_prev_transfers = True # Assume we've reached past transfers
+        for row in rows[1:-1]:
+            fields = [s.strip() for s in row.getText().split("\n\n") if s!=""]
+            if "Upcoming transfer" in fields:
+                # The next row will be a future transfer
+                reached_prev_transfers = False
+            if reached_prev_transfers:
+                new_row = pd.Series({
+                    "Season": fields[0],
+                    "Date": fields[1],
+                    "Left": fields[2],
+                    "Joined": fields[3],
+                    "MV": fields[4],
+                    "Fee": fields[5]
+                })
+                self.transfer_history = self.transfer_history.append(new_row, ignore_index=True)
+            if "Transfer history" in fields:
+                # Now we've reached past transfers
+                reached_prev_transfers = True
```

### Comparing `ScraperFC-2.6.5/ScraperFC/Understat.py` & `ScraperFC-2.7.0/ScraperFC/Understat.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,1021 +1,1021 @@
-import datetime
-import json
-import numpy as np
-import pandas as pd
-from ScraperFC.shared_functions import check_season
-from selenium import webdriver
-from selenium.webdriver.chrome.options import Options
-from selenium.webdriver.common.by import By
-from selenium.common.exceptions import NoSuchElementException
-from webdriver_manager.chrome import ChromeDriverManager
-from tqdm.auto import tqdm
-import requests
-from bs4 import BeautifulSoup
-import time
-
-
-class Understat:
-    
-    ####################################################################################################################
-    def __init__(self):
-        options = Options()
-        options.headless = True
-        options.add_argument("window-size=1400,600")
-        prefs = {'profile.managed_default_content_settings.images': 2} # don't load images
-        options.add_experimental_option('prefs', prefs)
-        self.driver = webdriver.Chrome(ChromeDriverManager().install(), options=options)
-        
-        
-    ####################################################################################################################
-    def close(self):
-        """ Closes and quits the Selenium WebDriver instance.
-        """
-        self.driver.close()
-        self.driver.quit()
-        
-        
-    ####################################################################################################################
-    def get_season_link(self, year, league):
-        """ Gets URL of the chosen league season.
-
-        Args
-        ----
-        year : int
-            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
-        league : str
-            League. Look in shared_functions.py for the available leagues for\
-            each module.
-
-        Returns
-        -------
-        : str
-            URL to the Understat page of the chosen league season.
-        """
-        lg = league.replace(" ","_")
-        url = f"https://understat.com/league/{lg}/{str(year-1)}"
-        return url
-        
-        
-    ####################################################################################################################
-    def get_match_links(self, year, league):
-        """ Gets all of the match links for the chosen league season
-
-        Args
-        ----
-        year : int
-            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
-        league : str
-            League. Look in shared_functions.py for the available leagues for\
-            each module.
-
-        Returns
-        -------
-        : list
-            List of match links of the chosen league season
-        """
-        check_season(year,league,'Understat')
-         
-        base_url = "https://understat.com/"
-        lg = league.replace(" ","_")
-        url = base_url+"league/"+lg+"/"+str(year-1)
-        self.driver.get(url)
-        
-        # Gather the links by hitting the "prev week" button until it's disabled
-        links = set()
-        btn = self.driver.find_element(By.CLASS_NAME, "calendar-prev")
-
-        while "disabled" not in btn.get_attribute("outerHTML"):
-            for el in self.driver.find_elements(By.CLASS_NAME, "match-info"):
-                links.add(el.get_attribute("href"))
-            btn.click()
-            
-        # One final collection for first week of season
-        for el in self.driver.find_elements(By.CLASS_NAME, "match-info"):
-            links.add(el.get_attribute("href"))
-                
-        # Remove Nones from the list of links 
-        links = np.array(list(links))
-        links = links[links!=None]
-
-        return list(links)
-    
-    ####################################################################################################################
-    def get_team_links(self, year, league):
-        """ Gets all of the team links for the chosen league season
-
-        Args
-        ----
-        year : int
-            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
-        league : str
-            League. Look in shared_functions.py for the available leagues for\
-            each module.
-
-        Returns
-        -------
-        : list
-            List of team URL's from the chosen season.
-        """
-        team_links = set()
-        self.driver.get(self.get_season_link(year, league))
-        for el in self.driver.find_elements(By.TAG_NAME, 'a'):
-            href = el.get_attribute('href')
-            if href and 'team' in href:
-                team_links.add(href)
-        return list(team_links)
-    
-    
-    ####################################################################################################################
-    def remove_diff(self, string):
-        """ Removes the plus/minus from some stats like xG.
-
-        Args
-        ----
-        string : str
-            The string to remove the difference from
-
-        Returns
-        -------
-        : str
-            String passed in as arg with the difference removed
-        """
-        string = string.split('-')[0]
-        return float(string.split('+')[0])
-    
-    
-    ####################################################################################################################
-    def unhide_stats(self, columns):
-        """ Understat doesn't display all stats by default. 
-        
-        This functions uses the stats currently shown in the table columns to\
-        unhide stats that aren't being displayed.
-
-        Args
-        ----
-        columns : Pandas DataFrame.columns
-            The columns currently shown in the table being scraped
-
-        Returns
-        -------
-        None
-        """
-        # Show the options popup
-        self.driver.find_elements(By.CLASS_NAME, "options-button")[0].click()
-        
-        # Iterate across all stats and show the ones that aren't in columns
-        for el in self.driver.find_elements(By.CLASS_NAME, "table-options-row"):
-            stat_name = el.find_element(By.CLASS_NAME, "row-title").text
-            if (stat_name not in columns) and (stat_name != ""):
-                el.find_element(By.CLASS_NAME, "row-display").click()
-
-        # click the apply button
-        self.driver.find_elements(By.CLASS_NAME, "button-apply")[0].click()
-        
-        return
-        
-        
-    ####################################################################################################################
-    def scrape_match(self, link):
-        """ Scrapes a single match from Understat.
-
-        Args
-        ----
-        link : str
-            URL to the match
-
-        Returns
-        -------
-        match : Pandas DataFrame
-            The match stats
-        """
-        # self.driver.get(link)
-        # soup = BeautifulSoup(self.driver.page_source, 'html.parser')
-        soup = BeautifulSoup(requests.get(link).content, 'html.parser')
-
-        # Match ID and date ============================================================================================
-        match_id = link.split('/')[-1]
-        date = soup.find('div', {'class': 'page-wrapper'}).find_all('li')[-1].text
-        date = datetime.datetime.strptime(date,'%b %d %Y').date()
-
-        # Shots data
-        shots_script = soup.find('div', {'class':'scheme-block', 'data-scheme':'chart'}).parent.find('script').text
-        shots_data = shots_script.split('JSON.parse(\'')[1].split('\')')[0]
-        shots_data = shots_data.encode('unicode_escape').replace(b'\\\\',b'\\').decode('unicode-escape')
-        shots_data = json.loads(shots_data)
-        shots_home_df = pd.json_normalize(shots_data['h'])
-        shots_away_df = pd.json_normalize(shots_data['a'])
-        all_shots_df = pd.concat([shots_home_df, shots_away_df], axis=0, ignore_index=True)
-        all_shots_df['minute'] = all_shots_df['minute'].astype(int)
-        all_shots_df = all_shots_df.sort_values('minute').reset_index(drop=True)
-
-        # Team stats table =============================================================================================
-        stats_scheme_block = soup.find_all('div', {'data-scheme':'stats'})
-        assert len(stats_scheme_block) == 1
-        stats_scheme_block = stats_scheme_block[0]
-        # Team Names
-        home_team, away_team = [
-            x.text for x in 
-            stats_scheme_block.find('div', {'class':'progress-bar teams-titles'}).find_all('div', {'class': 'progress-value'})
-        ]
-        # Chances
-        chances_bar = stats_scheme_block.find_all('div', {'class':'progress-bar'})[1]
-        home_chance = float(chances_bar.find('div', {'class':'progress-home'})['title'].replace('%',''))
-        draw_chance = float(chances_bar.find('div', {'class':'progress-draw'})['title'].replace('%',''))
-        away_chance = float(chances_bar.find('div', {'class':'progress-away'})['title'].replace('%',''))
-        # Goals
-        goals_bar = stats_scheme_block.find_all('div', {'class':'progress-bar'})[2]
-        home_goals, away_goals = [float(x.text) for x in goals_bar.find_all('div', {'class':'progress-value'})]
-        # xG
-        xg_bar = stats_scheme_block.find_all('div', {'class':'progress-bar'})[3]
-        home_xg, away_xg = [float(x.text) for x in xg_bar.find_all('div', {'class':'progress-value'})]
-        # Shots
-        shots_bar = stats_scheme_block.find_all('div', {'class':'progress-bar'})[4]
-        home_shots, away_shots = [float(x.text) for x in shots_bar.find_all('div', {'class':'progress-value'})]
-        # Shots on Target
-        sot_bar = stats_scheme_block.find_all('div', {'class':'progress-bar'})[5]
-        home_sot, away_sot = [float(x.text) for x in sot_bar.find_all('div', {'class':'progress-value'})]
-        # DEEP
-        deep_bar = stats_scheme_block.find_all('div', {'class':'progress-bar'})[6]
-        home_deep, away_deep = [float(x.text) for x in deep_bar.find_all('div', {'class':'progress-value'})]
-        # PPDA
-        ppda_bar = stats_scheme_block.find_all('div', {'class':'progress-bar'})[7]
-        home_ppda, away_ppda = [float(x.text) for x in ppda_bar.find_all('div', {'class':'progress-value'})]
-        # xPTS
-        xpts_bar = stats_scheme_block.find_all('div', {'class':'progress-bar'})[8]
-        home_xpts, away_xpts = [float(x.text) for x in xpts_bar.find_all('div', {'class':'progress-value'})]
-
-        # Player stats tables ==========================================================================================
-        players_script = soup.find('div', {'id':'match-rosters'}).parent.find('script').text
-        players_data = players_script.split('JSON.parse(\'')[1].split('\')')[0]
-        players_data = players_data.encode('unicode_escape').replace(b'\\\\',b'\\').decode('unicode-escape')
-        players_data = json.loads(players_data)
-        players_home_df = pd.json_normalize(players_data['h'].values())
-        players_away_df = pd.json_normalize(players_data['a'].values())
-
-        # Build match df ===============================================================================================
-        match = pd.Series(dtype=float)
-        match['id'] = match_id
-        match['date'] = date
-        match['shots'] = all_shots_df
-        match['home team'] = home_team
-        match['away team'] = away_team
-        match['home win proba'] = home_chance
-        match['draw proba'] = draw_chance
-        match['away win proba'] = away_chance
-        match['home goals'] = home_goals
-        match['away goals'] = away_goals
-        match['home xG'] = home_xg
-        match['away xG'] = away_xg
-        match['home shots'] = home_shots
-        match['away shots'] = away_shots
-        match['home SoT'] = home_sot
-        match['away SoT'] = away_sot
-        match['home DEEP'] = home_deep
-        match['away DEEP'] = away_deep
-        match['home PPDA'] = home_ppda
-        match['away PPDA'] = away_ppda
-        match['home xPTS'] = home_xpts
-        match['away xPTS'] = away_xpts
-        match['home player stats'] = players_home_df
-        match['away player stats'] = players_away_df
-        match = match.to_frame().T
-
-        return match
-        
-    ####################################################################################################################    
-    def scrape_matches(self, year, league, save=False):
-        """ Scrapes all of the matches from the chosen league season. 
-        
-        Gathers all match links from the chosen league season and then call\
-            scrape_match() on each one.
-
-        Args
-        ----
-        year : int
-            Calendar year that the season ends in (e.g. 2023 for the 2022/23\
-            season)
-        league : str
-            League. Look in shared_functions.py for the available leagues for\
-            each module.
-        save : bool
-            OPTIONAL, default False. If True, saves the DataFrame of match stats\
-            to a CSV.
-
-        Returns
-        -------
-        matches : Pandas DataFrame
-            If save=False
-        filename : str
-            If save=True, the filename the DataFrame was saved to
-        """
-        check_season(year,league,'Understat')
-        
-        season = str(year-1)+'-'+str(year)
-        links = self.get_match_links(year, league)
-        matches = pd.DataFrame()
-        
-        for link in tqdm(links):
-            match   = self.scrape_match(link)
-            matches = pd.concat([matches, match], ignore_index=True, axis=0)
-            time.sleep(2)
-        
-        # save to CSV if requested by user
-        if save:
-            filename = f'{season}_{league}_Understat_matches.csv'
-            matches.to_csv(path_or_buf=filename, index=False)
-            print('Matches dataframe saved to ' + filename)
-            return filename
-        else:
-            return matches
-        
-        
-    ####################################################################################################################
-    def scrape_league_table(self, year, league, normalize=False):
-        """ Scrapes the league table for the chosen league season.
-
-        Args
-        ----
-        year : int
-            Calendar year that the season ends in (e.g. 2023 for the 2022/23\
-            season)
-        league : str
-            League. Look in shared_functions.py for the available leagues for\
-            each module.
-        normalize : bool 
-            OPTIONAL, default False. If True, normalizes stats to per90
-
-        Returns
-        -------
-        : Pandas DataFrame
-            The league table of the chosen league season.
-        """
-        check_season(year,league,'Understat')
-        
-        url = self.get_season_link(year, league) # link to the selected league/season
-        self.driver.get(url)
-        
-        # Show all of the stats 
-        # Get column names currently show in the table
-        table = self.driver.find_elements(By.TAG_NAME, "table")[0].get_attribute("outerHTML")
-        columns = pd.read_html(table)[0].columns
-        self.unhide_stats(columns)
-
-        # dataframe 
-        table = self.driver.find_elements(By.TAG_NAME, "table")[0].get_attribute("outerHTML")
-        df = pd.read_html(table)[0]
-        
-        # remove performance differential text from some columns
-        for i in range(df.shape[0]):
-            df.loc[i,"xG"] = self.remove_diff(df.loc[i,"xG"])
-            df.loc[i,"xGA"] = self.remove_diff(df.loc[i,"xGA"])
-            df.loc[i,"xPTS"] = self.remove_diff(df.loc[i,"xPTS"])
-            
-        if normalize:
-            df.iloc[:,3:14] = df.iloc[:,3:14].divide(df["M"], axis="rows")
-            df.iloc[:,16:] = df.iloc[:,16:].divide(df["M"], axis="rows")
-        
-        self.close()
-        self.__init__()
-        return df
-    
-    
-    ####################################################################################################################
-    def scrape_home_away_tables(self, year, league, normalize=False):
-        """ Scrapes the home and away league tables for the chosen league season.
-
-        Args
-        ----
-        year : int
-            Calendar year that the season ends in (e.g. 2023 for the 2022/23\
-            season)
-        league : str
-            League. Look in shared_functions.py for the available leagues for\
-            each module.
-        normalize : bool 
-            OPTIONAL, default False. If True, normalizes stats to per90
-
-        Returns
-        -------
-        home : Pandas DataFrame
-            Home league table
-        away : Pandas DataFrame
-            Away league table
-        """
-        check_season(year,league,'Understat')
-        
-        url = self.get_season_link(year, league) # link to the selected league/season
-        self.driver.get(url)
-
-        # Show all of the stats
-        # Get columns that are already shown
-        labels = self.driver.find_elements(By.TAG_NAME, "label")
-        [el for el in labels if el.text=='home'][0].click()
-        table = self.driver.find_elements(By.TAG_NAME, "table")[0].get_attribute('outerHTML')
-        columns = pd.read_html(table)[0].columns 
-        self.unhide_stats(columns)
-        
-        # Home Table
-        labels = self.driver.find_elements(By.TAG_NAME, "label")
-        [el for el in labels if el.text=='home'][0].click()
-        table = self.driver.find_elements(By.TAG_NAME, "table")[0].get_attribute('outerHTML')
-        home = pd.read_html(table)[0]
-        
-        
-        # Away Table
-        [el for el in labels if el.text=='away'][0].click()
-        table = self.driver.find_elements(By.TAG_NAME, "table")[0].get_attribute('outerHTML')
-        away = pd.read_html(table)[0]
-        
-        # remove differentials from some columns
-        for i in range(home.shape[0]):
-            home.loc[i,"xG"] = self.remove_diff(home.loc[i,"xG"])
-            home.loc[i,"xGA"] = self.remove_diff(home.loc[i,"xGA"])
-            home.loc[i,"xPTS"] = self.remove_diff(home.loc[i,"xPTS"])
-            away.loc[i,"xG"] = self.remove_diff(away.loc[i,"xG"])
-            away.loc[i,"xGA"] = self.remove_diff(away.loc[i,"xGA"])
-            away.loc[i,"xPTS"] = self.remove_diff(away.loc[i,"xPTS"])
-        
-        if normalize:
-            home.iloc[:,3:14] = home.iloc[:,3:14].divide(home["M"], axis="rows")
-            home.iloc[:,16:] = home.iloc[:,16:].divide(home["M"], axis="rows")
-            away.iloc[:,3:14] = away.iloc[:,3:14].divide(away["M"], axis="rows")
-            away.iloc[:,16:] = away.iloc[:,16:].divide(away["M"], axis="rows")
-        
-        self.close()
-        self.__init__()
-        return home, away
-    
-    
-    ####################################################################################################################
-    def scrape_situations(self, year, league):
-        """ Scrapes the situations leading to shots for each team in the chosen\
-            league season.
-
-        Args
-        ----
-        year : int
-            Calendar year that the season ends in (e.g. 2023 for the 2022/23\
-            season)
-        league : str
-            League. Look in shared_functions.py for the available leagues for\
-            each module.
-
-        Returns
-        -------
-        : Pandas DataFrame
-            DataFrame containing the situations
-        """
-        check_season(year,league,'Understat')
-        
-        # Get links for teams in league that season
-        team_links = self.get_team_links(year, league)
-                
-        mi = pd.MultiIndex.from_product(
-            [["Open play", "From corner", "Set piece", "Direct FK", "Penalty"],
-             ["Sh", "G", "ShA", "GA", "xG", "xGA", "xGD", "xG/Sh", "xGA/Sh"]]
-        )
-        mi = mi.insert(0, ("Team names", "Team"))
-        situations = pd.DataFrame()#columns=mi)
-        
-        for link in team_links:
-            
-            team_name = link.split("/")[-2]
-            self.driver.get(link)
-            table = self.driver.find_elements(By.TAG_NAME, "table")[0].get_attribute("outerHTML")
-            df = pd.read_html(table)[0]
-            
-            for i in range(df.shape[0]):
-                # remove performance differential text from some columns
-                df.loc[i,"xG"] = self.remove_diff(df.loc[i,"xG"])
-                df.loc[i,"xGA"] = self.remove_diff(df.loc[i,"xGA"])
-            
-            # reformat df to fit into a row
-            df.drop(columns=["№","Situation"], inplace=True)
-            row = df.to_numpy()
-            row = np.insert(row, 0, team_name) # insert team name
-            
-            # append row
-            situations = situations.append(
-                pd.DataFrame(row.reshape(1,-1)),#, columns=situations.columns),
-                ignore_index=True
-            )
-        
-        situations.columns = mi
-        self.close()
-        self.__init__()
-        return situations
-    
-    
-    ####################################################################################################################
-    def scrape_formations(self, year, league):
-        """ Scrapes the stats for each team in the year and league, broken down\
-            by formation used by the team.
-
-        Args
-        ----
-        year : int
-            Calendar year that the season ends in (e.g. 2023 for the 2022/23\
-            season)
-        league : str
-            League. Look in shared_functions.py for the available leagues for\
-            each module.
-
-        Returns
-        -------
-        : dict
-            Keys are each team. Values are more dicts with keys for each formation\
-            and values are stats for each formation.
-        """
-        check_season(year,league,'Understat')
-        
-        # Get links for teams in league that season
-        team_links = self.get_team_links(year, league)
-        
-        formations = dict()
-        
-        for link in team_links:
-            
-            # Get team name to add to formations
-            team_name = link.split("/")[-2]
-            if team_name not in formations.keys():
-                formations[team_name] = dict()
-                
-            # Got to team's link, click formations, and get table of formations used
-            self.driver.get(link)
-            self.driver.find_element(
-                By.XPATH, 
-                "/html/body/div[1]/div[3]/div[3]/div/div[1]/div/label[2]"
-            ).click()
-            
-            table = self.driver.find_elements(By.TAG_NAME, "table")[0].get_attribute("outerHTML")
-            df = pd.read_html(table)[0]
-            df.drop(columns=["№"], inplace=True)
-            
-            # Remove performance differential text from some columns
-            for i in range(df.shape[0]):
-                df.loc[i,"xG"] = self.remove_diff(df.loc[i,"xG"])
-                df.loc[i,"xGA"] = self.remove_diff(df.loc[i,"xGA"])
-                
-                formation = df.loc[i,"Formation"]
-                
-                if formation not in formations[team_name].keys():
-                    formations[team_name][formation] = df.iloc[i,:].drop(columns=["№","Formation"])                
-                
-        self.close()
-        self.__init__()
-        return formations
-    
-    
-    ####################################################################################################################
-    def scrape_game_states(self, year, league):
-        """ Scrapes the game states for each team in the year and league
-
-        Args
-        ----
-        year : int
-            Calendar year that the season ends in (e.g. 2023 for the 2022/23\
-            season)
-        league : str
-            League. Look in shared_functions.py for the available leagues for\
-            each module.
-
-        Returns
-        -------
-        : Pandas DataFrame
-            DataFrame containing the game states
-        """
-        check_season(year,league,'Understat')
-        
-        # Get links for teams in league that season
-        team_links = self.get_team_links(year, league)
-                
-        mi = pd.MultiIndex.from_product(
-            [["Goal diff 0", "Goal diff -1", "Goal diff +1", "Goal diff < -1", "Goal diff > +1"],
-             ["Min", "Sh", "G", "ShA", "GA", "xG", "xGA", "xGD", "xG90", "xGA90"]]
-        )
-        mi = mi.insert(0, ("Team names", "Team"))
-        game_states = pd.DataFrame()#columns=mi)
-        
-        for link in team_links:
-            
-            team_name = link.split("/")[-2]
-            self.driver.get(link)
-            self.driver.find_element(
-                By.XPATH, 
-                "/html/body/div[1]/div[3]/div[3]/div/div[1]/div/label[3]"
-            ).click()
-            table = self.driver.find_elements(By.TAG_NAME, "table")[0].get_attribute("outerHTML")
-            df = pd.read_html(table)[0]
-            df.drop(columns=["№"], inplace=True)
-            
-            row = {
-                "Goal diff 0": None,
-                "Goal diff -1": None,
-                "Goal diff +1": None,
-                "Goal diff < -1": None,
-                "Goal diff > +1": None
-            }
-            for i in range(df.shape[0]):
-                # remove performance differential text from some columns
-                df.loc[i,"xG"] = self.remove_diff(df.loc[i,"xG"])
-                df.loc[i,"xGA"] = self.remove_diff(df.loc[i,"xGA"])
-                
-                game_state = df.loc[i,"Game state"]
-                row[game_state] = df.loc[i,:].drop(labels=["Game state"])
-                
-            row_array = []
-            for key in row.keys():
-                row_array.append( row[key].to_numpy() )
-            row_array = np.array(row_array)
-            row_array = np.insert(row_array, 0, team_name) # insert team name
-            
-            # append row
-            game_states = game_states.append(
-                pd.DataFrame(row_array.reshape(1,-1)),#, columns=game_states.columns),
-                ignore_index=True
-            )
-            
-        game_states.columns = mi
-        self.close()
-        self.__init__()
-        return game_states
-    
-    
-    ####################################################################################################################
-    def scrape_timing(self, year, league):
-        """ Scrapes the timing of goals for each team in the year and league
-
-        Args
-        ----
-        year : int
-            Calendar year that the season ends in (e.g. 2023 for the 2022/23\
-            season)
-        league : str
-            League. Look in shared_functions.py for the available leagues for\
-            each module.
-
-        Returns
-        -------
-        : Pandas DataFrame
-            DataFrame containing the timing stats
-        """
-        check_season(year,league,'Understat')
-        
-        # Get links for teams in league that season
-        team_links = self.get_team_links(year, league)
-
-        mi = pd.MultiIndex.from_product(
-            [["1-15", "16-30", "31-45", "46-60", "61-75", "76+"],
-             ["Sh", "G", "ShA", "GA", "xG", "xGA", "xGD", "xG/Sh", "xGA/Sh"]]
-        )
-        mi = mi.insert(0, ("Team names", "Team"))
-        timing_df = pd.DataFrame()#columns=mi)
-
-        for link in team_links:
-            
-            team_name = link.split("/")[-2]
-            self.driver.get(link)
-            self.driver.find_element(
-                By.XPATH, 
-                "/html/body/div[1]/div[3]/div[3]/div/div[1]/div/label[4]"
-            ).click()
-            table = self.driver.find_elements(By.TAG_NAME, "table")[0].get_attribute("outerHTML")
-            df = pd.read_html(table)[0]
-            df.drop(columns=["№"], inplace=True)
-
-            row = {
-                "1-15": None,
-                "16-30": None,
-                "31-45": None,
-                "46-60": None,
-                "61-75": None,
-                "76+": None
-            }
-            for i in range(df.shape[0]):
-                # remove performance differential text from some columns
-                df.loc[i,"xG"] = self.remove_diff(df.loc[i,"xG"])
-                df.loc[i,"xGA"] = self.remove_diff(df.loc[i,"xGA"])
-
-                timing = df.loc[i, "Timing"]
-                row[timing] = df.loc[i,:].drop(labels=["Timing"])
-
-            row_array = []
-            for key in row.keys():
-                row_array.append(row[key].to_numpy())
-            row_array = np.array(row_array)
-            row_array = np.insert(row_array, 0, team_name) # insert team name
-
-            # append row
-            timing_df = timing_df.append(
-                pd.DataFrame(row_array.reshape(1,-1)),#, columns=timing_df.columns),
-                ignore_index=True
-            )
-            
-        timing_df.columns = mi
-        self.close()
-        self.__init__()
-        return timing_df
-    
-    
-    ####################################################################################################################
-    def scrape_shot_zones(self, year, league):
-        """ Scrapes the shot zones for each team in the year and league
-
-        Args
-        ----
-        year : int
-            Calendar year that the season ends in (e.g. 2023 for the 2022/23\
-            season)
-        league : str
-            League. Look in shared_functions.py for the available leagues for\
-            each module.
-
-        Returns
-        -------
-        : Pandas DataFrame
-            DataFrame containing the shot zones data
-        """
-        check_season(year,league,'Understat')
-        
-        # Get links for teams in league that season
-        team_links = self.get_team_links(year, league)
-
-        mi = pd.MultiIndex.from_product(
-            [["Own goals", "Out of box", "Penalty area", "Six-yard box"],
-             ["Sh", "G", "ShA", "GA", "xG", "xGA", "xGD", "xG/Sh", "xGA/Sh"]]
-        )
-        mi = mi.insert(0, ("Team names", "Team"))
-        shot_zones_df = pd.DataFrame()#columns=mi)
-
-        for link in team_links:
-            
-            team_name = link.split("/")[-2]
-            self.driver.get(link)
-            self.driver.find_element(
-                By.XPATH, 
-                "/html/body/div[1]/div[3]/div[3]/div/div[1]/div/label[5]"
-            ).click()
-            table = self.driver.find_elements(By.TAG_NAME, "table")[0].get_attribute("outerHTML")
-            df = pd.read_html(table)[0]
-            df.drop(columns=["№"], inplace=True)
-
-            row = {
-                "Own goals": None,
-                "Out of box": None,
-                "Penalty area": None,
-                "Six-yard box": None
-            }
-            for i in range(df.shape[0]):
-                # remove performance differential text from some columns
-                df.loc[i,"xG"] = self.remove_diff(df.loc[i,"xG"])
-                df.loc[i,"xGA"] = self.remove_diff(df.loc[i,"xGA"])
-
-                zone = df.loc[i, "Shot zones"]
-                row[zone] = df.loc[i,:].drop(labels=["Shot zones"])
-
-            row_array = []
-            for key in row.keys():
-                if row[key] is None:
-                    row[key] = pd.Series(np.zeros((9)))
-                row_array.append(row[key].to_numpy())
-            row_array = np.array(row_array)
-            row_array = np.insert(row_array, 0, team_name) # insert team name
-
-            # append row
-            shot_zones_df = shot_zones_df.append(
-                pd.DataFrame(row_array.reshape(1,-1)),#, columns=shot_zones_df.columns),
-                ignore_index=True
-            )
-            
-        shot_zones_df.columns = mi
-        self.close()
-        self.__init__()
-        return shot_zones_df
-    
-    
-    ####################################################################################################################
-    def scrape_attack_speeds(self, year, league):
-        """ Scrapes the attack speeds for each team in the year and league
-
-        Args
-        ----
-        year : int
-            Calendar year that the season ends in (e.g. 2023 for the 2022/23\
-            season)
-        league : str
-            League. Look in shared_functions.py for the available leagues for\
-            each module.
-
-        Returns
-        -------
-        : Pandas DataFrame
-            DataFrame containing the attack speeds of each team
-        """
-        check_season(year,league,'Understat')
-        
-        # Get links for teams in league that season
-        team_links = self.get_team_links(year, league)
-
-        mi = pd.MultiIndex.from_product(
-            [["Normal", "Standard", "Slow", "Fast"],
-             ["Sh", "G", "ShA", "GA", "xG", "xGA", "xGD", "xG/Sh", "xGA/Sh"]]
-        )
-        mi = mi.insert(0, ("Team names", "Team"))
-        attack_speeds_df = pd.DataFrame()#columns=mi)
-
-        for link in team_links:
-            
-            team_name = link.split("/")[-2]
-            self.driver.get(link)
-            self.driver.find_element(
-                By.XPATH, 
-                 "/html/body/div[1]/div[3]/div[3]/div/div[1]/div/label[6]"
-            ).click()
-            
-            table = self.driver.find_elements(By.TAG_NAME, "table")[0].get_attribute("outerHTML")
-            df = pd.read_html(table)[0]
-            df.drop(columns=["№"], inplace=True)
-
-            row = {
-                "Normal": None,
-                "Standard": None,
-                "Slow": None,
-                "Fast": None
-            }
-            for i in range(df.shape[0]):
-                # remove performance differential text from some columns
-                df.loc[i,"xG"] = self.remove_diff(df.loc[i,"xG"])
-                df.loc[i,"xGA"] = self.remove_diff(df.loc[i,"xGA"])
-
-                speed = df.loc[i, "Attack speed"]
-                row[speed] = df.loc[i,:].drop(labels=["Attack speed"])
-
-            row_array = []
-            for key in row.keys():
-                row_array.append(row[key].to_numpy())
-            row_array = np.array(row_array)
-            row_array = np.insert(row_array, 0, team_name) # insert team name
-
-            # append row
-            attack_speeds_df = attack_speeds_df.append(
-                pd.DataFrame(row_array.reshape(1,-1)),#, columns=attack_speeds_df.columns),
-                ignore_index=True
-            )
-            
-        attack_speeds_df.columns = mi
-        self.close()
-        self.__init__()
-        return attack_speeds_df
-    
-    
-    ####################################################################################################################
-    def scrape_shot_results(self, year, league):
-        """ Scrapes the shot results for each team in the year and league
-
-        Args
-        ----
-        year : int
-            Calendar year that the season ends in (e.g. 2023 for the 2022/23\
-            season)
-        league : str
-            League. Look in shared_functions.py for the available leagues for\
-            each module.
-
-        Returns
-        -------
-        : Pandas DataFrame
-            DataFrame containing the shot results data
-        """
-        check_season(year,league,'Understat')
-        
-        # Get links for teams in league that season
-        team_links = self.get_team_links(year, league)
-
-        mi = pd.MultiIndex.from_product(
-            [["Missed shot", "Goal", "Saved shot", "Blocked shot", "Shot on post"],
-             ["Sh", "G", "ShA", "GA", "xG", "xGA", "xGD", "xG/Sh", "xGA/Sh"]]
-        )
-        mi = mi.insert(0, ("Team names", "Team"))
-        shot_results_df = pd.DataFrame()#columns=mi)
-
-        for link in team_links:
-            
-            team_name = link.split("/")[-2]
-            self.driver.get(link)
-            self.driver.find_element(By.XPATH, "/html/body/div[1]/div[3]/div[3]/div/div[1]/div/label[7]").click()
-            table = self.driver.find_elements(By.TAG_NAME, "table")[0].get_attribute("outerHTML")
-            df = pd.read_html(table)[0]
-            df.drop(columns=["№"], inplace=True)
-
-            row = {
-                "Missed shot": None,
-                "Goal": None,
-                "Saved shot": None,
-                "Blocked shot": None,
-                "Shot on post": None
-            }
-            for i in range(df.shape[0]):
-                # remove performance differential text from some columns
-                df.loc[i,"xG"] = self.remove_diff(df.loc[i,"xG"])
-                df.loc[i,"xGA"] = self.remove_diff(df.loc[i,"xGA"])
-
-                result = df.loc[i, "Result"]
-                row[result] = df.loc[i,:].drop(labels=["Result"])
-
-            row_array = []
-            for key in row.keys():
-                row_array.append(row[key].to_numpy())
-            row_array = np.array(row_array)
-            row_array = np.insert(row_array, 0, team_name) # insert team name
-
-            # append row
-            shot_results_df = shot_results_df.append(
-                pd.DataFrame(row_array.reshape(1,-1)),
-                # columns=shot_results_df.columns),
-                ignore_index=True
-            )
-            
-        shot_results_df.columns = mi
-        self.close()
-        self.__init__()
-        return shot_results_df
-            
-        
-    ####################################################################################################################
-    def scrape_shot_xy(self, year, league, save=False, format='json'):
-        """ Scrapes the info for every shot in the league and year.
-
-        Args
-        ----
-        year : int
-            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
-        league : str
-            League. Look in shared_functions.py for the available leagues for each module.
-        save : bool
-            OPTIONAL, default if False. If True, shot XY's will be saved to a JSON file.
-        format : str
-            OPTIONAL, format of the output. Options are "json" and "dataframe"
-
-        Returns
-        -------
-        : dict, Padnas DataFrame, or str
-            Dict if save=False and format=json
-            Dataframe if save=False and format=json
-            Str if save=True. Filetype is determined by format argument
-        """
-        check_season(year,league,'Understat')
-
-        if format not in ['json', 'dataframe']:
-            raise ValueError('Format must be one of "json" or "dataframe".')
-        
-        season = str(year-1)+'-'+str(year)
-        links = self.get_match_links(year, league)
-        shots_data = dict()
-        failures = list()
-
-        for link in tqdm(links, desc='Shot XY'):
-            
-            match_id = link.split("/")[-1]
-            try:
-                game_shots_data = json.loads(
-                    requests.get(link).text\
-                        .split("shotsData")[1]\
-                        .split("JSON.parse(\'")[1]\
-                        .split("\')")[0]\
-                        .encode("latin-1")\
-                        .decode("unicode-escape")
-                )
-                shots_data[match_id] = game_shots_data
-            except:
-                failures.append(match_id)
-                shots_data[match_id] = "Error scraping"
-            
-        self.close()
-        self.__init__()
-        
-        # print any matches that scraping failed for
-        if len(failures) != 0:
-            print(f"Failed scraping the following matches: {failures}.")
-
-        # Convert json to dataframe if requested
-        if format == 'dataframe':
-            shots_df = pd.DataFrame()
-            for k in shots_data:
-                for team in shots_data[k]:
-                    shots_df = pd.concat([shots_df, pd.json_normalize(shots_data[k][team])], ignore_index=True, axis=0)
-            shots_data = shots_df
-        
-        # Save shots data to file if requested
-        if save:
-            filename_prefix = f'{season}_{league}_shot_xy'
-            if format == 'json':
-                filename = filename_prefix + '.json'
-                with open(filename, "w") as f:
-                    f.write(json.dumps(shots_data))
-            elif format == 'dataframe':
-                filename = filename_prefix + '.csv'
-                shots_data.to_csv(filename, index=False)
-            print(f'Understat shot XY saved to {filename}.')
-            shots_data = filename # return filename
-
-        return shots_data
+import datetime
+import json
+import numpy as np
+import pandas as pd
+from ScraperFC.shared_functions import check_season
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
+from selenium.webdriver.common.by import By
+from selenium.common.exceptions import NoSuchElementException
+from webdriver_manager.chrome import ChromeDriverManager
+from tqdm.auto import tqdm
+import requests
+from bs4 import BeautifulSoup
+import time
+
+
+class Understat:
+    
+    ####################################################################################################################
+    def __init__(self):
+        options = Options()
+        options.headless = True
+        options.add_argument("window-size=1400,600")
+        prefs = {'profile.managed_default_content_settings.images': 2} # don't load images
+        options.add_experimental_option('prefs', prefs)
+        self.driver = webdriver.Chrome(ChromeDriverManager().install(), options=options)
+        
+        
+    ####################################################################################################################
+    def close(self):
+        """ Closes and quits the Selenium WebDriver instance.
+        """
+        self.driver.close()
+        self.driver.quit()
+        
+        
+    ####################################################################################################################
+    def get_season_link(self, year, league):
+        """ Gets URL of the chosen league season.
+
+        Args
+        ----
+        year : int
+            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
+        league : str
+            League. Look in shared_functions.py for the available leagues for\
+            each module.
+
+        Returns
+        -------
+        : str
+            URL to the Understat page of the chosen league season.
+        """
+        lg = league.replace(" ","_")
+        url = f"https://understat.com/league/{lg}/{str(year-1)}"
+        return url
+        
+        
+    ####################################################################################################################
+    def get_match_links(self, year, league):
+        """ Gets all of the match links for the chosen league season
+
+        Args
+        ----
+        year : int
+            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
+        league : str
+            League. Look in shared_functions.py for the available leagues for\
+            each module.
+
+        Returns
+        -------
+        : list
+            List of match links of the chosen league season
+        """
+        check_season(year,league,'Understat')
+         
+        base_url = "https://understat.com/"
+        lg = league.replace(" ","_")
+        url = base_url+"league/"+lg+"/"+str(year-1)
+        self.driver.get(url)
+        
+        # Gather the links by hitting the "prev week" button until it's disabled
+        links = set()
+        btn = self.driver.find_element(By.CLASS_NAME, "calendar-prev")
+
+        while "disabled" not in btn.get_attribute("outerHTML"):
+            for el in self.driver.find_elements(By.CLASS_NAME, "match-info"):
+                links.add(el.get_attribute("href"))
+            btn.click()
+            
+        # One final collection for first week of season
+        for el in self.driver.find_elements(By.CLASS_NAME, "match-info"):
+            links.add(el.get_attribute("href"))
+                
+        # Remove Nones from the list of links 
+        links = np.array(list(links))
+        links = links[links!=None]
+
+        return list(links)
+    
+    ####################################################################################################################
+    def get_team_links(self, year, league):
+        """ Gets all of the team links for the chosen league season
+
+        Args
+        ----
+        year : int
+            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
+        league : str
+            League. Look in shared_functions.py for the available leagues for\
+            each module.
+
+        Returns
+        -------
+        : list
+            List of team URL's from the chosen season.
+        """
+        team_links = set()
+        self.driver.get(self.get_season_link(year, league))
+        for el in self.driver.find_elements(By.TAG_NAME, 'a'):
+            href = el.get_attribute('href')
+            if href and 'team' in href:
+                team_links.add(href)
+        return list(team_links)
+    
+    
+    ####################################################################################################################
+    def remove_diff(self, string):
+        """ Removes the plus/minus from some stats like xG.
+
+        Args
+        ----
+        string : str
+            The string to remove the difference from
+
+        Returns
+        -------
+        : str
+            String passed in as arg with the difference removed
+        """
+        string = string.split('-')[0]
+        return float(string.split('+')[0])
+    
+    
+    ####################################################################################################################
+    def unhide_stats(self, columns):
+        """ Understat doesn't display all stats by default. 
+        
+        This functions uses the stats currently shown in the table columns to\
+        unhide stats that aren't being displayed.
+
+        Args
+        ----
+        columns : Pandas DataFrame.columns
+            The columns currently shown in the table being scraped
+
+        Returns
+        -------
+        None
+        """
+        # Show the options popup
+        self.driver.find_elements(By.CLASS_NAME, "options-button")[0].click()
+        
+        # Iterate across all stats and show the ones that aren't in columns
+        for el in self.driver.find_elements(By.CLASS_NAME, "table-options-row"):
+            stat_name = el.find_element(By.CLASS_NAME, "row-title").text
+            if (stat_name not in columns) and (stat_name != ""):
+                el.find_element(By.CLASS_NAME, "row-display").click()
+
+        # click the apply button
+        self.driver.find_elements(By.CLASS_NAME, "button-apply")[0].click()
+        
+        return
+        
+        
+    ####################################################################################################################
+    def scrape_match(self, link):
+        """ Scrapes a single match from Understat.
+
+        Args
+        ----
+        link : str
+            URL to the match
+
+        Returns
+        -------
+        match : Pandas DataFrame
+            The match stats
+        """
+        # self.driver.get(link)
+        # soup = BeautifulSoup(self.driver.page_source, 'html.parser')
+        soup = BeautifulSoup(requests.get(link).content, 'html.parser')
+
+        # Match ID and date ============================================================================================
+        match_id = link.split('/')[-1]
+        date = soup.find('div', {'class': 'page-wrapper'}).find_all('li')[-1].text
+        date = datetime.datetime.strptime(date,'%b %d %Y').date()
+
+        # Shots data
+        shots_script = soup.find('div', {'class':'scheme-block', 'data-scheme':'chart'}).parent.find('script').text
+        shots_data = shots_script.split('JSON.parse(\'')[1].split('\')')[0]
+        shots_data = shots_data.encode('unicode_escape').replace(b'\\\\',b'\\').decode('unicode-escape')
+        shots_data = json.loads(shots_data)
+        shots_home_df = pd.json_normalize(shots_data['h'])
+        shots_away_df = pd.json_normalize(shots_data['a'])
+        all_shots_df = pd.concat([shots_home_df, shots_away_df], axis=0, ignore_index=True)
+        all_shots_df['minute'] = all_shots_df['minute'].astype(int)
+        all_shots_df = all_shots_df.sort_values('minute').reset_index(drop=True)
+
+        # Team stats table =============================================================================================
+        stats_scheme_block = soup.find_all('div', {'data-scheme':'stats'})
+        assert len(stats_scheme_block) == 1
+        stats_scheme_block = stats_scheme_block[0]
+        # Team Names
+        home_team, away_team = [
+            x.text for x in 
+            stats_scheme_block.find('div', {'class':'progress-bar teams-titles'}).find_all('div', {'class': 'progress-value'})
+        ]
+        # Chances
+        chances_bar = stats_scheme_block.find_all('div', {'class':'progress-bar'})[1]
+        home_chance = float(chances_bar.find('div', {'class':'progress-home'})['title'].replace('%',''))
+        draw_chance = float(chances_bar.find('div', {'class':'progress-draw'})['title'].replace('%',''))
+        away_chance = float(chances_bar.find('div', {'class':'progress-away'})['title'].replace('%',''))
+        # Goals
+        goals_bar = stats_scheme_block.find_all('div', {'class':'progress-bar'})[2]
+        home_goals, away_goals = [float(x.text) for x in goals_bar.find_all('div', {'class':'progress-value'})]
+        # xG
+        xg_bar = stats_scheme_block.find_all('div', {'class':'progress-bar'})[3]
+        home_xg, away_xg = [float(x.text) for x in xg_bar.find_all('div', {'class':'progress-value'})]
+        # Shots
+        shots_bar = stats_scheme_block.find_all('div', {'class':'progress-bar'})[4]
+        home_shots, away_shots = [float(x.text) for x in shots_bar.find_all('div', {'class':'progress-value'})]
+        # Shots on Target
+        sot_bar = stats_scheme_block.find_all('div', {'class':'progress-bar'})[5]
+        home_sot, away_sot = [float(x.text) for x in sot_bar.find_all('div', {'class':'progress-value'})]
+        # DEEP
+        deep_bar = stats_scheme_block.find_all('div', {'class':'progress-bar'})[6]
+        home_deep, away_deep = [float(x.text) for x in deep_bar.find_all('div', {'class':'progress-value'})]
+        # PPDA
+        ppda_bar = stats_scheme_block.find_all('div', {'class':'progress-bar'})[7]
+        home_ppda, away_ppda = [float(x.text) for x in ppda_bar.find_all('div', {'class':'progress-value'})]
+        # xPTS
+        xpts_bar = stats_scheme_block.find_all('div', {'class':'progress-bar'})[8]
+        home_xpts, away_xpts = [float(x.text) for x in xpts_bar.find_all('div', {'class':'progress-value'})]
+
+        # Player stats tables ==========================================================================================
+        players_script = soup.find('div', {'id':'match-rosters'}).parent.find('script').text
+        players_data = players_script.split('JSON.parse(\'')[1].split('\')')[0]
+        players_data = players_data.encode('unicode_escape').replace(b'\\\\',b'\\').decode('unicode-escape')
+        players_data = json.loads(players_data)
+        players_home_df = pd.json_normalize(players_data['h'].values())
+        players_away_df = pd.json_normalize(players_data['a'].values())
+
+        # Build match df ===============================================================================================
+        match = pd.Series(dtype=float)
+        match['id'] = match_id
+        match['date'] = date
+        match['shots'] = all_shots_df
+        match['home team'] = home_team
+        match['away team'] = away_team
+        match['home win proba'] = home_chance
+        match['draw proba'] = draw_chance
+        match['away win proba'] = away_chance
+        match['home goals'] = home_goals
+        match['away goals'] = away_goals
+        match['home xG'] = home_xg
+        match['away xG'] = away_xg
+        match['home shots'] = home_shots
+        match['away shots'] = away_shots
+        match['home SoT'] = home_sot
+        match['away SoT'] = away_sot
+        match['home DEEP'] = home_deep
+        match['away DEEP'] = away_deep
+        match['home PPDA'] = home_ppda
+        match['away PPDA'] = away_ppda
+        match['home xPTS'] = home_xpts
+        match['away xPTS'] = away_xpts
+        match['home player stats'] = players_home_df
+        match['away player stats'] = players_away_df
+        match = match.to_frame().T
+
+        return match
+        
+    ####################################################################################################################    
+    def scrape_matches(self, year, league, save=False):
+        """ Scrapes all of the matches from the chosen league season. 
+        
+        Gathers all match links from the chosen league season and then call\
+            scrape_match() on each one.
+
+        Args
+        ----
+        year : int
+            Calendar year that the season ends in (e.g. 2023 for the 2022/23\
+            season)
+        league : str
+            League. Look in shared_functions.py for the available leagues for\
+            each module.
+        save : bool
+            OPTIONAL, default False. If True, saves the DataFrame of match stats\
+            to a CSV.
+
+        Returns
+        -------
+        matches : Pandas DataFrame
+            If save=False
+        filename : str
+            If save=True, the filename the DataFrame was saved to
+        """
+        check_season(year,league,'Understat')
+        
+        season = str(year-1)+'-'+str(year)
+        links = self.get_match_links(year, league)
+        matches = pd.DataFrame()
+        
+        for link in tqdm(links):
+            match   = self.scrape_match(link)
+            matches = pd.concat([matches, match], ignore_index=True, axis=0)
+            time.sleep(2)
+        
+        # save to CSV if requested by user
+        if save:
+            filename = f'{season}_{league}_Understat_matches.csv'
+            matches.to_csv(path_or_buf=filename, index=False)
+            print('Matches dataframe saved to ' + filename)
+            return filename
+        else:
+            return matches
+        
+        
+    ####################################################################################################################
+    def scrape_league_table(self, year, league, normalize=False):
+        """ Scrapes the league table for the chosen league season.
+
+        Args
+        ----
+        year : int
+            Calendar year that the season ends in (e.g. 2023 for the 2022/23\
+            season)
+        league : str
+            League. Look in shared_functions.py for the available leagues for\
+            each module.
+        normalize : bool 
+            OPTIONAL, default False. If True, normalizes stats to per90
+
+        Returns
+        -------
+        : Pandas DataFrame
+            The league table of the chosen league season.
+        """
+        check_season(year,league,'Understat')
+        
+        url = self.get_season_link(year, league) # link to the selected league/season
+        self.driver.get(url)
+        
+        # Show all of the stats 
+        # Get column names currently show in the table
+        table = self.driver.find_elements(By.TAG_NAME, "table")[0].get_attribute("outerHTML")
+        columns = pd.read_html(table)[0].columns
+        self.unhide_stats(columns)
+
+        # dataframe 
+        table = self.driver.find_elements(By.TAG_NAME, "table")[0].get_attribute("outerHTML")
+        df = pd.read_html(table)[0]
+        
+        # remove performance differential text from some columns
+        for i in range(df.shape[0]):
+            df.loc[i,"xG"] = self.remove_diff(df.loc[i,"xG"])
+            df.loc[i,"xGA"] = self.remove_diff(df.loc[i,"xGA"])
+            df.loc[i,"xPTS"] = self.remove_diff(df.loc[i,"xPTS"])
+            
+        if normalize:
+            df.iloc[:,3:14] = df.iloc[:,3:14].divide(df["M"], axis="rows")
+            df.iloc[:,16:] = df.iloc[:,16:].divide(df["M"], axis="rows")
+        
+        self.close()
+        self.__init__()
+        return df
+    
+    
+    ####################################################################################################################
+    def scrape_home_away_tables(self, year, league, normalize=False):
+        """ Scrapes the home and away league tables for the chosen league season.
+
+        Args
+        ----
+        year : int
+            Calendar year that the season ends in (e.g. 2023 for the 2022/23\
+            season)
+        league : str
+            League. Look in shared_functions.py for the available leagues for\
+            each module.
+        normalize : bool 
+            OPTIONAL, default False. If True, normalizes stats to per90
+
+        Returns
+        -------
+        home : Pandas DataFrame
+            Home league table
+        away : Pandas DataFrame
+            Away league table
+        """
+        check_season(year,league,'Understat')
+        
+        url = self.get_season_link(year, league) # link to the selected league/season
+        self.driver.get(url)
+
+        # Show all of the stats
+        # Get columns that are already shown
+        labels = self.driver.find_elements(By.TAG_NAME, "label")
+        [el for el in labels if el.text=='home'][0].click()
+        table = self.driver.find_elements(By.TAG_NAME, "table")[0].get_attribute('outerHTML')
+        columns = pd.read_html(table)[0].columns 
+        self.unhide_stats(columns)
+        
+        # Home Table
+        labels = self.driver.find_elements(By.TAG_NAME, "label")
+        [el for el in labels if el.text=='home'][0].click()
+        table = self.driver.find_elements(By.TAG_NAME, "table")[0].get_attribute('outerHTML')
+        home = pd.read_html(table)[0]
+        
+        
+        # Away Table
+        [el for el in labels if el.text=='away'][0].click()
+        table = self.driver.find_elements(By.TAG_NAME, "table")[0].get_attribute('outerHTML')
+        away = pd.read_html(table)[0]
+        
+        # remove differentials from some columns
+        for i in range(home.shape[0]):
+            home.loc[i,"xG"] = self.remove_diff(home.loc[i,"xG"])
+            home.loc[i,"xGA"] = self.remove_diff(home.loc[i,"xGA"])
+            home.loc[i,"xPTS"] = self.remove_diff(home.loc[i,"xPTS"])
+            away.loc[i,"xG"] = self.remove_diff(away.loc[i,"xG"])
+            away.loc[i,"xGA"] = self.remove_diff(away.loc[i,"xGA"])
+            away.loc[i,"xPTS"] = self.remove_diff(away.loc[i,"xPTS"])
+        
+        if normalize:
+            home.iloc[:,3:14] = home.iloc[:,3:14].divide(home["M"], axis="rows")
+            home.iloc[:,16:] = home.iloc[:,16:].divide(home["M"], axis="rows")
+            away.iloc[:,3:14] = away.iloc[:,3:14].divide(away["M"], axis="rows")
+            away.iloc[:,16:] = away.iloc[:,16:].divide(away["M"], axis="rows")
+        
+        self.close()
+        self.__init__()
+        return home, away
+    
+    
+    ####################################################################################################################
+    def scrape_situations(self, year, league):
+        """ Scrapes the situations leading to shots for each team in the chosen\
+            league season.
+
+        Args
+        ----
+        year : int
+            Calendar year that the season ends in (e.g. 2023 for the 2022/23\
+            season)
+        league : str
+            League. Look in shared_functions.py for the available leagues for\
+            each module.
+
+        Returns
+        -------
+        : Pandas DataFrame
+            DataFrame containing the situations
+        """
+        check_season(year,league,'Understat')
+        
+        # Get links for teams in league that season
+        team_links = self.get_team_links(year, league)
+                
+        mi = pd.MultiIndex.from_product(
+            [["Open play", "From corner", "Set piece", "Direct FK", "Penalty"],
+             ["Sh", "G", "ShA", "GA", "xG", "xGA", "xGD", "xG/Sh", "xGA/Sh"]]
+        )
+        mi = mi.insert(0, ("Team names", "Team"))
+        situations = pd.DataFrame()#columns=mi)
+        
+        for link in team_links:
+            
+            team_name = link.split("/")[-2]
+            self.driver.get(link)
+            table = self.driver.find_elements(By.TAG_NAME, "table")[0].get_attribute("outerHTML")
+            df = pd.read_html(table)[0]
+            
+            for i in range(df.shape[0]):
+                # remove performance differential text from some columns
+                df.loc[i,"xG"] = self.remove_diff(df.loc[i,"xG"])
+                df.loc[i,"xGA"] = self.remove_diff(df.loc[i,"xGA"])
+            
+            # reformat df to fit into a row
+            df.drop(columns=["№","Situation"], inplace=True)
+            row = df.to_numpy()
+            row = np.insert(row, 0, team_name) # insert team name
+            
+            # append row
+            situations = situations.append(
+                pd.DataFrame(row.reshape(1,-1)),#, columns=situations.columns),
+                ignore_index=True
+            )
+        
+        situations.columns = mi
+        self.close()
+        self.__init__()
+        return situations
+    
+    
+    ####################################################################################################################
+    def scrape_formations(self, year, league):
+        """ Scrapes the stats for each team in the year and league, broken down\
+            by formation used by the team.
+
+        Args
+        ----
+        year : int
+            Calendar year that the season ends in (e.g. 2023 for the 2022/23\
+            season)
+        league : str
+            League. Look in shared_functions.py for the available leagues for\
+            each module.
+
+        Returns
+        -------
+        : dict
+            Keys are each team. Values are more dicts with keys for each formation\
+            and values are stats for each formation.
+        """
+        check_season(year,league,'Understat')
+        
+        # Get links for teams in league that season
+        team_links = self.get_team_links(year, league)
+        
+        formations = dict()
+        
+        for link in team_links:
+            
+            # Get team name to add to formations
+            team_name = link.split("/")[-2]
+            if team_name not in formations.keys():
+                formations[team_name] = dict()
+                
+            # Got to team's link, click formations, and get table of formations used
+            self.driver.get(link)
+            self.driver.find_element(
+                By.XPATH, 
+                "/html/body/div[1]/div[3]/div[3]/div/div[1]/div/label[2]"
+            ).click()
+            
+            table = self.driver.find_elements(By.TAG_NAME, "table")[0].get_attribute("outerHTML")
+            df = pd.read_html(table)[0]
+            df.drop(columns=["№"], inplace=True)
+            
+            # Remove performance differential text from some columns
+            for i in range(df.shape[0]):
+                df.loc[i,"xG"] = self.remove_diff(df.loc[i,"xG"])
+                df.loc[i,"xGA"] = self.remove_diff(df.loc[i,"xGA"])
+                
+                formation = df.loc[i,"Formation"]
+                
+                if formation not in formations[team_name].keys():
+                    formations[team_name][formation] = df.iloc[i,:].drop(columns=["№","Formation"])                
+                
+        self.close()
+        self.__init__()
+        return formations
+    
+    
+    ####################################################################################################################
+    def scrape_game_states(self, year, league):
+        """ Scrapes the game states for each team in the year and league
+
+        Args
+        ----
+        year : int
+            Calendar year that the season ends in (e.g. 2023 for the 2022/23\
+            season)
+        league : str
+            League. Look in shared_functions.py for the available leagues for\
+            each module.
+
+        Returns
+        -------
+        : Pandas DataFrame
+            DataFrame containing the game states
+        """
+        check_season(year,league,'Understat')
+        
+        # Get links for teams in league that season
+        team_links = self.get_team_links(year, league)
+                
+        mi = pd.MultiIndex.from_product(
+            [["Goal diff 0", "Goal diff -1", "Goal diff +1", "Goal diff < -1", "Goal diff > +1"],
+             ["Min", "Sh", "G", "ShA", "GA", "xG", "xGA", "xGD", "xG90", "xGA90"]]
+        )
+        mi = mi.insert(0, ("Team names", "Team"))
+        game_states = pd.DataFrame()#columns=mi)
+        
+        for link in team_links:
+            
+            team_name = link.split("/")[-2]
+            self.driver.get(link)
+            self.driver.find_element(
+                By.XPATH, 
+                "/html/body/div[1]/div[3]/div[3]/div/div[1]/div/label[3]"
+            ).click()
+            table = self.driver.find_elements(By.TAG_NAME, "table")[0].get_attribute("outerHTML")
+            df = pd.read_html(table)[0]
+            df.drop(columns=["№"], inplace=True)
+            
+            row = {
+                "Goal diff 0": None,
+                "Goal diff -1": None,
+                "Goal diff +1": None,
+                "Goal diff < -1": None,
+                "Goal diff > +1": None
+            }
+            for i in range(df.shape[0]):
+                # remove performance differential text from some columns
+                df.loc[i,"xG"] = self.remove_diff(df.loc[i,"xG"])
+                df.loc[i,"xGA"] = self.remove_diff(df.loc[i,"xGA"])
+                
+                game_state = df.loc[i,"Game state"]
+                row[game_state] = df.loc[i,:].drop(labels=["Game state"])
+                
+            row_array = []
+            for key in row.keys():
+                row_array.append( row[key].to_numpy() )
+            row_array = np.array(row_array)
+            row_array = np.insert(row_array, 0, team_name) # insert team name
+            
+            # append row
+            game_states = game_states.append(
+                pd.DataFrame(row_array.reshape(1,-1)),#, columns=game_states.columns),
+                ignore_index=True
+            )
+            
+        game_states.columns = mi
+        self.close()
+        self.__init__()
+        return game_states
+    
+    
+    ####################################################################################################################
+    def scrape_timing(self, year, league):
+        """ Scrapes the timing of goals for each team in the year and league
+
+        Args
+        ----
+        year : int
+            Calendar year that the season ends in (e.g. 2023 for the 2022/23\
+            season)
+        league : str
+            League. Look in shared_functions.py for the available leagues for\
+            each module.
+
+        Returns
+        -------
+        : Pandas DataFrame
+            DataFrame containing the timing stats
+        """
+        check_season(year,league,'Understat')
+        
+        # Get links for teams in league that season
+        team_links = self.get_team_links(year, league)
+
+        mi = pd.MultiIndex.from_product(
+            [["1-15", "16-30", "31-45", "46-60", "61-75", "76+"],
+             ["Sh", "G", "ShA", "GA", "xG", "xGA", "xGD", "xG/Sh", "xGA/Sh"]]
+        )
+        mi = mi.insert(0, ("Team names", "Team"))
+        timing_df = pd.DataFrame()#columns=mi)
+
+        for link in team_links:
+            
+            team_name = link.split("/")[-2]
+            self.driver.get(link)
+            self.driver.find_element(
+                By.XPATH, 
+                "/html/body/div[1]/div[3]/div[3]/div/div[1]/div/label[4]"
+            ).click()
+            table = self.driver.find_elements(By.TAG_NAME, "table")[0].get_attribute("outerHTML")
+            df = pd.read_html(table)[0]
+            df.drop(columns=["№"], inplace=True)
+
+            row = {
+                "1-15": None,
+                "16-30": None,
+                "31-45": None,
+                "46-60": None,
+                "61-75": None,
+                "76+": None
+            }
+            for i in range(df.shape[0]):
+                # remove performance differential text from some columns
+                df.loc[i,"xG"] = self.remove_diff(df.loc[i,"xG"])
+                df.loc[i,"xGA"] = self.remove_diff(df.loc[i,"xGA"])
+
+                timing = df.loc[i, "Timing"]
+                row[timing] = df.loc[i,:].drop(labels=["Timing"])
+
+            row_array = []
+            for key in row.keys():
+                row_array.append(row[key].to_numpy())
+            row_array = np.array(row_array)
+            row_array = np.insert(row_array, 0, team_name) # insert team name
+
+            # append row
+            timing_df = timing_df.append(
+                pd.DataFrame(row_array.reshape(1,-1)),#, columns=timing_df.columns),
+                ignore_index=True
+            )
+            
+        timing_df.columns = mi
+        self.close()
+        self.__init__()
+        return timing_df
+    
+    
+    ####################################################################################################################
+    def scrape_shot_zones(self, year, league):
+        """ Scrapes the shot zones for each team in the year and league
+
+        Args
+        ----
+        year : int
+            Calendar year that the season ends in (e.g. 2023 for the 2022/23\
+            season)
+        league : str
+            League. Look in shared_functions.py for the available leagues for\
+            each module.
+
+        Returns
+        -------
+        : Pandas DataFrame
+            DataFrame containing the shot zones data
+        """
+        check_season(year,league,'Understat')
+        
+        # Get links for teams in league that season
+        team_links = self.get_team_links(year, league)
+
+        mi = pd.MultiIndex.from_product(
+            [["Own goals", "Out of box", "Penalty area", "Six-yard box"],
+             ["Sh", "G", "ShA", "GA", "xG", "xGA", "xGD", "xG/Sh", "xGA/Sh"]]
+        )
+        mi = mi.insert(0, ("Team names", "Team"))
+        shot_zones_df = pd.DataFrame()#columns=mi)
+
+        for link in team_links:
+            
+            team_name = link.split("/")[-2]
+            self.driver.get(link)
+            self.driver.find_element(
+                By.XPATH, 
+                "/html/body/div[1]/div[3]/div[3]/div/div[1]/div/label[5]"
+            ).click()
+            table = self.driver.find_elements(By.TAG_NAME, "table")[0].get_attribute("outerHTML")
+            df = pd.read_html(table)[0]
+            df.drop(columns=["№"], inplace=True)
+
+            row = {
+                "Own goals": None,
+                "Out of box": None,
+                "Penalty area": None,
+                "Six-yard box": None
+            }
+            for i in range(df.shape[0]):
+                # remove performance differential text from some columns
+                df.loc[i,"xG"] = self.remove_diff(df.loc[i,"xG"])
+                df.loc[i,"xGA"] = self.remove_diff(df.loc[i,"xGA"])
+
+                zone = df.loc[i, "Shot zones"]
+                row[zone] = df.loc[i,:].drop(labels=["Shot zones"])
+
+            row_array = []
+            for key in row.keys():
+                if row[key] is None:
+                    row[key] = pd.Series(np.zeros((9)))
+                row_array.append(row[key].to_numpy())
+            row_array = np.array(row_array)
+            row_array = np.insert(row_array, 0, team_name) # insert team name
+
+            # append row
+            shot_zones_df = shot_zones_df.append(
+                pd.DataFrame(row_array.reshape(1,-1)),#, columns=shot_zones_df.columns),
+                ignore_index=True
+            )
+            
+        shot_zones_df.columns = mi
+        self.close()
+        self.__init__()
+        return shot_zones_df
+    
+    
+    ####################################################################################################################
+    def scrape_attack_speeds(self, year, league):
+        """ Scrapes the attack speeds for each team in the year and league
+
+        Args
+        ----
+        year : int
+            Calendar year that the season ends in (e.g. 2023 for the 2022/23\
+            season)
+        league : str
+            League. Look in shared_functions.py for the available leagues for\
+            each module.
+
+        Returns
+        -------
+        : Pandas DataFrame
+            DataFrame containing the attack speeds of each team
+        """
+        check_season(year,league,'Understat')
+        
+        # Get links for teams in league that season
+        team_links = self.get_team_links(year, league)
+
+        mi = pd.MultiIndex.from_product(
+            [["Normal", "Standard", "Slow", "Fast"],
+             ["Sh", "G", "ShA", "GA", "xG", "xGA", "xGD", "xG/Sh", "xGA/Sh"]]
+        )
+        mi = mi.insert(0, ("Team names", "Team"))
+        attack_speeds_df = pd.DataFrame()#columns=mi)
+
+        for link in team_links:
+            
+            team_name = link.split("/")[-2]
+            self.driver.get(link)
+            self.driver.find_element(
+                By.XPATH, 
+                 "/html/body/div[1]/div[3]/div[3]/div/div[1]/div/label[6]"
+            ).click()
+            
+            table = self.driver.find_elements(By.TAG_NAME, "table")[0].get_attribute("outerHTML")
+            df = pd.read_html(table)[0]
+            df.drop(columns=["№"], inplace=True)
+
+            row = {
+                "Normal": None,
+                "Standard": None,
+                "Slow": None,
+                "Fast": None
+            }
+            for i in range(df.shape[0]):
+                # remove performance differential text from some columns
+                df.loc[i,"xG"] = self.remove_diff(df.loc[i,"xG"])
+                df.loc[i,"xGA"] = self.remove_diff(df.loc[i,"xGA"])
+
+                speed = df.loc[i, "Attack speed"]
+                row[speed] = df.loc[i,:].drop(labels=["Attack speed"])
+
+            row_array = []
+            for key in row.keys():
+                row_array.append(row[key].to_numpy())
+            row_array = np.array(row_array)
+            row_array = np.insert(row_array, 0, team_name) # insert team name
+
+            # append row
+            attack_speeds_df = attack_speeds_df.append(
+                pd.DataFrame(row_array.reshape(1,-1)),#, columns=attack_speeds_df.columns),
+                ignore_index=True
+            )
+            
+        attack_speeds_df.columns = mi
+        self.close()
+        self.__init__()
+        return attack_speeds_df
+    
+    
+    ####################################################################################################################
+    def scrape_shot_results(self, year, league):
+        """ Scrapes the shot results for each team in the year and league
+
+        Args
+        ----
+        year : int
+            Calendar year that the season ends in (e.g. 2023 for the 2022/23\
+            season)
+        league : str
+            League. Look in shared_functions.py for the available leagues for\
+            each module.
+
+        Returns
+        -------
+        : Pandas DataFrame
+            DataFrame containing the shot results data
+        """
+        check_season(year,league,'Understat')
+        
+        # Get links for teams in league that season
+        team_links = self.get_team_links(year, league)
+
+        mi = pd.MultiIndex.from_product(
+            [["Missed shot", "Goal", "Saved shot", "Blocked shot", "Shot on post"],
+             ["Sh", "G", "ShA", "GA", "xG", "xGA", "xGD", "xG/Sh", "xGA/Sh"]]
+        )
+        mi = mi.insert(0, ("Team names", "Team"))
+        shot_results_df = pd.DataFrame()#columns=mi)
+
+        for link in team_links:
+            
+            team_name = link.split("/")[-2]
+            self.driver.get(link)
+            self.driver.find_element(By.XPATH, "/html/body/div[1]/div[3]/div[3]/div/div[1]/div/label[7]").click()
+            table = self.driver.find_elements(By.TAG_NAME, "table")[0].get_attribute("outerHTML")
+            df = pd.read_html(table)[0]
+            df.drop(columns=["№"], inplace=True)
+
+            row = {
+                "Missed shot": None,
+                "Goal": None,
+                "Saved shot": None,
+                "Blocked shot": None,
+                "Shot on post": None
+            }
+            for i in range(df.shape[0]):
+                # remove performance differential text from some columns
+                df.loc[i,"xG"] = self.remove_diff(df.loc[i,"xG"])
+                df.loc[i,"xGA"] = self.remove_diff(df.loc[i,"xGA"])
+
+                result = df.loc[i, "Result"]
+                row[result] = df.loc[i,:].drop(labels=["Result"])
+
+            row_array = []
+            for key in row.keys():
+                row_array.append(row[key].to_numpy())
+            row_array = np.array(row_array)
+            row_array = np.insert(row_array, 0, team_name) # insert team name
+
+            # append row
+            shot_results_df = shot_results_df.append(
+                pd.DataFrame(row_array.reshape(1,-1)),
+                # columns=shot_results_df.columns),
+                ignore_index=True
+            )
+            
+        shot_results_df.columns = mi
+        self.close()
+        self.__init__()
+        return shot_results_df
+            
+        
+    ####################################################################################################################
+    def scrape_shot_xy(self, year, league, save=False, format='json'):
+        """ Scrapes the info for every shot in the league and year.
+
+        Args
+        ----
+        year : int
+            Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
+        league : str
+            League. Look in shared_functions.py for the available leagues for each module.
+        save : bool
+            OPTIONAL, default if False. If True, shot XY's will be saved to a JSON file.
+        format : str
+            OPTIONAL, format of the output. Options are "json" and "dataframe"
+
+        Returns
+        -------
+        : dict, Padnas DataFrame, or str
+            Dict if save=False and format=json
+            Dataframe if save=False and format=json
+            Str if save=True. Filetype is determined by format argument
+        """
+        check_season(year,league,'Understat')
+
+        if format not in ['json', 'dataframe']:
+            raise ValueError('Format must be one of "json" or "dataframe".')
+        
+        season = str(year-1)+'-'+str(year)
+        links = self.get_match_links(year, league)
+        shots_data = dict()
+        failures = list()
+
+        for link in tqdm(links, desc='Shot XY'):
+            
+            match_id = link.split("/")[-1]
+            try:
+                game_shots_data = json.loads(
+                    requests.get(link).text\
+                        .split("shotsData")[1]\
+                        .split("JSON.parse(\'")[1]\
+                        .split("\')")[0]\
+                        .encode("latin-1")\
+                        .decode("unicode-escape")
+                )
+                shots_data[match_id] = game_shots_data
+            except:
+                failures.append(match_id)
+                shots_data[match_id] = "Error scraping"
+            
+        self.close()
+        self.__init__()
+        
+        # print any matches that scraping failed for
+        if len(failures) != 0:
+            print(f"Failed scraping the following matches: {failures}.")
+
+        # Convert json to dataframe if requested
+        if format == 'dataframe':
+            shots_df = pd.DataFrame()
+            for k in shots_data:
+                for team in shots_data[k]:
+                    shots_df = pd.concat([shots_df, pd.json_normalize(shots_data[k][team])], ignore_index=True, axis=0)
+            shots_data = shots_df
+        
+        # Save shots data to file if requested
+        if save:
+            filename_prefix = f'{season}_{league}_shot_xy'
+            if format == 'json':
+                filename = filename_prefix + '.json'
+                with open(filename, "w") as f:
+                    f.write(json.dumps(shots_data))
+            elif format == 'dataframe':
+                filename = filename_prefix + '.csv'
+                shots_data.to_csv(filename, index=False)
+            print(f'Understat shot XY saved to {filename}.')
+            shots_data = filename # return filename
+
+        return shots_data
```

### Comparing `ScraperFC-2.6.5/ScraperFC/shared_functions.py` & `ScraperFC-2.7.0/ScraperFC/shared_functions.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,449 +1,449 @@
-from selenium import webdriver
-from selenium.webdriver.chrome.options import Options
-from selenium.webdriver.common.by import By
-from webdriver_manager.chrome import ChromeDriverManager
-from IPython.display import clear_output
-import random
-import pandas as pd
-import numpy as np
-
-# Dict of data sources and leagues for each source
-sources = {
-    'All': {},
-    'FBRef': {
-        # Each competition gets its first valid year (from the competition seasons history page on fbref), the url
-        # to the season history page, and the 'finder' which is used to find the season and match links in HTML
-        #################################
-        # Men's club international cups #
-        #################################
-        'Copa Libertadores': {
-            'first valid year': 2014,
-            'url': 'https://fbref.com/en/comps/14/history/Copa-Libertadores-Seasons',
-            'finder': ['Copa-Libertadores'],
-        },
-        'Champions League': {
-            'first valid year': 1991,
-            'url': 'https://fbref.com/en/comps/8/history/Champions-League-Seasons',
-            'finder': ['European-Cup', 'Champions-League'],
-        },
-        'Europa League': {
-            'first valid year': 1991,
-            'url': 'https://fbref.com/en/comps/19/history/Europa-League-Seasons',
-            'finder': ['UEFA-Cup', 'Europa-League'],
-        },
-        'Europa Conference League': {
-            'first valid year': 2022,
-            'url': 'https://fbref.com/en/comps/882/history/Europa-Conference-League-Seasons',
-            'finder': ['Europa-Conference-League'],
-        },
-        ####################################
-        # Men's national team competitions #
-        ####################################
-        'World Cup': {
-            'first valid year': 1930,
-            'url': 'https://fbref.com/en/comps/1/history/World-Cup-Seasons',
-            'finder': ['World-Cup'],
-        },
-        'Copa America': {
-            'first valid year': 2015,
-            'url': 'https://fbref.com/en/comps/685/history/Copa-America-Seasons',
-            'finder': ['Copa-America'],
-        },
-        'Euros': {
-            'first valid year': 2000,
-            'url': 'https://fbref.com/en/comps/676/history/European-Championship-Seasons',
-            'finder': ['UEFA-Euro', 'European-Championship'],
-        },
-        ###############
-        # Men's big 5 #
-        ###############
-        'Big 5 combined': {
-            'first valid year': 1996,
-            'url': 'https://fbref.com/en/comps/Big5/history/Big-5-European-Leagues-Seasons',
-            'finder': ['Big-5-European-Leagues'],
-        },
-        'EPL': {
-            'first valid year': 1993,
-            'url': 'https://fbref.com/en/comps/9/history/Premier-League-Seasons',
-            'finder': ['Premier-League'],
-        },
-        'Ligue 1': {
-            'first valid year': 1996,
-            'url': 'https://fbref.com/en/comps/13/history/Ligue-1-Seasons',
-            'finder': ['Ligue-1', 'Division-1'],
-        },
-        'Bundesliga': {
-            'first valid year': 1989,
-            'url': 'https://fbref.com/en/comps/20/history/Bundesliga-Seasons',
-            'finder': ['Bundesliga'],
-        },
-        'Serie A': {
-            'first valid year': 1989,
-            'url': 'https://fbref.com/en/comps/11/history/Serie-A-Seasons',
-            'finder': ['Serie-A'],
-        },
-        'La Liga': {
-            'first valid year': 1989,
-            'url': 'https://fbref.com/en/comps/12/history/La-Liga-Seasons',
-            'finder': ['La-Liga'],
-        },
-        #####################################
-        # Men's domestic leagues - 1st tier #
-        #####################################
-        'MLS': {
-            'first valid year': 1996,
-            'url': 'https://fbref.com/en/comps/22/history/Major-League-Soccer-Seasons',
-            'finder': ['Major-League-Soccer'],
-        },
-        'Brazilian Serie A': {
-            'first valid year': 2014,
-            'url': 'https://fbref.com/en/comps/24/history/Serie-A-Seasons',
-            'finder': ['Serie-A'],
-        },
-        'Eredivisie': {
-            'first valid year': 2001,
-            'url': 'https://fbref.com/en/comps/23/history/Eredivisie-Seasons',
-            'finder': ['Eredivisie'],
-        },
-        'Liga MX': {
-            'first valid year': 2004,
-            'url': 'https://fbref.com/en/comps/31/history/Liga-MX-Seasons',
-            'finder': ['Primera-Division', 'Liga-MX'],
-        },
-        'Primeira Liga': {
-            'first valid year': 2001,
-            'url': 'https://fbref.com/en/comps/32/history/Primeira-Liga-Seasons',
-            'finder': ['Primeira-Liga'],
-        },
-        ####################################
-        # Men's domestic league - 2nd tier #
-        ####################################
-        'EFL Championship': {
-            'first valid year': 2002,
-            'url': 'https://fbref.com/en/comps/10/history/Championship-Seasons',
-            'finder': ['First-Division', 'Championship'],
-        },
-        ##############################################
-        # Men's domestic league - 3rd tier and lower #
-        ##############################################
-        #######################
-        # Men's domestic cups #
-        #######################
-        #########################################
-        # Women's internation club competitions #
-        #########################################
-        'Women Champions League': {
-            'first valid year': 2015,
-            'url': 'https://fbref.com/en/comps/181/history/Champions-League-Seasons',
-            'finder': ['Champions-League'],
-        },
-        ######################################
-        # Women's national team competitions #
-        ######################################
-        'Womens World Cup': {
-            'first valid year': 1991,
-            'url': 'https://fbref.com/en/comps/106/history/Womens-World-Cup-Seasons',
-            'finder': ['Womens-World-Cup'],
-        },
-        'Womens Euros': {
-            'first valid year': 2001,
-            'url': 'https://fbref.com/en/comps/162/history/UEFA-Womens-Euro-Seasons',
-            'finder': ['UEFA-Womens-Euro'],
-        },
-        ############################
-        # Women's domestic leagues #
-        ############################
-        'NWSL': {
-            'first valid year': 2013,
-            'url': 'https://fbref.com/en/comps/182/history/NWSL-Seasons',
-            'finder': ['NWSL'],
-        },
-        'A-League Women': {
-            'first valid year': 2019,
-            'url': 'https://fbref.com/en/comps/196/history/A-League-Women-Seasons',
-            'finder': ['A-League-Women', 'W-League'],
-        },
-        'WSL': {
-            'first valid year': 2017,
-            'url': 'https://fbref.com/en/comps/189/history/Womens-Super-League-Seasons',
-            'finder': ['Womens-Super-League'],
-        },
-        'D1 Feminine': {
-            'first valid year': 2018,
-            'url': 'https://fbref.com/en/comps/193/history/Division-1-Feminine-Seasons',
-            'finder': ['Division-1-Feminine'],
-        },
-        'Womens Bundesliga': {
-            'first valid year': 2017,
-            'url': 'https://fbref.com/en/comps/183/history/Frauen-Bundesliga-Seasons',
-            'finder': ['Frauen-Bundesliga'],
-        },
-        'Womens Serie A': {
-            'first valid year': 2019,
-            'url': 'https://fbref.com/en/comps/208/history/Serie-A-Seasons',
-            'finder': ['Serie-A'],
-        },
-        'Liga F': {
-            'first valid year': 2023,
-            'url': 'https://fbref.com/en/comps/230/history/Liga-F-Seasons',
-            'finder': ['Liga-F'],
-        },
-        #########################
-        # Women's domestic cups #
-        #########################
-        'NWSL Challenge Cup': {
-            'first valid year': 2020,
-            'url': 'https://fbref.com/en/comps/881/history/NWSL-Challenge-Cup-Seasons',
-            'finder': ['NWSL-Challenge-Cup'],
-        },
-        'NWSL Fall Series': {
-            'first valid year': 2020,
-            'url': 'https://fbref.com/en/comps/884/history/NWSL-Fall-Series-Seasons',
-            'finder': ['NWSL-Fall-Series'],
-        },
-    },
-    'Understat': {
-        'EPL': {'first valid year': 2015,},
-        'La Liga': {'first valid year': 2015,},
-        'Bundesliga':  {'first valid year': 2015,},
-        'Serie A':  {'first valid year': 2015,},
-        'Ligue 1':  {'first valid year': 2015,},
-    },
-    'FiveThirtyEight': {
-        'EPL':  {'first valid year': 2017,},
-        'La Liga':  {'first valid year': 2017,},
-        'Bundesliga':  {'first valid year': 2017,},
-        'Serie A':  {'first valid year': 2017,},
-        'Ligue 1':  {'first valid year': 2017,},
-    },
-    'SofaScore': {'USL League One':  {'first valid year': 2019,}},
-    'Capology': {
-        'Bundesliga':  {'first valid year': 2014,},
-        '2.Bundesliga':  {'first valid year': 2020,},
-        'EPL':  {'first valid year': 2014,},
-        'EFL Championship':  {'first valid year': 2014,},
-        'Serie A':  {'first valid year': 2010,},
-        'Serie B':  {'first valid year': 2020,},
-        'La Liga':  {'first valid year': 2014,},
-        'La Liga 2':  {'first valid year': 2020,},
-        'Ligue 1':  {'first valid year': 2014,},
-        'Ligue 2':  {'first valid year': 2020,},
-        'Eredivisie':  {'first valid year': 2014,},
-        'Primeira Liga':  {'first valid year': 2014,},
-        'Scottish PL':  {'first valid year': 2020,},
-        'Super Lig':  {'first valid year': 2014,},
-        'Belgian 1st Division':  {'first valid year': 2014,},
-    },
-    'Transfermarkt': {
-        'EPL':  {'first valid year': 1993,},
-        'EFL Championship': {'first valid year': 2005,},
-        'EFL1': {'first valid year': 2005,},
-        'EFL2': {'first valid year': 2005,},
-        'Bundesliga': {'first valid year': 1964,},
-        '2.Bundesliga': {'first valid year': 1982,},
-        'Serie A': {'first valid year': 1930,},
-        'Serie B': {'first valid year': 1930,},
-        'La Liga': {'first valid year': 1929,},
-        'La Liga 2': {'first valid year': 1929,},
-        'Ligue 1': {'first valid year': 1970,},
-        'Ligue 2': {'first valid year': 1993,},
-        'Eredivisie': {'first valid year': 1955,},
-        'Scottish PL': {'first valid year': 2004,},
-        'Super Lig': {'first valid year': 1960,},
-        'Jupiler Pro League': {'first valid year': 1987,},
-        'Liga Nos': {'first valid year': 1994,},
-        'Russian Premier League': {'first valid year': 2011,},
-        'Brasileirao': {'first valid year': 2001,},
-        'Argentina Liga Profesional': {'first valid year': 2015,},
-        'MLS': {'first valid year': 1996,},
-    },
-}
-
-########################################################################################################################
-class InvalidSourceException(Exception):
-    ''' Raised when an invalid source is used with the check_season() function.
-    '''
-    def __init__(self, source):
-        super().__init__()
-        self.source = source
-    def __str__(self):
-        return f'{self.source} is not a valid source. Must be one of {list(sources.keys())}.'
-
-########################################################################################################################
-class InvalidLeagueException(Exception):
-    ''' Raised when an invalid league is used with the check_season() function.
-    '''
-    def __init__(self, league, source):
-        super().__init__()
-        self.league = league
-        self.source = source
-    def __str__(self):
-        return f'{self.league} is not a valid league for {self.source}. Options are {list(sources[self.source].keys())}.'
-
-########################################################################################################################
-class InvalidYearException(Exception):
-    ''' Raised when an invalid year is used with the check_season() function.
-    '''
-    def __init__(self, year, league, source):
-        super().__init__()
-        self.year = year
-        self.league = league
-        self.source = source
-    def __str__(self):
-        return f'{self.year} invalid for source {self.source} and league {self.league}. ' +\
-            f'Must be {sources[self.source][self.league]["first valid year"]} or later.'
-
-########################################################################################################################
-class InvalidCurrencyException(Exception):
-    ''' Raised when an invalid currency is used with the Capology module.
-    '''
-    def __init__(self):
-        super().__init__()
-    def __str__():
-        return 'Currency must be one of "eur", "gbp", or "usd".'
-
-########################################################################################################################
-class UnavailableSeasonException(Exception):
-    ''' Raised when a given year and league is unavailable from a source.
-    '''
-    def __init__(self, year, league, source):
-        super().__init__()
-        self.year = year
-        self.league = league
-        self.source = source
-    def __str__(self):
-        return f'No {self.league} {self.year} season is available on {self.source}.'
-
-########################################################################################################################
-class NoMatchLinksException(Exception):
-    ''' Raised when no match links are found
-    '''
-    def __init__(self, fixtures_url, year, league):
-        super().__init__()
-        self.fixtures_url = fixtures_url
-        self.league = league
-        self.year = year
-    def __str__(self):
-        return f'No match score elements with links found at {self.fixtures_url} for {self.year} {self.league}.'
-
-########################################################################################################################
-def check_season(year, league, source):
-    ''' Checks to make sure that the given league season is a valid season for the scraper.
-    
-    Args
-    ----
-    year : int
-        Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
-    league : str
-        League. Look in shared_functions.py for the available leagues for each\
-        module.
-    source : str
-        The scraper to be checked (e.g. 'FBRef', 'Transfermarkt, etc.). These\
-        are the ScraperFC modules.
-    Returns
-    -------
-    err : str
-        String of the error message, if there is one.
-    valid : bool
-        True if the league season is valid for the scraper. False otherwise.
-    '''
-    # Check source
-    if source not in list(sources.keys()):
-        raise InvalidSourceException(source)
-
-    # Check league
-    if type(league)!=str:
-        raise TypeError('League must be a string.')
-    if league not in list(sources[source].keys()):
-        raise InvalidLeagueException(league, source)
-    
-    # Check year
-    if type(year) != int:
-        raise TypeError('Year must be an integer.')
-    if year < sources[source][league]['first valid year']:
-        raise InvalidYearException(year, league, source)
-    
-    return
-
-########################################################################################################################
-def get_proxy():
-    ''' Gets a proxy address.
-
-    Can be used to initialize a Selenium WebDriver to change the address of the\
-    browser. Adapted from https://stackoverflow.com/questions/59409418/how-to-rotate-selenium-webrowser-ip-address.\
-    Randomly chooses one proxy.
-    
-    Returns
-    -------
-    proxy : str
-        In the form <IP address>:<port>
-    '''
-    options = Options()
-    options.headless = True
-    options.add_argument('window-size=700,600')
-    driver = webdriver.Chrome(ChromeDriverManager().install(), options=options)
-    clear_output()
-    
-    try:
-        driver.get('https://sslproxies.org/')
-        table = driver.find_elements(By.TAG_NAME, 'table')[0]
-        df = pd.read_html(table.get_attribute('outerHTML'))[0]
-        df = df.iloc[np.where(~np.isnan(df['Port']))[0],:] # ignore nans
-
-        ips = df['IP Address'].values
-        ports = df['Port'].astype('int').values
-
-        driver.quit()
-        proxies = list()
-        for i in range(len(ips)):
-            proxies.append('{}:{}'.format(ips[i], ports[i]))
-        i = random.randint(0, len(proxies)-1)
-        return proxies[i]
-    except Exception as e:
-        driver.close()
-        driver.quit()
-        raise e
-        
-########################################################################################################################
-def xpath_soup(element):
-    ''' Generate xpath from BeautifulSoup4 element.
-    
-    I shamelessly stole this from https://gist.github.com/ergoithz/6cf043e3fdedd1b94fcf.
-    
-    Args
-    ----
-    element : bs4.element.Tag or bs4.element.NavigableString
-        BeautifulSoup4 element.
-    Returns
-    -------
-    : str
-        xpath as string
-    Usage
-    -----
-    >>> import bs4
-    >>> html = (
-    ...     '<html><head><title>title</title></head>'
-    ...     '<body><p>p <i>1</i></p><p>p <i>2</i></p></body></html>'
-    ...     )
-    >>> soup = bs4.BeautifulSoup(html, 'html.parser')
-    >>> xpath_soup(soup.html.body.p.i)
-    '/html/body/p[1]/i'
-    >>> import bs4
-    >>> xml = '<doc><elm/><elm/></doc>'
-    >>> soup = bs4.BeautifulSoup(xml, 'lxml-xml')
-    >>> xpath_soup(soup.doc.elm.next_sibling)
-    '/doc/elm[2]'
-    '''
-    components = []
-    child = element if element.name else element.parent
-    for parent in child.parents:  # type: bs4.element.Tag
-        siblings = parent.find_all(child.name, recursive=False)
-        components.append(
-            child.name if 1 == len(siblings) else '%s[%d]' % (
-                child.name,
-                next(i for i, s in enumerate(siblings, 1) if s is child)
-                )
-            )
-        child = parent
-    components.reverse()
-    return '/%s' % '/'.join(components)
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
+from selenium.webdriver.common.by import By
+from webdriver_manager.chrome import ChromeDriverManager
+from IPython.display import clear_output
+import random
+import pandas as pd
+import numpy as np
+
+# Dict of data sources and leagues for each source
+sources = {
+    'All': {},
+    'FBRef': {
+        # Each competition gets its first valid year (from the competition seasons history page on fbref), the url
+        # to the season history page, and the 'finder' which is used to find the season and match links in HTML
+        #################################
+        # Men's club international cups #
+        #################################
+        'Copa Libertadores': {
+            'first valid year': 2014,
+            'url': 'https://fbref.com/en/comps/14/history/Copa-Libertadores-Seasons',
+            'finder': ['Copa-Libertadores'],
+        },
+        'Champions League': {
+            'first valid year': 1991,
+            'url': 'https://fbref.com/en/comps/8/history/Champions-League-Seasons',
+            'finder': ['European-Cup', 'Champions-League'],
+        },
+        'Europa League': {
+            'first valid year': 1991,
+            'url': 'https://fbref.com/en/comps/19/history/Europa-League-Seasons',
+            'finder': ['UEFA-Cup', 'Europa-League'],
+        },
+        'Europa Conference League': {
+            'first valid year': 2022,
+            'url': 'https://fbref.com/en/comps/882/history/Europa-Conference-League-Seasons',
+            'finder': ['Europa-Conference-League'],
+        },
+        ####################################
+        # Men's national team competitions #
+        ####################################
+        'World Cup': {
+            'first valid year': 1930,
+            'url': 'https://fbref.com/en/comps/1/history/World-Cup-Seasons',
+            'finder': ['World-Cup'],
+        },
+        'Copa America': {
+            'first valid year': 2015,
+            'url': 'https://fbref.com/en/comps/685/history/Copa-America-Seasons',
+            'finder': ['Copa-America'],
+        },
+        'Euros': {
+            'first valid year': 2000,
+            'url': 'https://fbref.com/en/comps/676/history/European-Championship-Seasons',
+            'finder': ['UEFA-Euro', 'European-Championship'],
+        },
+        ###############
+        # Men's big 5 #
+        ###############
+        'Big 5 combined': {
+            'first valid year': 1996,
+            'url': 'https://fbref.com/en/comps/Big5/history/Big-5-European-Leagues-Seasons',
+            'finder': ['Big-5-European-Leagues'],
+        },
+        'EPL': {
+            'first valid year': 1993,
+            'url': 'https://fbref.com/en/comps/9/history/Premier-League-Seasons',
+            'finder': ['Premier-League'],
+        },
+        'Ligue 1': {
+            'first valid year': 1996,
+            'url': 'https://fbref.com/en/comps/13/history/Ligue-1-Seasons',
+            'finder': ['Ligue-1', 'Division-1'],
+        },
+        'Bundesliga': {
+            'first valid year': 1989,
+            'url': 'https://fbref.com/en/comps/20/history/Bundesliga-Seasons',
+            'finder': ['Bundesliga'],
+        },
+        'Serie A': {
+            'first valid year': 1989,
+            'url': 'https://fbref.com/en/comps/11/history/Serie-A-Seasons',
+            'finder': ['Serie-A'],
+        },
+        'La Liga': {
+            'first valid year': 1989,
+            'url': 'https://fbref.com/en/comps/12/history/La-Liga-Seasons',
+            'finder': ['La-Liga'],
+        },
+        #####################################
+        # Men's domestic leagues - 1st tier #
+        #####################################
+        'MLS': {
+            'first valid year': 1996,
+            'url': 'https://fbref.com/en/comps/22/history/Major-League-Soccer-Seasons',
+            'finder': ['Major-League-Soccer'],
+        },
+        'Brazilian Serie A': {
+            'first valid year': 2014,
+            'url': 'https://fbref.com/en/comps/24/history/Serie-A-Seasons',
+            'finder': ['Serie-A'],
+        },
+        'Eredivisie': {
+            'first valid year': 2001,
+            'url': 'https://fbref.com/en/comps/23/history/Eredivisie-Seasons',
+            'finder': ['Eredivisie'],
+        },
+        'Liga MX': {
+            'first valid year': 2004,
+            'url': 'https://fbref.com/en/comps/31/history/Liga-MX-Seasons',
+            'finder': ['Primera-Division', 'Liga-MX'],
+        },
+        'Primeira Liga': {
+            'first valid year': 2001,
+            'url': 'https://fbref.com/en/comps/32/history/Primeira-Liga-Seasons',
+            'finder': ['Primeira-Liga'],
+        },
+        ####################################
+        # Men's domestic league - 2nd tier #
+        ####################################
+        'EFL Championship': {
+            'first valid year': 2002,
+            'url': 'https://fbref.com/en/comps/10/history/Championship-Seasons',
+            'finder': ['First-Division', 'Championship'],
+        },
+        ##############################################
+        # Men's domestic league - 3rd tier and lower #
+        ##############################################
+        #######################
+        # Men's domestic cups #
+        #######################
+        #########################################
+        # Women's internation club competitions #
+        #########################################
+        'Women Champions League': {
+            'first valid year': 2015,
+            'url': 'https://fbref.com/en/comps/181/history/Champions-League-Seasons',
+            'finder': ['Champions-League'],
+        },
+        ######################################
+        # Women's national team competitions #
+        ######################################
+        'Womens World Cup': {
+            'first valid year': 1991,
+            'url': 'https://fbref.com/en/comps/106/history/Womens-World-Cup-Seasons',
+            'finder': ['Womens-World-Cup'],
+        },
+        'Womens Euros': {
+            'first valid year': 2001,
+            'url': 'https://fbref.com/en/comps/162/history/UEFA-Womens-Euro-Seasons',
+            'finder': ['UEFA-Womens-Euro'],
+        },
+        ############################
+        # Women's domestic leagues #
+        ############################
+        'NWSL': {
+            'first valid year': 2013,
+            'url': 'https://fbref.com/en/comps/182/history/NWSL-Seasons',
+            'finder': ['NWSL'],
+        },
+        'A-League Women': {
+            'first valid year': 2019,
+            'url': 'https://fbref.com/en/comps/196/history/A-League-Women-Seasons',
+            'finder': ['A-League-Women', 'W-League'],
+        },
+        'WSL': {
+            'first valid year': 2017,
+            'url': 'https://fbref.com/en/comps/189/history/Womens-Super-League-Seasons',
+            'finder': ['Womens-Super-League'],
+        },
+        'D1 Feminine': {
+            'first valid year': 2018,
+            'url': 'https://fbref.com/en/comps/193/history/Division-1-Feminine-Seasons',
+            'finder': ['Division-1-Feminine'],
+        },
+        'Womens Bundesliga': {
+            'first valid year': 2017,
+            'url': 'https://fbref.com/en/comps/183/history/Frauen-Bundesliga-Seasons',
+            'finder': ['Frauen-Bundesliga'],
+        },
+        'Womens Serie A': {
+            'first valid year': 2019,
+            'url': 'https://fbref.com/en/comps/208/history/Serie-A-Seasons',
+            'finder': ['Serie-A'],
+        },
+        'Liga F': {
+            'first valid year': 2023,
+            'url': 'https://fbref.com/en/comps/230/history/Liga-F-Seasons',
+            'finder': ['Liga-F'],
+        },
+        #########################
+        # Women's domestic cups #
+        #########################
+        'NWSL Challenge Cup': {
+            'first valid year': 2020,
+            'url': 'https://fbref.com/en/comps/881/history/NWSL-Challenge-Cup-Seasons',
+            'finder': ['NWSL-Challenge-Cup'],
+        },
+        'NWSL Fall Series': {
+            'first valid year': 2020,
+            'url': 'https://fbref.com/en/comps/884/history/NWSL-Fall-Series-Seasons',
+            'finder': ['NWSL-Fall-Series'],
+        },
+    },
+    'Understat': {
+        'EPL': {'first valid year': 2015,},
+        'La Liga': {'first valid year': 2015,},
+        'Bundesliga':  {'first valid year': 2015,},
+        'Serie A':  {'first valid year': 2015,},
+        'Ligue 1':  {'first valid year': 2015,},
+    },
+    'FiveThirtyEight': {
+        'EPL':  {'first valid year': 2017,},
+        'La Liga':  {'first valid year': 2017,},
+        'Bundesliga':  {'first valid year': 2017,},
+        'Serie A':  {'first valid year': 2017,},
+        'Ligue 1':  {'first valid year': 2017,},
+    },
+    'SofaScore': {'USL League One':  {'first valid year': 2019,}},
+    'Capology': {
+        'Bundesliga':  {'first valid year': 2014,},
+        '2.Bundesliga':  {'first valid year': 2020,},
+        'EPL':  {'first valid year': 2014,},
+        'EFL Championship':  {'first valid year': 2014,},
+        'Serie A':  {'first valid year': 2010,},
+        'Serie B':  {'first valid year': 2020,},
+        'La Liga':  {'first valid year': 2014,},
+        'La Liga 2':  {'first valid year': 2020,},
+        'Ligue 1':  {'first valid year': 2014,},
+        'Ligue 2':  {'first valid year': 2020,},
+        'Eredivisie':  {'first valid year': 2014,},
+        'Primeira Liga':  {'first valid year': 2014,},
+        'Scottish PL':  {'first valid year': 2020,},
+        'Super Lig':  {'first valid year': 2014,},
+        'Belgian 1st Division':  {'first valid year': 2014,},
+    },
+    'Transfermarkt': {
+        'EPL':  {'first valid year': 1993,},
+        'EFL Championship': {'first valid year': 2005,},
+        'EFL1': {'first valid year': 2005,},
+        'EFL2': {'first valid year': 2005,},
+        'Bundesliga': {'first valid year': 1964,},
+        '2.Bundesliga': {'first valid year': 1982,},
+        'Serie A': {'first valid year': 1930,},
+        'Serie B': {'first valid year': 1930,},
+        'La Liga': {'first valid year': 1929,},
+        'La Liga 2': {'first valid year': 1929,},
+        'Ligue 1': {'first valid year': 1970,},
+        'Ligue 2': {'first valid year': 1993,},
+        'Eredivisie': {'first valid year': 1955,},
+        'Scottish PL': {'first valid year': 2004,},
+        'Super Lig': {'first valid year': 1960,},
+        'Jupiler Pro League': {'first valid year': 1987,},
+        'Liga Nos': {'first valid year': 1994,},
+        'Russian Premier League': {'first valid year': 2011,},
+        'Brasileirao': {'first valid year': 2001,},
+        'Argentina Liga Profesional': {'first valid year': 2015,},
+        'MLS': {'first valid year': 1996,},
+    },
+}
+
+########################################################################################################################
+class InvalidSourceException(Exception):
+    ''' Raised when an invalid source is used with the check_season() function.
+    '''
+    def __init__(self, source):
+        super().__init__()
+        self.source = source
+    def __str__(self):
+        return f'{self.source} is not a valid source. Must be one of {list(sources.keys())}.'
+
+########################################################################################################################
+class InvalidLeagueException(Exception):
+    ''' Raised when an invalid league is used with the check_season() function.
+    '''
+    def __init__(self, league, source):
+        super().__init__()
+        self.league = league
+        self.source = source
+    def __str__(self):
+        return f'{self.league} is not a valid league for {self.source}. Options are {list(sources[self.source].keys())}.'
+
+########################################################################################################################
+class InvalidYearException(Exception):
+    ''' Raised when an invalid year is used with the check_season() function.
+    '''
+    def __init__(self, year, league, source):
+        super().__init__()
+        self.year = year
+        self.league = league
+        self.source = source
+    def __str__(self):
+        return f'{self.year} invalid for source {self.source} and league {self.league}. ' +\
+            f'Must be {sources[self.source][self.league]["first valid year"]} or later.'
+
+########################################################################################################################
+class InvalidCurrencyException(Exception):
+    ''' Raised when an invalid currency is used with the Capology module.
+    '''
+    def __init__(self):
+        super().__init__()
+    def __str__():
+        return 'Currency must be one of "eur", "gbp", or "usd".'
+
+########################################################################################################################
+class UnavailableSeasonException(Exception):
+    ''' Raised when a given year and league is unavailable from a source.
+    '''
+    def __init__(self, year, league, source):
+        super().__init__()
+        self.year = year
+        self.league = league
+        self.source = source
+    def __str__(self):
+        return f'No {self.league} {self.year} season is available on {self.source}.'
+
+########################################################################################################################
+class NoMatchLinksException(Exception):
+    ''' Raised when no match links are found
+    '''
+    def __init__(self, fixtures_url, year, league):
+        super().__init__()
+        self.fixtures_url = fixtures_url
+        self.league = league
+        self.year = year
+    def __str__(self):
+        return f'No match score elements with links found at {self.fixtures_url} for {self.year} {self.league}.'
+
+########################################################################################################################
+def check_season(year, league, source):
+    ''' Checks to make sure that the given league season is a valid season for the scraper.
+    
+    Args
+    ----
+    year : int
+        Calendar year that the season ends in (e.g. 2023 for the 2022/23 season)
+    league : str
+        League. Look in shared_functions.py for the available leagues for each\
+        module.
+    source : str
+        The scraper to be checked (e.g. 'FBRef', 'Transfermarkt, etc.). These\
+        are the ScraperFC modules.
+    Returns
+    -------
+    err : str
+        String of the error message, if there is one.
+    valid : bool
+        True if the league season is valid for the scraper. False otherwise.
+    '''
+    # Check source
+    if source not in list(sources.keys()):
+        raise InvalidSourceException(source)
+
+    # Check league
+    if type(league)!=str:
+        raise TypeError('League must be a string.')
+    if league not in list(sources[source].keys()):
+        raise InvalidLeagueException(league, source)
+    
+    # Check year
+    if type(year) != int:
+        raise TypeError('Year must be an integer.')
+    if year < sources[source][league]['first valid year']:
+        raise InvalidYearException(year, league, source)
+    
+    return
+
+########################################################################################################################
+def get_proxy():
+    ''' Gets a proxy address.
+
+    Can be used to initialize a Selenium WebDriver to change the address of the\
+    browser. Adapted from https://stackoverflow.com/questions/59409418/how-to-rotate-selenium-webrowser-ip-address.\
+    Randomly chooses one proxy.
+    
+    Returns
+    -------
+    proxy : str
+        In the form <IP address>:<port>
+    '''
+    options = Options()
+    options.headless = True
+    options.add_argument('window-size=700,600')
+    driver = webdriver.Chrome(ChromeDriverManager().install(), options=options)
+    clear_output()
+    
+    try:
+        driver.get('https://sslproxies.org/')
+        table = driver.find_elements(By.TAG_NAME, 'table')[0]
+        df = pd.read_html(table.get_attribute('outerHTML'))[0]
+        df = df.iloc[np.where(~np.isnan(df['Port']))[0],:] # ignore nans
+
+        ips = df['IP Address'].values
+        ports = df['Port'].astype('int').values
+
+        driver.quit()
+        proxies = list()
+        for i in range(len(ips)):
+            proxies.append('{}:{}'.format(ips[i], ports[i]))
+        i = random.randint(0, len(proxies)-1)
+        return proxies[i]
+    except Exception as e:
+        driver.close()
+        driver.quit()
+        raise e
+        
+########################################################################################################################
+def xpath_soup(element):
+    ''' Generate xpath from BeautifulSoup4 element.
+    
+    I shamelessly stole this from https://gist.github.com/ergoithz/6cf043e3fdedd1b94fcf.
+    
+    Args
+    ----
+    element : bs4.element.Tag or bs4.element.NavigableString
+        BeautifulSoup4 element.
+    Returns
+    -------
+    : str
+        xpath as string
+    Usage
+    -----
+    >>> import bs4
+    >>> html = (
+    ...     '<html><head><title>title</title></head>'
+    ...     '<body><p>p <i>1</i></p><p>p <i>2</i></p></body></html>'
+    ...     )
+    >>> soup = bs4.BeautifulSoup(html, 'html.parser')
+    >>> xpath_soup(soup.html.body.p.i)
+    '/html/body/p[1]/i'
+    >>> import bs4
+    >>> xml = '<doc><elm/><elm/></doc>'
+    >>> soup = bs4.BeautifulSoup(xml, 'lxml-xml')
+    >>> xpath_soup(soup.doc.elm.next_sibling)
+    '/doc/elm[2]'
+    '''
+    components = []
+    child = element if element.name else element.parent
+    for parent in child.parents:  # type: bs4.element.Tag
+        siblings = parent.find_all(child.name, recursive=False)
+        components.append(
+            child.name if 1 == len(siblings) else '%s[%d]' % (
+                child.name,
+                next(i for i, s in enumerate(siblings, 1) if s is child)
+                )
+            )
+        child = parent
+    components.reverse()
+    return '/%s' % '/'.join(components)
```

### Comparing `ScraperFC-2.6.5/ScraperFC.egg-info/PKG-INFO` & `ScraperFC-2.7.0/ScraperFC.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-Metadata-Version: 2.1
-Name: ScraperFC
-Version: 2.6.5
-Summary: Package for scraping soccer data from a variety of sources.
-Home-page: https://github.com/oseymour/ScraperFC
-Author: Owen Seymour
-Author-email: osmour043@gmail.com
-Keywords: soccer,football,Premier League,Serie A,La Liga,Bundesliga,Ligue 1,web scraping,soccer data,soccer stats,football data,football stats,web scraping soccer stats,web scraping football stats,web scraping soccer data,web scraping football data
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<p align="center">
-  <img src="https://github.com/oseymour/ScraperFC/blob/main/scraperfc_logo.png?raw=true" alt="ScraperFC logo. The underlined text ScraperFC, where the circle of the p is a soccer ball.">
-</p>
-<p align="center">
-  <a href="https://pypi.org/project/ScraperFC/"><img src="https://img.shields.io/pypi/v/scraperfc.svg", alt="pypi version badge"></a>
-  <a href="https://pypi.org/project/ScraperFC/"><img src="https://static.pepy.tech/badge/scraperfc" alt="total pypi downloads badge"/></a>
-  <a href="https://pypi.org/project/ScraperFC/"><img src="https://img.shields.io/pypi/dm/ScraperFC.svg" alt="monthly pypi downloads badge"/></a>
-  <a href="https://pypi.org/project/ScraperFC/"><img src="https://img.shields.io/pypi/dw/ScraperFC.svg" alt="weekly pypi downloads badge"/></a>
-  <a href="https://pypi.org/project/ScraperFC/"><img src="https://img.shields.io/pypi/dd/ScraperFC.svg" alt="dailypypi downloads badge"/></a>
-  <a href="https://scraperfc.readthedocs.io/en/latest/"><img src="https://readthedocs.org/projects/nrc4d/badge/?version=latest" alt="documentation status badge"/></a>
-  <a href="https://github.com/oseymour/ScraperFC"><img src="http://hits.dwyl.com/oseymour/scraperfc.svg?style=flat"></a>
-</p>
-
-This is ScraperFC, a Python package that I hope will give more people access to soccer data. Gone are the days of downloading spreadsheets one-by-one, copy-pasting, or entering data into spreadsheets by hand. I try to make ScraperFC as easy-to-use as possible so that anybody with a bit of Python experience can use it.
-
-To install ScraperFC, run ```pip install ScraperFC``` from the command line.
-
-Data can be scraped from the following sources:
-* [FBRef](https://fbref.com/en/)
-* [Understat](https://understat.com/)
-* [FiveThirtyEight](https://projects.fivethirtyeight.com/soccer-predictions/)
-* [ClubELO](http://clubelo.com/)
-* [Capology](https://www.capology.com/)
-* [Transfermarkt](https://www.transfermarkt.us/)
-
-For documentation, head over to the [Read the Docs page](https://scraperfc.readthedocs.io).
-
-For usage examples, look at Examples.ipynb in the top level directory or some of my example analyses in the analytics_examples folder.
-
-I'd love to hear your feedback, bugs you find, or new features you want! The best way is to open an issue on this repository and I can respond to it there. Otherwise, you can reach me via email at osmour043@gmail.com or my Twitter handle is [@owen_seymour](https://twitter.com/owen_seymour).
+Metadata-Version: 2.1
+Name: ScraperFC
+Version: 2.7.0
+Summary: Package for scraping soccer data from a variety of sources.
+Home-page: https://github.com/oseymour/ScraperFC
+Author: Owen Seymour
+Author-email: osmour043@gmail.com
+Keywords: soccer,football,Premier League,Serie A,La Liga,Bundesliga,Ligue 1,web scraping,soccer data,soccer stats,football data,football stats,web scraping soccer stats,web scraping football stats,web scraping soccer data,web scraping football data
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="center">
+  <img src="https://github.com/oseymour/ScraperFC/blob/main/scraperfc_logo.png?raw=true" alt="ScraperFC logo. The underlined text ScraperFC, where the circle of the p is a soccer ball.">
+</p>
+<p align="center">
+  <a href="https://pypi.org/project/ScraperFC/"><img src="https://img.shields.io/pypi/v/scraperfc.svg", alt="pypi version badge"></a>
+  <a href="https://pypi.org/project/ScraperFC/"><img src="https://static.pepy.tech/badge/scraperfc" alt="total pypi downloads badge"/></a>
+  <a href="https://pypi.org/project/ScraperFC/"><img src="https://img.shields.io/pypi/dm/ScraperFC.svg" alt="monthly pypi downloads badge"/></a>
+  <a href="https://pypi.org/project/ScraperFC/"><img src="https://img.shields.io/pypi/dw/ScraperFC.svg" alt="weekly pypi downloads badge"/></a>
+  <a href="https://pypi.org/project/ScraperFC/"><img src="https://img.shields.io/pypi/dd/ScraperFC.svg" alt="dailypypi downloads badge"/></a>
+  <a href="https://scraperfc.readthedocs.io/en/latest/"><img src="https://readthedocs.org/projects/nrc4d/badge/?version=latest" alt="documentation status badge"/></a>
+  <a href="https://github.com/oseymour/ScraperFC"><img src="http://hits.dwyl.com/oseymour/scraperfc.svg?style=flat"></a>
+</p>
+
+This is ScraperFC, a Python package that I hope will give more people access to soccer data. Gone are the days of downloading spreadsheets one-by-one, copy-pasting, or entering data into spreadsheets by hand. I try to make ScraperFC as easy-to-use as possible so that anybody with a bit of Python experience can use it.
+
+To install ScraperFC, run ```pip install ScraperFC``` from the command line.
+
+Data can be scraped from the following sources:
+* [FBRef](https://fbref.com/en/)
+* [Understat](https://understat.com/)
+* [FiveThirtyEight](https://projects.fivethirtyeight.com/soccer-predictions/)
+* [ClubELO](http://clubelo.com/)
+* [Capology](https://www.capology.com/)
+* [Transfermarkt](https://www.transfermarkt.us/)
+
+For documentation, head over to the [Read the Docs page](https://scraperfc.readthedocs.io).
+
+For usage examples, look at Examples.ipynb in the top level directory or some of my example analyses in the analytics_examples folder.
+
+I'd love to hear your feedback, bugs you find, or new features you want! The best way is to open an issue on this repository and I can respond to it there. Otherwise, you can reach me via email at osmour043@gmail.com or my Twitter handle is [@owen_seymour](https://twitter.com/owen_seymour).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ScraperFC Version: 2.6.5 Summary: Package for
+Metadata-Version: 2.1 Name: ScraperFC Version: 2.7.0 Summary: Package for
 scraping soccer data from a variety of sources. Home-page: https://github.com/
 oseymour/ScraperFC Author: Owen Seymour Author-email: osmour043@gmail.com
 Keywords: soccer,football,Premier League,Serie A,La Liga,Bundesliga,Ligue 1,web
 scraping,soccer data,soccer stats,football data,football stats,web scraping
 soccer stats,web scraping football stats,web scraping soccer data,web scraping
 football data Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
```

### Comparing `ScraperFC-2.6.5/setup.py` & `ScraperFC-2.7.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-import setuptools
-
-with open("README.md", "r", encoding="utf-8") as f:
-    long_description = f.read()
-    
-setuptools.setup(
-    name = "ScraperFC",
-    version = '2.6.5',
-    author = "Owen Seymour",
-    author_email = 'osmour043@gmail.com',
-    description = 'Package for scraping soccer data from a variety of sources.',
-    long_description = long_description,
-    long_description_content_type = 'text/markdown',
-    url = 'https://github.com/oseymour/ScraperFC',
-    packages = ['ScraperFC',],
-    keywords = [
-        'soccer', 'football', 'Premier League', 'Serie A', 'La Liga', 
-        'Bundesliga', 'Ligue 1', 'web scraping', 'soccer data', 
-        'soccer stats', 'football data', 'football stats',
-        'web scraping soccer stats', 'web scraping football stats',
-        'web scraping soccer data', 'web scraping football data',
-    ],
-    install_requires = [
-        'selenium', 'webdriver-manager', 'pandas', 'numpy', 'datetime',
-        'ipython', 'requests', 'bs4', 'lxml', 'tqdm',
-    ],
-    classifiers = [
-        'Programming Language :: Python :: 3',
-        'Operating System :: OS Independent'
-    ],
-    python_requires = '>=3.6'
-)
+import setuptools
+
+with open("README.md", "r", encoding="utf-8") as f:
+    long_description = f.read()
+    
+setuptools.setup(
+    name = "ScraperFC",
+    version = '2.7.0',
+    author = "Owen Seymour",
+    author_email = 'osmour043@gmail.com',
+    description = 'Package for scraping soccer data from a variety of sources.',
+    long_description = long_description,
+    long_description_content_type = 'text/markdown',
+    url = 'https://github.com/oseymour/ScraperFC',
+    packages = ['ScraperFC',],
+    keywords = [
+        'soccer', 'football', 'Premier League', 'Serie A', 'La Liga', 
+        'Bundesliga', 'Ligue 1', 'web scraping', 'soccer data', 
+        'soccer stats', 'football data', 'football stats',
+        'web scraping soccer stats', 'web scraping football stats',
+        'web scraping soccer data', 'web scraping football data',
+    ],
+    install_requires = [
+        'selenium', 'webdriver-manager', 'pandas', 'numpy', 'datetime',
+        'ipython', 'requests', 'bs4', 'lxml', 'tqdm',
+    ],
+    classifiers = [
+        'Programming Language :: Python :: 3',
+        'Operating System :: OS Independent'
+    ],
+    python_requires = '>=3.6'
+)
```

