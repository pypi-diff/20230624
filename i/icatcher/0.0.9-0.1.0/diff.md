# Comparing `tmp/icatcher-0.0.9.tar.gz` & `tmp/icatcher-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icatcher-0.0.9.tar", last modified: Tue Mar 21 02:00:23 2023, max compression
+gzip compressed data, was "icatcher-0.1.0.tar", last modified: Fri Jun 23 23:08:01 2023, max compression
```

## Comparing `icatcher-0.0.9.tar` & `icatcher-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-03-21 02:00:23.598953 icatcher-0.0.9/
--rw-rw-rw-   0        0        0    35823 2022-08-25 04:26:17.000000 icatcher-0.0.9/LICENSE
--rw-rw-rw-   0        0        0    51909 2023-03-21 02:00:23.598953 icatcher-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0    10122 2023-03-09 09:36:40.000000 icatcher-0.0.9/README.md
--rw-rw-rw-   0        0        0     1328 2023-03-21 01:40:11.000000 icatcher-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-21 02:00:23.598953 icatcher-0.0.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-21 02:00:23.529161 icatcher-0.0.9/src/
-drwxrwxrwx   0        0        0        0 2023-03-21 02:00:23.579135 icatcher-0.0.9/src/icatcher/
--rw-rw-rw-   0        0        0       44 2023-03-21 01:40:11.000000 icatcher-0.0.9/src/icatcher/__init__.py
--rw-rw-rw-   0        0        0    25796 2023-03-21 01:54:19.000000 icatcher-0.0.9/src/icatcher/cli.py
--rw-rw-rw-   0        0        0     4685 2023-03-10 04:48:55.000000 icatcher-0.0.9/src/icatcher/draw.py
--rw-rw-rw-   0        0        0     4733 2023-02-02 10:55:03.000000 icatcher-0.0.9/src/icatcher/models.py
--rw-rw-rw-   0        0        0     6610 2023-03-21 01:37:17.000000 icatcher-0.0.9/src/icatcher/options.py
--rw-rw-rw-   0        0        0      911 2023-02-02 10:31:25.000000 icatcher-0.0.9/src/icatcher/parsers.py
--rw-rw-rw-   0        0        0     2016 2023-02-02 12:15:34.000000 icatcher-0.0.9/src/icatcher/video.py
-drwxrwxrwx   0        0        0        0 2023-03-21 02:00:23.589219 icatcher-0.0.9/src/icatcher.egg-info/
--rw-rw-rw-   0        0        0    51909 2023-03-21 02:00:23.000000 icatcher-0.0.9/src/icatcher.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-03-21 02:00:23.000000 icatcher-0.0.9/src/icatcher.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-21 02:00:23.000000 icatcher-0.0.9/src/icatcher.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-03-21 02:00:23.000000 icatcher-0.0.9/src/icatcher.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      122 2023-03-21 02:00:23.000000 icatcher-0.0.9/src/icatcher.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-21 02:00:23.000000 icatcher-0.0.9/src/icatcher.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-21 02:00:23.598953 icatcher-0.0.9/tests/
--rw-rw-rw-   0        0        0      425 2023-03-14 15:02:09.000000 icatcher-0.0.9/tests/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:08:01.980412 icatcher-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-23 23:05:42.000000 icatcher-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    47847 2023-06-23 23:08:01.980412 icatcher-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-06-23 23:05:42.000000 icatcher-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-23 23:05:42.000000 icatcher-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 23:08:01.980412 icatcher-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:08:01.976412 icatcher-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:08:01.976412 icatcher-0.1.0/src/icatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-23 23:05:42.000000 icatcher-0.1.0/src/icatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23510 2023-06-23 23:05:42.000000 icatcher-0.1.0/src/icatcher/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-06-23 23:05:42.000000 icatcher-0.1.0/src/icatcher/draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-06-23 23:05:42.000000 icatcher-0.1.0/src/icatcher/face_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-06-23 23:05:42.000000 icatcher-0.1.0/src/icatcher/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8534 2023-06-23 23:05:42.000000 icatcher-0.1.0/src/icatcher/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-23 23:05:42.000000 icatcher-0.1.0/src/icatcher/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-06-23 23:05:42.000000 icatcher-0.1.0/src/icatcher/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:08:01.980412 icatcher-0.1.0/src/icatcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    47847 2023-06-23 23:08:01.000000 icatcher-0.1.0/src/icatcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-23 23:08:01.000000 icatcher-0.1.0/src/icatcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 23:08:01.000000 icatcher-0.1.0/src/icatcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-23 23:08:01.000000 icatcher-0.1.0/src/icatcher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-23 23:08:01.000000 icatcher-0.1.0/src/icatcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-23 23:08:01.000000 icatcher-0.1.0/src/icatcher.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:08:01.980412 icatcher-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-23 23:05:42.000000 icatcher-0.1.0/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-06-23 23:05:42.000000 icatcher-0.1.0/tests/test_face_detector.py
```

### Comparing `icatcher-0.0.9/LICENSE` & `icatcher-0.1.0/LICENSE`

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

### Comparing `icatcher-0.0.9/PKG-INFO` & `icatcher-0.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,863 +1,813 @@
-Metadata-Version: 2.1
-Name: icatcher
-Version: 0.0.9
-Summary: iCatcher+: Robust and automated annotation of infant gaze from videos collected in laboratory, field, and online studies.
-Author-email: Yotam Erel <erelyotam@gmail.com>
-License:                     GNU GENERAL PUBLIC LICENSE
-                               Version 3, 29 June 2007
-        
-         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
-         Everyone is permitted to copy and distribute verbatim copies
-         of this license document, but changing it is not allowed.
-        
-                                    Preamble
-        
-          The GNU General Public License is a free, copyleft license for
-        software and other kinds of works.
-        
-          The licenses for most software and other practical works are designed
-        to take away your freedom to share and change the works.  By contrast,
-        the GNU General Public License is intended to guarantee your freedom to
-        share and change all versions of a program--to make sure it remains free
-        software for all its users.  We, the Free Software Foundation, use the
-        GNU General Public License for most of our software; it applies also to
-        any other work released this way by its authors.  You can apply it to
-        your programs, too.
-        
-          When we speak of free software, we are referring to freedom, not
-        price.  Our General Public Licenses are designed to make sure that you
-        have the freedom to distribute copies of free software (and charge for
-        them if you wish), that you receive source code or can get it if you
-        want it, that you can change the software or use pieces of it in new
-        free programs, and that you know you can do these things.
-        
-          To protect your rights, we need to prevent others from denying you
-        these rights or asking you to surrender the rights.  Therefore, you have
-        certain responsibilities if you distribute copies of the software, or if
-        you modify it: responsibilities to respect the freedom of others.
-        
-          For example, if you distribute copies of such a program, whether
-        gratis or for a fee, you must pass on to the recipients the same
-        freedoms that you received.  You must make sure that they, too, receive
-        or can get the source code.  And you must show them these terms so they
-        know their rights.
-        
-          Developers that use the GNU GPL protect your rights with two steps:
-        (1) assert copyright on the software, and (2) offer you this License
-        giving you legal permission to copy, distribute and/or modify it.
-        
-          For the developers' and authors' protection, the GPL clearly explains
-        that there is no warranty for this free software.  For both users' and
-        authors' sake, the GPL requires that modified versions be marked as
-        changed, so that their problems will not be attributed erroneously to
-        authors of previous versions.
-        
-          Some devices are designed to deny users access to install or run
-        modified versions of the software inside them, although the manufacturer
-        can do so.  This is fundamentally incompatible with the aim of
-        protecting users' freedom to change the software.  The systematic
-        pattern of such abuse occurs in the area of products for individuals to
-        use, which is precisely where it is most unacceptable.  Therefore, we
-        have designed this version of the GPL to prohibit the practice for those
-        products.  If such problems arise substantially in other domains, we
-        stand ready to extend this provision to those domains in future versions
-        of the GPL, as needed to protect the freedom of users.
-        
-          Finally, every program is threatened constantly by software patents.
-        States should not allow patents to restrict development and use of
-        software on general-purpose computers, but in those that do, we wish to
-        avoid the special danger that patents applied to a free program could
-        make it effectively proprietary.  To prevent this, the GPL assures that
-        patents cannot be used to render the program non-free.
-        
-          The precise terms and conditions for copying, distribution and
-        modification follow.
-        
-                               TERMS AND CONDITIONS
-        
-          0. Definitions.
-        
-          "This License" refers to version 3 of the GNU General Public License.
-        
-          "Copyright" also means copyright-like laws that apply to other kinds of
-        works, such as semiconductor masks.
-        
-          "The Program" refers to any copyrightable work licensed under this
-        License.  Each licensee is addressed as "you".  "Licensees" and
-        "recipients" may be individuals or organizations.
-        
-          To "modify" a work means to copy from or adapt all or part of the work
-        in a fashion requiring copyright permission, other than the making of an
-        exact copy.  The resulting work is called a "modified version" of the
-        earlier work or a work "based on" the earlier work.
-        
-          A "covered work" means either the unmodified Program or a work based
-        on the Program.
-        
-          To "propagate" a work means to do anything with it that, without
-        permission, would make you directly or secondarily liable for
-        infringement under applicable copyright law, except executing it on a
-        computer or modifying a private copy.  Propagation includes copying,
-        distribution (with or without modification), making available to the
-        public, and in some countries other activities as well.
-        
-          To "convey" a work means any kind of propagation that enables other
-        parties to make or receive copies.  Mere interaction with a user through
-        a computer network, with no transfer of a copy, is not conveying.
-        
-          An interactive user interface displays "Appropriate Legal Notices"
-        to the extent that it includes a convenient and prominently visible
-        feature that (1) displays an appropriate copyright notice, and (2)
-        tells the user that there is no warranty for the work (except to the
-        extent that warranties are provided), that licensees may convey the
-        work under this License, and how to view a copy of this License.  If
-        the interface presents a list of user commands or options, such as a
-        menu, a prominent item in the list meets this criterion.
-        
-          1. Source Code.
-        
-          The "source code" for a work means the preferred form of the work
-        for making modifications to it.  "Object code" means any non-source
-        form of a work.
-        
-          A "Standard Interface" means an interface that either is an official
-        standard defined by a recognized standards body, or, in the case of
-        interfaces specified for a particular programming language, one that
-        is widely used among developers working in that language.
-        
-          The "System Libraries" of an executable work include anything, other
-        than the work as a whole, that (a) is included in the normal form of
-        packaging a Major Component, but which is not part of that Major
-        Component, and (b) serves only to enable use of the work with that
-        Major Component, or to implement a Standard Interface for which an
-        implementation is available to the public in source code form.  A
-        "Major Component", in this context, means a major essential component
-        (kernel, window system, and so on) of the specific operating system
-        (if any) on which the executable work runs, or a compiler used to
-        produce the work, or an object code interpreter used to run it.
-        
-          The "Corresponding Source" for a work in object code form means all
-        the source code needed to generate, install, and (for an executable
-        work) run the object code and to modify the work, including scripts to
-        control those activities.  However, it does not include the work's
-        System Libraries, or general-purpose tools or generally available free
-        programs which are used unmodified in performing those activities but
-        which are not part of the work.  For example, Corresponding Source
-        includes interface definition files associated with source files for
-        the work, and the source code for shared libraries and dynamically
-        linked subprograms that the work is specifically designed to require,
-        such as by intimate data communication or control flow between those
-        subprograms and other parts of the work.
-        
-          The Corresponding Source need not include anything that users
-        can regenerate automatically from other parts of the Corresponding
-        Source.
-        
-          The Corresponding Source for a work in source code form is that
-        same work.
-        
-          2. Basic Permissions.
-        
-          All rights granted under this License are granted for the term of
-        copyright on the Program, and are irrevocable provided the stated
-        conditions are met.  This License explicitly affirms your unlimited
-        permission to run the unmodified Program.  The output from running a
-        covered work is covered by this License only if the output, given its
-        content, constitutes a covered work.  This License acknowledges your
-        rights of fair use or other equivalent, as provided by copyright law.
-        
-          You may make, run and propagate covered works that you do not
-        convey, without conditions so long as your license otherwise remains
-        in force.  You may convey covered works to others for the sole purpose
-        of having them make modifications exclusively for you, or provide you
-        with facilities for running those works, provided that you comply with
-        the terms of this License in conveying all material for which you do
-        not control copyright.  Those thus making or running the covered works
-        for you must do so exclusively on your behalf, under your direction
-        and control, on terms that prohibit them from making any copies of
-        your copyrighted material outside their relationship with you.
-        
-          Conveying under any other circumstances is permitted solely under
-        the conditions stated below.  Sublicensing is not allowed; section 10
-        makes it unnecessary.
-        
-          3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-        
-          No covered work shall be deemed part of an effective technological
-        measure under any applicable law fulfilling obligations under article
-        11 of the WIPO copyright treaty adopted on 20 December 1996, or
-        similar laws prohibiting or restricting circumvention of such
-        measures.
-        
-          When you convey a covered work, you waive any legal power to forbid
-        circumvention of technological measures to the extent such circumvention
-        is effected by exercising rights under this License with respect to
-        the covered work, and you disclaim any intention to limit operation or
-        modification of the work as a means of enforcing, against the work's
-        users, your or third parties' legal rights to forbid circumvention of
-        technological measures.
-        
-          4. Conveying Verbatim Copies.
-        
-          You may convey verbatim copies of the Program's source code as you
-        receive it, in any medium, provided that you conspicuously and
-        appropriately publish on each copy an appropriate copyright notice;
-        keep intact all notices stating that this License and any
-        non-permissive terms added in accord with section 7 apply to the code;
-        keep intact all notices of the absence of any warranty; and give all
-        recipients a copy of this License along with the Program.
-        
-          You may charge any price or no price for each copy that you convey,
-        and you may offer support or warranty protection for a fee.
-        
-          5. Conveying Modified Source Versions.
-        
-          You may convey a work based on the Program, or the modifications to
-        produce it from the Program, in the form of source code under the
-        terms of section 4, provided that you also meet all of these conditions:
-        
-            a) The work must carry prominent notices stating that you modified
-            it, and giving a relevant date.
-        
-            b) The work must carry prominent notices stating that it is
-            released under this License and any conditions added under section
-            7.  This requirement modifies the requirement in section 4 to
-            "keep intact all notices".
-        
-            c) You must license the entire work, as a whole, under this
-            License to anyone who comes into possession of a copy.  This
-            License will therefore apply, along with any applicable section 7
-            additional terms, to the whole of the work, and all its parts,
-            regardless of how they are packaged.  This License gives no
-            permission to license the work in any other way, but it does not
-            invalidate such permission if you have separately received it.
-        
-            d) If the work has interactive user interfaces, each must display
-            Appropriate Legal Notices; however, if the Program has interactive
-            interfaces that do not display Appropriate Legal Notices, your
-            work need not make them do so.
-        
-          A compilation of a covered work with other separate and independent
-        works, which are not by their nature extensions of the covered work,
-        and which are not combined with it such as to form a larger program,
-        in or on a volume of a storage or distribution medium, is called an
-        "aggregate" if the compilation and its resulting copyright are not
-        used to limit the access or legal rights of the compilation's users
-        beyond what the individual works permit.  Inclusion of a covered work
-        in an aggregate does not cause this License to apply to the other
-        parts of the aggregate.
-        
-          6. Conveying Non-Source Forms.
-        
-          You may convey a covered work in object code form under the terms
-        of sections 4 and 5, provided that you also convey the
-        machine-readable Corresponding Source under the terms of this License,
-        in one of these ways:
-        
-            a) Convey the object code in, or embodied in, a physical product
-            (including a physical distribution medium), accompanied by the
-            Corresponding Source fixed on a durable physical medium
-            customarily used for software interchange.
-        
-            b) Convey the object code in, or embodied in, a physical product
-            (including a physical distribution medium), accompanied by a
-            written offer, valid for at least three years and valid for as
-            long as you offer spare parts or customer support for that product
-            model, to give anyone who possesses the object code either (1) a
-            copy of the Corresponding Source for all the software in the
-            product that is covered by this License, on a durable physical
-            medium customarily used for software interchange, for a price no
-            more than your reasonable cost of physically performing this
-            conveying of source, or (2) access to copy the
-            Corresponding Source from a network server at no charge.
-        
-            c) Convey individual copies of the object code with a copy of the
-            written offer to provide the Corresponding Source.  This
-            alternative is allowed only occasionally and noncommercially, and
-            only if you received the object code with such an offer, in accord
-            with subsection 6b.
-        
-            d) Convey the object code by offering access from a designated
-            place (gratis or for a charge), and offer equivalent access to the
-            Corresponding Source in the same way through the same place at no
-            further charge.  You need not require recipients to copy the
-            Corresponding Source along with the object code.  If the place to
-            copy the object code is a network server, the Corresponding Source
-            may be on a different server (operated by you or a third party)
-            that supports equivalent copying facilities, provided you maintain
-            clear directions next to the object code saying where to find the
-            Corresponding Source.  Regardless of what server hosts the
-            Corresponding Source, you remain obligated to ensure that it is
-            available for as long as needed to satisfy these requirements.
-        
-            e) Convey the object code using peer-to-peer transmission, provided
-            you inform other peers where the object code and Corresponding
-            Source of the work are being offered to the general public at no
-            charge under subsection 6d.
-        
-          A separable portion of the object code, whose source code is excluded
-        from the Corresponding Source as a System Library, need not be
-        included in conveying the object code work.
-        
-          A "User Product" is either (1) a "consumer product", which means any
-        tangible personal property which is normally used for personal, family,
-        or household purposes, or (2) anything designed or sold for incorporation
-        into a dwelling.  In determining whether a product is a consumer product,
-        doubtful cases shall be resolved in favor of coverage.  For a particular
-        product received by a particular user, "normally used" refers to a
-        typical or common use of that class of product, regardless of the status
-        of the particular user or of the way in which the particular user
-        actually uses, or expects or is expected to use, the product.  A product
-        is a consumer product regardless of whether the product has substantial
-        commercial, industrial or non-consumer uses, unless such uses represent
-        the only significant mode of use of the product.
-        
-          "Installation Information" for a User Product means any methods,
-        procedures, authorization keys, or other information required to install
-        and execute modified versions of a covered work in that User Product from
-        a modified version of its Corresponding Source.  The information must
-        suffice to ensure that the continued functioning of the modified object
-        code is in no case prevented or interfered with solely because
-        modification has been made.
-        
-          If you convey an object code work under this section in, or with, or
-        specifically for use in, a User Product, and the conveying occurs as
-        part of a transaction in which the right of possession and use of the
-        User Product is transferred to the recipient in perpetuity or for a
-        fixed term (regardless of how the transaction is characterized), the
-        Corresponding Source conveyed under this section must be accompanied
-        by the Installation Information.  But this requirement does not apply
-        if neither you nor any third party retains the ability to install
-        modified object code on the User Product (for example, the work has
-        been installed in ROM).
-        
-          The requirement to provide Installation Information does not include a
-        requirement to continue to provide support service, warranty, or updates
-        for a work that has been modified or installed by the recipient, or for
-        the User Product in which it has been modified or installed.  Access to a
-        network may be denied when the modification itself materially and
-        adversely affects the operation of the network or violates the rules and
-        protocols for communication across the network.
-        
-          Corresponding Source conveyed, and Installation Information provided,
-        in accord with this section must be in a format that is publicly
-        documented (and with an implementation available to the public in
-        source code form), and must require no special password or key for
-        unpacking, reading or copying.
-        
-          7. Additional Terms.
-        
-          "Additional permissions" are terms that supplement the terms of this
-        License by making exceptions from one or more of its conditions.
-        Additional permissions that are applicable to the entire Program shall
-        be treated as though they were included in this License, to the extent
-        that they are valid under applicable law.  If additional permissions
-        apply only to part of the Program, that part may be used separately
-        under those permissions, but the entire Program remains governed by
-        this License without regard to the additional permissions.
-        
-          When you convey a copy of a covered work, you may at your option
-        remove any additional permissions from that copy, or from any part of
-        it.  (Additional permissions may be written to require their own
-        removal in certain cases when you modify the work.)  You may place
-        additional permissions on material, added by you to a covered work,
-        for which you have or can give appropriate copyright permission.
-        
-          Notwithstanding any other provision of this License, for material you
-        add to a covered work, you may (if authorized by the copyright holders of
-        that material) supplement the terms of this License with terms:
-        
-            a) Disclaiming warranty or limiting liability differently from the
-            terms of sections 15 and 16 of this License; or
-        
-            b) Requiring preservation of specified reasonable legal notices or
-            author attributions in that material or in the Appropriate Legal
-            Notices displayed by works containing it; or
-        
-            c) Prohibiting misrepresentation of the origin of that material, or
-            requiring that modified versions of such material be marked in
-            reasonable ways as different from the original version; or
-        
-            d) Limiting the use for publicity purposes of names of licensors or
-            authors of the material; or
-        
-            e) Declining to grant rights under trademark law for use of some
-            trade names, trademarks, or service marks; or
-        
-            f) Requiring indemnification of licensors and authors of that
-            material by anyone who conveys the material (or modified versions of
-            it) with contractual assumptions of liability to the recipient, for
-            any liability that these contractual assumptions directly impose on
-            those licensors and authors.
-        
-          All other non-permissive additional terms are considered "further
-        restrictions" within the meaning of section 10.  If the Program as you
-        received it, or any part of it, contains a notice stating that it is
-        governed by this License along with a term that is a further
-        restriction, you may remove that term.  If a license document contains
-        a further restriction but permits relicensing or conveying under this
-        License, you may add to a covered work material governed by the terms
-        of that license document, provided that the further restriction does
-        not survive such relicensing or conveying.
-        
-          If you add terms to a covered work in accord with this section, you
-        must place, in the relevant source files, a statement of the
-        additional terms that apply to those files, or a notice indicating
-        where to find the applicable terms.
-        
-          Additional terms, permissive or non-permissive, may be stated in the
-        form of a separately written license, or stated as exceptions;
-        the above requirements apply either way.
-        
-          8. Termination.
-        
-          You may not propagate or modify a covered work except as expressly
-        provided under this License.  Any attempt otherwise to propagate or
-        modify it is void, and will automatically terminate your rights under
-        this License (including any patent licenses granted under the third
-        paragraph of section 11).
-        
-          However, if you cease all violation of this License, then your
-        license from a particular copyright holder is reinstated (a)
-        provisionally, unless and until the copyright holder explicitly and
-        finally terminates your license, and (b) permanently, if the copyright
-        holder fails to notify you of the violation by some reasonable means
-        prior to 60 days after the cessation.
-        
-          Moreover, your license from a particular copyright holder is
-        reinstated permanently if the copyright holder notifies you of the
-        violation by some reasonable means, this is the first time you have
-        received notice of violation of this License (for any work) from that
-        copyright holder, and you cure the violation prior to 30 days after
-        your receipt of the notice.
-        
-          Termination of your rights under this section does not terminate the
-        licenses of parties who have received copies or rights from you under
-        this License.  If your rights have been terminated and not permanently
-        reinstated, you do not qualify to receive new licenses for the same
-        material under section 10.
-        
-          9. Acceptance Not Required for Having Copies.
-        
-          You are not required to accept this License in order to receive or
-        run a copy of the Program.  Ancillary propagation of a covered work
-        occurring solely as a consequence of using peer-to-peer transmission
-        to receive a copy likewise does not require acceptance.  However,
-        nothing other than this License grants you permission to propagate or
-        modify any covered work.  These actions infringe copyright if you do
-        not accept this License.  Therefore, by modifying or propagating a
-        covered work, you indicate your acceptance of this License to do so.
-        
-          10. Automatic Licensing of Downstream Recipients.
-        
-          Each time you convey a covered work, the recipient automatically
-        receives a license from the original licensors, to run, modify and
-        propagate that work, subject to this License.  You are not responsible
-        for enforcing compliance by third parties with this License.
-        
-          An "entity transaction" is a transaction transferring control of an
-        organization, or substantially all assets of one, or subdividing an
-        organization, or merging organizations.  If propagation of a covered
-        work results from an entity transaction, each party to that
-        transaction who receives a copy of the work also receives whatever
-        licenses to the work the party's predecessor in interest had or could
-        give under the previous paragraph, plus a right to possession of the
-        Corresponding Source of the work from the predecessor in interest, if
-        the predecessor has it or can get it with reasonable efforts.
-        
-          You may not impose any further restrictions on the exercise of the
-        rights granted or affirmed under this License.  For example, you may
-        not impose a license fee, royalty, or other charge for exercise of
-        rights granted under this License, and you may not initiate litigation
-        (including a cross-claim or counterclaim in a lawsuit) alleging that
-        any patent claim is infringed by making, using, selling, offering for
-        sale, or importing the Program or any portion of it.
-        
-          11. Patents.
-        
-          A "contributor" is a copyright holder who authorizes use under this
-        License of the Program or a work on which the Program is based.  The
-        work thus licensed is called the contributor's "contributor version".
-        
-          A contributor's "essential patent claims" are all patent claims
-        owned or controlled by the contributor, whether already acquired or
-        hereafter acquired, that would be infringed by some manner, permitted
-        by this License, of making, using, or selling its contributor version,
-        but do not include claims that would be infringed only as a
-        consequence of further modification of the contributor version.  For
-        purposes of this definition, "control" includes the right to grant
-        patent sublicenses in a manner consistent with the requirements of
-        this License.
-        
-          Each contributor grants you a non-exclusive, worldwide, royalty-free
-        patent license under the contributor's essential patent claims, to
-        make, use, sell, offer for sale, import and otherwise run, modify and
-        propagate the contents of its contributor version.
-        
-          In the following three paragraphs, a "patent license" is any express
-        agreement or commitment, however denominated, not to enforce a patent
-        (such as an express permission to practice a patent or covenant not to
-        sue for patent infringement).  To "grant" such a patent license to a
-        party means to make such an agreement or commitment not to enforce a
-        patent against the party.
-        
-          If you convey a covered work, knowingly relying on a patent license,
-        and the Corresponding Source of the work is not available for anyone
-        to copy, free of charge and under the terms of this License, through a
-        publicly available network server or other readily accessible means,
-        then you must either (1) cause the Corresponding Source to be so
-        available, or (2) arrange to deprive yourself of the benefit of the
-        patent license for this particular work, or (3) arrange, in a manner
-        consistent with the requirements of this License, to extend the patent
-        license to downstream recipients.  "Knowingly relying" means you have
-        actual knowledge that, but for the patent license, your conveying the
-        covered work in a country, or your recipient's use of the covered work
-        in a country, would infringe one or more identifiable patents in that
-        country that you have reason to believe are valid.
-        
-          If, pursuant to or in connection with a single transaction or
-        arrangement, you convey, or propagate by procuring conveyance of, a
-        covered work, and grant a patent license to some of the parties
-        receiving the covered work authorizing them to use, propagate, modify
-        or convey a specific copy of the covered work, then the patent license
-        you grant is automatically extended to all recipients of the covered
-        work and works based on it.
-        
-          A patent license is "discriminatory" if it does not include within
-        the scope of its coverage, prohibits the exercise of, or is
-        conditioned on the non-exercise of one or more of the rights that are
-        specifically granted under this License.  You may not convey a covered
-        work if you are a party to an arrangement with a third party that is
-        in the business of distributing software, under which you make payment
-        to the third party based on the extent of your activity of conveying
-        the work, and under which the third party grants, to any of the
-        parties who would receive the covered work from you, a discriminatory
-        patent license (a) in connection with copies of the covered work
-        conveyed by you (or copies made from those copies), or (b) primarily
-        for and in connection with specific products or compilations that
-        contain the covered work, unless you entered into that arrangement,
-        or that patent license was granted, prior to 28 March 2007.
-        
-          Nothing in this License shall be construed as excluding or limiting
-        any implied license or other defenses to infringement that may
-        otherwise be available to you under applicable patent law.
-        
-          12. No Surrender of Others' Freedom.
-        
-          If conditions are imposed on you (whether by court order, agreement or
-        otherwise) that contradict the conditions of this License, they do not
-        excuse you from the conditions of this License.  If you cannot convey a
-        covered work so as to satisfy simultaneously your obligations under this
-        License and any other pertinent obligations, then as a consequence you may
-        not convey it at all.  For example, if you agree to terms that obligate you
-        to collect a royalty for further conveying from those to whom you convey
-        the Program, the only way you could satisfy both those terms and this
-        License would be to refrain entirely from conveying the Program.
-        
-          13. Use with the GNU Affero General Public License.
-        
-          Notwithstanding any other provision of this License, you have
-        permission to link or combine any covered work with a work licensed
-        under version 3 of the GNU Affero General Public License into a single
-        combined work, and to convey the resulting work.  The terms of this
-        License will continue to apply to the part which is the covered work,
-        but the special requirements of the GNU Affero General Public License,
-        section 13, concerning interaction through a network will apply to the
-        combination as such.
-        
-          14. Revised Versions of this License.
-        
-          The Free Software Foundation may publish revised and/or new versions of
-        the GNU General Public License from time to time.  Such new versions will
-        be similar in spirit to the present version, but may differ in detail to
-        address new problems or concerns.
-        
-          Each version is given a distinguishing version number.  If the
-        Program specifies that a certain numbered version of the GNU General
-        Public License "or any later version" applies to it, you have the
-        option of following the terms and conditions either of that numbered
-        version or of any later version published by the Free Software
-        Foundation.  If the Program does not specify a version number of the
-        GNU General Public License, you may choose any version ever published
-        by the Free Software Foundation.
-        
-          If the Program specifies that a proxy can decide which future
-        versions of the GNU General Public License can be used, that proxy's
-        public statement of acceptance of a version permanently authorizes you
-        to choose that version for the Program.
-        
-          Later license versions may give you additional or different
-        permissions.  However, no additional obligations are imposed on any
-        author or copyright holder as a result of your choosing to follow a
-        later version.
-        
-          15. Disclaimer of Warranty.
-        
-          THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-        APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-        HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-        OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-        THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-        PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-        IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-        ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-        
-          16. Limitation of Liability.
-        
-          IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-        WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-        THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-        GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-        USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-        DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-        PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-        EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-        SUCH DAMAGES.
-        
-          17. Interpretation of Sections 15 and 16.
-        
-          If the disclaimer of warranty and limitation of liability provided
-        above cannot be given local legal effect according to their terms,
-        reviewing courts shall apply local law that most closely approximates
-        an absolute waiver of all civil liability in connection with the
-        Program, unless a warranty or assumption of liability accompanies a
-        copy of the Program in return for a fee.
-        
-                             END OF TERMS AND CONDITIONS
-        
-                    How to Apply These Terms to Your New Programs
-        
-          If you develop a new program, and you want it to be of the greatest
-        possible use to the public, the best way to achieve this is to make it
-        free software which everyone can redistribute and change under these terms.
-        
-          To do so, attach the following notices to the program.  It is safest
-        to attach them to the start of each source file to most effectively
-        state the exclusion of warranty; and each file should have at least
-        the "copyright" line and a pointer to where the full notice is found.
-        
-            <one line to give the program's name and a brief idea of what it does.>
-            Copyright (C) <year>  <name of author>
-        
-            This program is free software: you can redistribute it and/or modify
-            it under the terms of the GNU General Public License as published by
-            the Free Software Foundation, either version 3 of the License, or
-            (at your option) any later version.
-        
-            This program is distributed in the hope that it will be useful,
-            but WITHOUT ANY WARRANTY; without even the implied warranty of
-            MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-            GNU General Public License for more details.
-        
-            You should have received a copy of the GNU General Public License
-            along with this program.  If not, see <https://www.gnu.org/licenses/>.
-        
-        Also add information on how to contact you by electronic and paper mail.
-        
-          If the program does terminal interaction, make it output a short
-        notice like this when it starts in an interactive mode:
-        
-            <program>  Copyright (C) <year>  <name of author>
-            This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-            This is free software, and you are welcome to redistribute it
-            under certain conditions; type `show c' for details.
-        
-        The hypothetical commands `show w' and `show c' should show the appropriate
-        parts of the General Public License.  Of course, your program's commands
-        might be different; for a GUI interface, you would use an "about box".
-        
-          You should also get your employer (if you work as a programmer) or school,
-        if any, to sign a "copyright disclaimer" for the program, if necessary.
-        For more information on this, and how to apply and follow the GNU GPL, see
-        <https://www.gnu.org/licenses/>.
-        
-          The GNU General Public License does not permit incorporating your program
-        into proprietary programs.  If your program is a subroutine library, you
-        may consider it more useful to permit linking proprietary applications with
-        the library.  If this is what you want to do, use the GNU Lesser General
-        Public License instead of this License.  But first, please read
-        <https://www.gnu.org/licenses/why-not-lgpl.html>.
-        
-Project-URL: Homepage, https://github.com/yoterel/icatcher_plus
-Keywords: eyetracker,eyetracking
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: build
-Provides-Extra: dev
-License-File: LICENSE
-
-[![DOI](https://zenodo.org/badge/486841882.svg)](https://zenodo.org/badge/latestdoi/486841882)
-
-# iCatcher+
-
-# Introduction
-This repository contains all the code for [iCatcher+](https://psyarxiv.com/up97k/), a tool for performing automatic annotation of discrete infant gaze directions from videos collected in the lab, field or online (remotely). It also contains code for reproducing the original manuscripts results.
-
-Click below for a video including examples of representative good and poor performance, taken from videos of infants participating in online research (all families featured consented to sharing their video data publicly):
-
-[![iCatcher representative good and poor performance](https://img.youtube.com/vi/iK_T2P2ZDnU/0.jpg)](https://www.youtube.com/watch?v=iK_T2P2ZDnU)
-
-# Installation
-## Quick installation (Windows, Linux, Mac)
-This option will let you use iCatcher+ with minimum effort, but only for predictions (inference).
-We strongly recommend using a virtual environment such as [Miniconda](https://conda.io) or [virtualenv](https://pypi.org/project/virtualenv/) before running the command below.
-
-`pip install icatcher`
-
-You will also need [ffmpeg](https://www.ffmpeg.org/) installed in your system and available. When using for the first time, neural network model files will automatically be downloaded to a local cache folder. To control where they are downloaded to set the "ICATCHER_DATA_DIR" environment variable.
-
-## Installation for reproduction of original research results
-This options allows you to reproduce the paper results, train icatcher on your own dataset, compare and measure performance and visualize results as well.
-
-### Step 1: Clone this repository to get a copy of the code to run locally
-
-`git clone https://github.com/yoterel/icatcher_plus.git`
-
-### Step 2: Create a conda virtual environment
-
-We recommend installing [Miniconda](https://docs.conda.io/en/latest/miniconda.html) for this, then create an environment using the environment.yml file in this repository:
-
-**Note**: conda must be in the PATH envrionment variable for the shell to find it.
-
-Navigate to the icatcher_plus reproduce folder using the Anaconda Prompt:
-
-`cd /path/to/icathcer_plus/reproduce`
-
-Then:
-
-`conda env create -n env -f environment.yml`
-
-Or (if you want to install the environment in a specific location):
-
-`conda env create --prefix /path/to/virtual/environment -f "/path/to/environment.yml"`
-
-**Note for Mac users**: you might need to edit the [environment.yml](https://github.com/yoterel/icatcher_plus/blob/master/environment.yml) file depending on your OS version. see [here](https://github.com/yoterel/icatcher_plus/issues/6#issuecomment-1244125700) for how.
-
-Activate the environment
-
-`conda activate env`
-
-### Step 3: Download the neural network model & weight files
-
-iCatcher+ relies on some neural-network model files to work (or reproduce experiments).
-
-Please download all files from [here](https://osf.io/ycju8/download) and place them in the reproduce/models directory.
-
-
-# Running iCatcher+
-If you installed iCatcher+ from source, the inference file is "test.py". It will require an additional mandatory argument of which model file to use for predicitons.
-Otherwise, using the quick installation, you can run iCatcher+ with the command:
-
-`icatcher --help`
-
-which will list all available options. Description below will help you get more familiar with some common command line arguments.
-
-To run iCatcher+ with a video file (if a folder is provided, all videos will be used for prediction):
-
-`icatcher /path/to/my/video.mp4`
-
-A common option is to add:
-
-`icatcher /path/to/my/video.mp4 --use_fc_model`
-
-Which enables a child face detector for more robust results (however, sometimes this can result in too much loss of data).
-
-You can save a labeled video by adding:
-
-`--output_video_path /path/to/output_folder`
-
-If you want to output annotations to a file, use:
-
-`--output_annotation /path/to/output_annotation_folder`
-
-To show the predictions online in a seperate window, add the option:
-
-`--show_output`
-
-You can also add parameters to crop the video a given percent before passing to iCatcher: 
-
-`--crop_mode m` where `m` is any of [top, left, right], specifying which side of the video to crop from (if not provided, default is none; if crop_percent is provided but not crop_mode, default is top)
-
-`--crop_percent x` where `x` is an integer (default = 0) specifying what percent of the video size to crop from the specified side. E.g., if `--crop_mode top` is provided with `--crop_percent 10`, 10% of the video height will be cropped from the top. If `--crop_mode left` is provided with `--crop_percent 25`, 25% of the video width will be cropped from the left side, etc. 
-
-# Output format
-
-Currently we supports 2 output formats, though further formats can be added upon request.
-
-- raw_output: a file where each row will contain the frame number, the class prediction and the confidence of that prediction seperated by a comma
-- compressed: a npz file containing two numpy arrays, one encoding the predicted class (n x 1 int32) and another the confidence (n x 1 float32) where n is the number of frames. This file can be loaded into memory using the numpy.load function. For the map between class number and name see test.py ("predict_from_video" function).
-
-# Datasets access & reproduction of results
-
-The public videos from the Lookit dataset, along with human annotations and group-level demographics for all datasets, are available at https://osf.io/ujteb/. Videos from the Lookit dataset with permission granted for scientific use are available at https://osf.io/5u9df/. Requests for access can be directed to Junyi Chu (junyichu@mit.edu).
-
-Requests for access to the remainder of the datasets (Cali-BW, Senegal) can be directed to Dr. Katherine Adams Shannon (katashannon@gmail.com). Note that access to raw video files from the California-BW and Senegal datasets *is not available* due to restricted participant privacy agreements. To protect participant privacy, the participant identifiers for the video and demographic data are not linked to each other. However, this information is available upon reasonable request.
-
-We made substantial effort to allow reproduction of results form the paper. True reproduction requires full access to the datasets (including the videos).
-Instead, to reproduce most of the statistics we present in the paper for the Lookit dataset, run visualize.py using the following commands:
-
-First navigate to the reproduce folder:
-
-`cd /path/to/icatcher_plus/reproduce`
-
-Then run:
-
-`python visualize.py output resource/lookit_annotations/coding_human1 resource/lookit_annotations/coding_icatcherplus just_annotations --human2_codings_folder resource/lookit_annotations/coding_human2`
-
-Results will appear in a folder called "output".
-
-## Best Results (test sets)
-To view visualizations of all results, see [plots](https://github.com/yoterel/icatcher_plus/tree/master/reproduce/plots).
-Per-session plots (i.e. per-video) are sorted from 0 to n, where 0 has the lowest agreement (between iCatcher+ and Coder 1) and n the highest.
-### A Note About Data-Leaks
-The test sets were kept "untouched" until the very last stages of submission (i.e. they were not *directly* nor *indirectly* used optimize the network models). Conforming to this methodolgy is encouraged to avoid data leaks, so if you happen to submit improvements made to iCatcher+ in terms of performance, **do not** use the test sets for improving your method. Please consider creating a validation set out of the original training set for that.
-
-<table>
-        <tr>
-                <td align="center"> <img src="https://github.com/yoterel/icatcher_plus/blob/master/resource/agreement.png"  alt="0" width = 400px height = 300px ></td>
-                <td align="center"><img src="https://github.com/yoterel/icatcher_plus/blob/master/resource/agreement_vs_confidence.png"  alt="0" width = 400px height = 300px ></td>
-        </tr>
-        <tr><td colspan=2>Lookit</td></tr>
-        <tr>
-                <td><img src="https://github.com/yoterel/icatcher_plus/blob/master/resource/lookit_bar.png" alt="0" width = 400px height = 300px></td>
-                <td><img src="https://github.com/yoterel/icatcher_plus/blob/master/resource/lookit_conf.png" alt="1" width = 300px height = 300px></td>
-        </tr>
-        <tr><td colspan=2>California-BW</td></tr>
-        <tr>
-                <td><img src="https://github.com/yoterel/icatcher_plus/blob/master/resource/cali-bw_bar.png" alt="0" width = 400px height = 300px></td>
-                <td><img src="https://github.com/yoterel/icatcher_plus/blob/master/resource/cali-bw_conf.png" alt="1" width = 300px height = 300px></td>
-        </tr>
-        <tr><td colspan=2>Senegal</td></tr>
-        <tr>
-                <td><img src="https://github.com/yoterel/icatcher_plus/blob/master/resource/senegal_bar.png" alt="0" width = 400px height = 300px></td>
-                <td><img src="https://github.com/yoterel/icatcher_plus/blob/master/resource/senegal_conf.png" alt="1" width = 300px height = 300px></td>
-        </tr>
-</table>
-
-
-# Performance Benchmark
-We benchmarked iCatcher+ performance over 10 videos (res 640 x 480). Reported results are averaged upon all frames.
-
-<table>
-        <tr>
-                <td>iCatcher+ on GPU (NVIDIA GeForce RTX 2060)</td>
-                <td>~45 fps</td>
-        </tr>
-        <tr>
-                <td>iCatcher+ on CPU (Intel Core i7-9700)</td>
-                <td>~17 fps</td>
-        </tr>
-</table>
-
-## Project Structure (subject to change):
-
-    ├── src                     # code for package (inference only)
-    ├── tests                   # tests for package
-    ├── reproduce               # all code used for producing paper results, including training and visualizations.
-    
-# Contributions
-Feel free to contribute by submitting a pull request. Make sure to run all tests under /tests
-
-
+Metadata-Version: 2.1
+Name: icatcher
+Version: 0.1.0
+Summary: iCatcher+: Robust and automated annotation of infant gaze from videos collected in laboratory, field, and online studies.
+Author-email: Yotam Erel <erelyotam@gmail.com>
+License:                     GNU GENERAL PUBLIC LICENSE
+                               Version 3, 29 June 2007
+        
+         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+         Everyone is permitted to copy and distribute verbatim copies
+         of this license document, but changing it is not allowed.
+        
+                                    Preamble
+        
+          The GNU General Public License is a free, copyleft license for
+        software and other kinds of works.
+        
+          The licenses for most software and other practical works are designed
+        to take away your freedom to share and change the works.  By contrast,
+        the GNU General Public License is intended to guarantee your freedom to
+        share and change all versions of a program--to make sure it remains free
+        software for all its users.  We, the Free Software Foundation, use the
+        GNU General Public License for most of our software; it applies also to
+        any other work released this way by its authors.  You can apply it to
+        your programs, too.
+        
+          When we speak of free software, we are referring to freedom, not
+        price.  Our General Public Licenses are designed to make sure that you
+        have the freedom to distribute copies of free software (and charge for
+        them if you wish), that you receive source code or can get it if you
+        want it, that you can change the software or use pieces of it in new
+        free programs, and that you know you can do these things.
+        
+          To protect your rights, we need to prevent others from denying you
+        these rights or asking you to surrender the rights.  Therefore, you have
+        certain responsibilities if you distribute copies of the software, or if
+        you modify it: responsibilities to respect the freedom of others.
+        
+          For example, if you distribute copies of such a program, whether
+        gratis or for a fee, you must pass on to the recipients the same
+        freedoms that you received.  You must make sure that they, too, receive
+        or can get the source code.  And you must show them these terms so they
+        know their rights.
+        
+          Developers that use the GNU GPL protect your rights with two steps:
+        (1) assert copyright on the software, and (2) offer you this License
+        giving you legal permission to copy, distribute and/or modify it.
+        
+          For the developers' and authors' protection, the GPL clearly explains
+        that there is no warranty for this free software.  For both users' and
+        authors' sake, the GPL requires that modified versions be marked as
+        changed, so that their problems will not be attributed erroneously to
+        authors of previous versions.
+        
+          Some devices are designed to deny users access to install or run
+        modified versions of the software inside them, although the manufacturer
+        can do so.  This is fundamentally incompatible with the aim of
+        protecting users' freedom to change the software.  The systematic
+        pattern of such abuse occurs in the area of products for individuals to
+        use, which is precisely where it is most unacceptable.  Therefore, we
+        have designed this version of the GPL to prohibit the practice for those
+        products.  If such problems arise substantially in other domains, we
+        stand ready to extend this provision to those domains in future versions
+        of the GPL, as needed to protect the freedom of users.
+        
+          Finally, every program is threatened constantly by software patents.
+        States should not allow patents to restrict development and use of
+        software on general-purpose computers, but in those that do, we wish to
+        avoid the special danger that patents applied to a free program could
+        make it effectively proprietary.  To prevent this, the GPL assures that
+        patents cannot be used to render the program non-free.
+        
+          The precise terms and conditions for copying, distribution and
+        modification follow.
+        
+                               TERMS AND CONDITIONS
+        
+          0. Definitions.
+        
+          "This License" refers to version 3 of the GNU General Public License.
+        
+          "Copyright" also means copyright-like laws that apply to other kinds of
+        works, such as semiconductor masks.
+        
+          "The Program" refers to any copyrightable work licensed under this
+        License.  Each licensee is addressed as "you".  "Licensees" and
+        "recipients" may be individuals or organizations.
+        
+          To "modify" a work means to copy from or adapt all or part of the work
+        in a fashion requiring copyright permission, other than the making of an
+        exact copy.  The resulting work is called a "modified version" of the
+        earlier work or a work "based on" the earlier work.
+        
+          A "covered work" means either the unmodified Program or a work based
+        on the Program.
+        
+          To "propagate" a work means to do anything with it that, without
+        permission, would make you directly or secondarily liable for
+        infringement under applicable copyright law, except executing it on a
+        computer or modifying a private copy.  Propagation includes copying,
+        distribution (with or without modification), making available to the
+        public, and in some countries other activities as well.
+        
+          To "convey" a work means any kind of propagation that enables other
+        parties to make or receive copies.  Mere interaction with a user through
+        a computer network, with no transfer of a copy, is not conveying.
+        
+          An interactive user interface displays "Appropriate Legal Notices"
+        to the extent that it includes a convenient and prominently visible
+        feature that (1) displays an appropriate copyright notice, and (2)
+        tells the user that there is no warranty for the work (except to the
+        extent that warranties are provided), that licensees may convey the
+        work under this License, and how to view a copy of this License.  If
+        the interface presents a list of user commands or options, such as a
+        menu, a prominent item in the list meets this criterion.
+        
+          1. Source Code.
+        
+          The "source code" for a work means the preferred form of the work
+        for making modifications to it.  "Object code" means any non-source
+        form of a work.
+        
+          A "Standard Interface" means an interface that either is an official
+        standard defined by a recognized standards body, or, in the case of
+        interfaces specified for a particular programming language, one that
+        is widely used among developers working in that language.
+        
+          The "System Libraries" of an executable work include anything, other
+        than the work as a whole, that (a) is included in the normal form of
+        packaging a Major Component, but which is not part of that Major
+        Component, and (b) serves only to enable use of the work with that
+        Major Component, or to implement a Standard Interface for which an
+        implementation is available to the public in source code form.  A
+        "Major Component", in this context, means a major essential component
+        (kernel, window system, and so on) of the specific operating system
+        (if any) on which the executable work runs, or a compiler used to
+        produce the work, or an object code interpreter used to run it.
+        
+          The "Corresponding Source" for a work in object code form means all
+        the source code needed to generate, install, and (for an executable
+        work) run the object code and to modify the work, including scripts to
+        control those activities.  However, it does not include the work's
+        System Libraries, or general-purpose tools or generally available free
+        programs which are used unmodified in performing those activities but
+        which are not part of the work.  For example, Corresponding Source
+        includes interface definition files associated with source files for
+        the work, and the source code for shared libraries and dynamically
+        linked subprograms that the work is specifically designed to require,
+        such as by intimate data communication or control flow between those
+        subprograms and other parts of the work.
+        
+          The Corresponding Source need not include anything that users
+        can regenerate automatically from other parts of the Corresponding
+        Source.
+        
+          The Corresponding Source for a work in source code form is that
+        same work.
+        
+          2. Basic Permissions.
+        
+          All rights granted under this License are granted for the term of
+        copyright on the Program, and are irrevocable provided the stated
+        conditions are met.  This License explicitly affirms your unlimited
+        permission to run the unmodified Program.  The output from running a
+        covered work is covered by this License only if the output, given its
+        content, constitutes a covered work.  This License acknowledges your
+        rights of fair use or other equivalent, as provided by copyright law.
+        
+          You may make, run and propagate covered works that you do not
+        convey, without conditions so long as your license otherwise remains
+        in force.  You may convey covered works to others for the sole purpose
+        of having them make modifications exclusively for you, or provide you
+        with facilities for running those works, provided that you comply with
+        the terms of this License in conveying all material for which you do
+        not control copyright.  Those thus making or running the covered works
+        for you must do so exclusively on your behalf, under your direction
+        and control, on terms that prohibit them from making any copies of
+        your copyrighted material outside their relationship with you.
+        
+          Conveying under any other circumstances is permitted solely under
+        the conditions stated below.  Sublicensing is not allowed; section 10
+        makes it unnecessary.
+        
+          3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+        
+          No covered work shall be deemed part of an effective technological
+        measure under any applicable law fulfilling obligations under article
+        11 of the WIPO copyright treaty adopted on 20 December 1996, or
+        similar laws prohibiting or restricting circumvention of such
+        measures.
+        
+          When you convey a covered work, you waive any legal power to forbid
+        circumvention of technological measures to the extent such circumvention
+        is effected by exercising rights under this License with respect to
+        the covered work, and you disclaim any intention to limit operation or
+        modification of the work as a means of enforcing, against the work's
+        users, your or third parties' legal rights to forbid circumvention of
+        technological measures.
+        
+          4. Conveying Verbatim Copies.
+        
+          You may convey verbatim copies of the Program's source code as you
+        receive it, in any medium, provided that you conspicuously and
+        appropriately publish on each copy an appropriate copyright notice;
+        keep intact all notices stating that this License and any
+        non-permissive terms added in accord with section 7 apply to the code;
+        keep intact all notices of the absence of any warranty; and give all
+        recipients a copy of this License along with the Program.
+        
+          You may charge any price or no price for each copy that you convey,
+        and you may offer support or warranty protection for a fee.
+        
+          5. Conveying Modified Source Versions.
+        
+          You may convey a work based on the Program, or the modifications to
+        produce it from the Program, in the form of source code under the
+        terms of section 4, provided that you also meet all of these conditions:
+        
+            a) The work must carry prominent notices stating that you modified
+            it, and giving a relevant date.
+        
+            b) The work must carry prominent notices stating that it is
+            released under this License and any conditions added under section
+            7.  This requirement modifies the requirement in section 4 to
+            "keep intact all notices".
+        
+            c) You must license the entire work, as a whole, under this
+            License to anyone who comes into possession of a copy.  This
+            License will therefore apply, along with any applicable section 7
+            additional terms, to the whole of the work, and all its parts,
+            regardless of how they are packaged.  This License gives no
+            permission to license the work in any other way, but it does not
+            invalidate such permission if you have separately received it.
+        
+            d) If the work has interactive user interfaces, each must display
+            Appropriate Legal Notices; however, if the Program has interactive
+            interfaces that do not display Appropriate Legal Notices, your
+            work need not make them do so.
+        
+          A compilation of a covered work with other separate and independent
+        works, which are not by their nature extensions of the covered work,
+        and which are not combined with it such as to form a larger program,
+        in or on a volume of a storage or distribution medium, is called an
+        "aggregate" if the compilation and its resulting copyright are not
+        used to limit the access or legal rights of the compilation's users
+        beyond what the individual works permit.  Inclusion of a covered work
+        in an aggregate does not cause this License to apply to the other
+        parts of the aggregate.
+        
+          6. Conveying Non-Source Forms.
+        
+          You may convey a covered work in object code form under the terms
+        of sections 4 and 5, provided that you also convey the
+        machine-readable Corresponding Source under the terms of this License,
+        in one of these ways:
+        
+            a) Convey the object code in, or embodied in, a physical product
+            (including a physical distribution medium), accompanied by the
+            Corresponding Source fixed on a durable physical medium
+            customarily used for software interchange.
+        
+            b) Convey the object code in, or embodied in, a physical product
+            (including a physical distribution medium), accompanied by a
+            written offer, valid for at least three years and valid for as
+            long as you offer spare parts or customer support for that product
+            model, to give anyone who possesses the object code either (1) a
+            copy of the Corresponding Source for all the software in the
+            product that is covered by this License, on a durable physical
+            medium customarily used for software interchange, for a price no
+            more than your reasonable cost of physically performing this
+            conveying of source, or (2) access to copy the
+            Corresponding Source from a network server at no charge.
+        
+            c) Convey individual copies of the object code with a copy of the
+            written offer to provide the Corresponding Source.  This
+            alternative is allowed only occasionally and noncommercially, and
+            only if you received the object code with such an offer, in accord
+            with subsection 6b.
+        
+            d) Convey the object code by offering access from a designated
+            place (gratis or for a charge), and offer equivalent access to the
+            Corresponding Source in the same way through the same place at no
+            further charge.  You need not require recipients to copy the
+            Corresponding Source along with the object code.  If the place to
+            copy the object code is a network server, the Corresponding Source
+            may be on a different server (operated by you or a third party)
+            that supports equivalent copying facilities, provided you maintain
+            clear directions next to the object code saying where to find the
+            Corresponding Source.  Regardless of what server hosts the
+            Corresponding Source, you remain obligated to ensure that it is
+            available for as long as needed to satisfy these requirements.
+        
+            e) Convey the object code using peer-to-peer transmission, provided
+            you inform other peers where the object code and Corresponding
+            Source of the work are being offered to the general public at no
+            charge under subsection 6d.
+        
+          A separable portion of the object code, whose source code is excluded
+        from the Corresponding Source as a System Library, need not be
+        included in conveying the object code work.
+        
+          A "User Product" is either (1) a "consumer product", which means any
+        tangible personal property which is normally used for personal, family,
+        or household purposes, or (2) anything designed or sold for incorporation
+        into a dwelling.  In determining whether a product is a consumer product,
+        doubtful cases shall be resolved in favor of coverage.  For a particular
+        product received by a particular user, "normally used" refers to a
+        typical or common use of that class of product, regardless of the status
+        of the particular user or of the way in which the particular user
+        actually uses, or expects or is expected to use, the product.  A product
+        is a consumer product regardless of whether the product has substantial
+        commercial, industrial or non-consumer uses, unless such uses represent
+        the only significant mode of use of the product.
+        
+          "Installation Information" for a User Product means any methods,
+        procedures, authorization keys, or other information required to install
+        and execute modified versions of a covered work in that User Product from
+        a modified version of its Corresponding Source.  The information must
+        suffice to ensure that the continued functioning of the modified object
+        code is in no case prevented or interfered with solely because
+        modification has been made.
+        
+          If you convey an object code work under this section in, or with, or
+        specifically for use in, a User Product, and the conveying occurs as
+        part of a transaction in which the right of possession and use of the
+        User Product is transferred to the recipient in perpetuity or for a
+        fixed term (regardless of how the transaction is characterized), the
+        Corresponding Source conveyed under this section must be accompanied
+        by the Installation Information.  But this requirement does not apply
+        if neither you nor any third party retains the ability to install
+        modified object code on the User Product (for example, the work has
+        been installed in ROM).
+        
+          The requirement to provide Installation Information does not include a
+        requirement to continue to provide support service, warranty, or updates
+        for a work that has been modified or installed by the recipient, or for
+        the User Product in which it has been modified or installed.  Access to a
+        network may be denied when the modification itself materially and
+        adversely affects the operation of the network or violates the rules and
+        protocols for communication across the network.
+        
+          Corresponding Source conveyed, and Installation Information provided,
+        in accord with this section must be in a format that is publicly
+        documented (and with an implementation available to the public in
+        source code form), and must require no special password or key for
+        unpacking, reading or copying.
+        
+          7. Additional Terms.
+        
+          "Additional permissions" are terms that supplement the terms of this
+        License by making exceptions from one or more of its conditions.
+        Additional permissions that are applicable to the entire Program shall
+        be treated as though they were included in this License, to the extent
+        that they are valid under applicable law.  If additional permissions
+        apply only to part of the Program, that part may be used separately
+        under those permissions, but the entire Program remains governed by
+        this License without regard to the additional permissions.
+        
+          When you convey a copy of a covered work, you may at your option
+        remove any additional permissions from that copy, or from any part of
+        it.  (Additional permissions may be written to require their own
+        removal in certain cases when you modify the work.)  You may place
+        additional permissions on material, added by you to a covered work,
+        for which you have or can give appropriate copyright permission.
+        
+          Notwithstanding any other provision of this License, for material you
+        add to a covered work, you may (if authorized by the copyright holders of
+        that material) supplement the terms of this License with terms:
+        
+            a) Disclaiming warranty or limiting liability differently from the
+            terms of sections 15 and 16 of this License; or
+        
+            b) Requiring preservation of specified reasonable legal notices or
+            author attributions in that material or in the Appropriate Legal
+            Notices displayed by works containing it; or
+        
+            c) Prohibiting misrepresentation of the origin of that material, or
+            requiring that modified versions of such material be marked in
+            reasonable ways as different from the original version; or
+        
+            d) Limiting the use for publicity purposes of names of licensors or
+            authors of the material; or
+        
+            e) Declining to grant rights under trademark law for use of some
+            trade names, trademarks, or service marks; or
+        
+            f) Requiring indemnification of licensors and authors of that
+            material by anyone who conveys the material (or modified versions of
+            it) with contractual assumptions of liability to the recipient, for
+            any liability that these contractual assumptions directly impose on
+            those licensors and authors.
+        
+          All other non-permissive additional terms are considered "further
+        restrictions" within the meaning of section 10.  If the Program as you
+        received it, or any part of it, contains a notice stating that it is
+        governed by this License along with a term that is a further
+        restriction, you may remove that term.  If a license document contains
+        a further restriction but permits relicensing or conveying under this
+        License, you may add to a covered work material governed by the terms
+        of that license document, provided that the further restriction does
+        not survive such relicensing or conveying.
+        
+          If you add terms to a covered work in accord with this section, you
+        must place, in the relevant source files, a statement of the
+        additional terms that apply to those files, or a notice indicating
+        where to find the applicable terms.
+        
+          Additional terms, permissive or non-permissive, may be stated in the
+        form of a separately written license, or stated as exceptions;
+        the above requirements apply either way.
+        
+          8. Termination.
+        
+          You may not propagate or modify a covered work except as expressly
+        provided under this License.  Any attempt otherwise to propagate or
+        modify it is void, and will automatically terminate your rights under
+        this License (including any patent licenses granted under the third
+        paragraph of section 11).
+        
+          However, if you cease all violation of this License, then your
+        license from a particular copyright holder is reinstated (a)
+        provisionally, unless and until the copyright holder explicitly and
+        finally terminates your license, and (b) permanently, if the copyright
+        holder fails to notify you of the violation by some reasonable means
+        prior to 60 days after the cessation.
+        
+          Moreover, your license from a particular copyright holder is
+        reinstated permanently if the copyright holder notifies you of the
+        violation by some reasonable means, this is the first time you have
+        received notice of violation of this License (for any work) from that
+        copyright holder, and you cure the violation prior to 30 days after
+        your receipt of the notice.
+        
+          Termination of your rights under this section does not terminate the
+        licenses of parties who have received copies or rights from you under
+        this License.  If your rights have been terminated and not permanently
+        reinstated, you do not qualify to receive new licenses for the same
+        material under section 10.
+        
+          9. Acceptance Not Required for Having Copies.
+        
+          You are not required to accept this License in order to receive or
+        run a copy of the Program.  Ancillary propagation of a covered work
+        occurring solely as a consequence of using peer-to-peer transmission
+        to receive a copy likewise does not require acceptance.  However,
+        nothing other than this License grants you permission to propagate or
+        modify any covered work.  These actions infringe copyright if you do
+        not accept this License.  Therefore, by modifying or propagating a
+        covered work, you indicate your acceptance of this License to do so.
+        
+          10. Automatic Licensing of Downstream Recipients.
+        
+          Each time you convey a covered work, the recipient automatically
+        receives a license from the original licensors, to run, modify and
+        propagate that work, subject to this License.  You are not responsible
+        for enforcing compliance by third parties with this License.
+        
+          An "entity transaction" is a transaction transferring control of an
+        organization, or substantially all assets of one, or subdividing an
+        organization, or merging organizations.  If propagation of a covered
+        work results from an entity transaction, each party to that
+        transaction who receives a copy of the work also receives whatever
+        licenses to the work the party's predecessor in interest had or could
+        give under the previous paragraph, plus a right to possession of the
+        Corresponding Source of the work from the predecessor in interest, if
+        the predecessor has it or can get it with reasonable efforts.
+        
+          You may not impose any further restrictions on the exercise of the
+        rights granted or affirmed under this License.  For example, you may
+        not impose a license fee, royalty, or other charge for exercise of
+        rights granted under this License, and you may not initiate litigation
+        (including a cross-claim or counterclaim in a lawsuit) alleging that
+        any patent claim is infringed by making, using, selling, offering for
+        sale, or importing the Program or any portion of it.
+        
+          11. Patents.
+        
+          A "contributor" is a copyright holder who authorizes use under this
+        License of the Program or a work on which the Program is based.  The
+        work thus licensed is called the contributor's "contributor version".
+        
+          A contributor's "essential patent claims" are all patent claims
+        owned or controlled by the contributor, whether already acquired or
+        hereafter acquired, that would be infringed by some manner, permitted
+        by this License, of making, using, or selling its contributor version,
+        but do not include claims that would be infringed only as a
+        consequence of further modification of the contributor version.  For
+        purposes of this definition, "control" includes the right to grant
+        patent sublicenses in a manner consistent with the requirements of
+        this License.
+        
+          Each contributor grants you a non-exclusive, worldwide, royalty-free
+        patent license under the contributor's essential patent claims, to
+        make, use, sell, offer for sale, import and otherwise run, modify and
+        propagate the contents of its contributor version.
+        
+          In the following three paragraphs, a "patent license" is any express
+        agreement or commitment, however denominated, not to enforce a patent
+        (such as an express permission to practice a patent or covenant not to
+        sue for patent infringement).  To "grant" such a patent license to a
+        party means to make such an agreement or commitment not to enforce a
+        patent against the party.
+        
+          If you convey a covered work, knowingly relying on a patent license,
+        and the Corresponding Source of the work is not available for anyone
+        to copy, free of charge and under the terms of this License, through a
+        publicly available network server or other readily accessible means,
+        then you must either (1) cause the Corresponding Source to be so
+        available, or (2) arrange to deprive yourself of the benefit of the
+        patent license for this particular work, or (3) arrange, in a manner
+        consistent with the requirements of this License, to extend the patent
+        license to downstream recipients.  "Knowingly relying" means you have
+        actual knowledge that, but for the patent license, your conveying the
+        covered work in a country, or your recipient's use of the covered work
+        in a country, would infringe one or more identifiable patents in that
+        country that you have reason to believe are valid.
+        
+          If, pursuant to or in connection with a single transaction or
+        arrangement, you convey, or propagate by procuring conveyance of, a
+        covered work, and grant a patent license to some of the parties
+        receiving the covered work authorizing them to use, propagate, modify
+        or convey a specific copy of the covered work, then the patent license
+        you grant is automatically extended to all recipients of the covered
+        work and works based on it.
+        
+          A patent license is "discriminatory" if it does not include within
+        the scope of its coverage, prohibits the exercise of, or is
+        conditioned on the non-exercise of one or more of the rights that are
+        specifically granted under this License.  You may not convey a covered
+        work if you are a party to an arrangement with a third party that is
+        in the business of distributing software, under which you make payment
+        to the third party based on the extent of your activity of conveying
+        the work, and under which the third party grants, to any of the
+        parties who would receive the covered work from you, a discriminatory
+        patent license (a) in connection with copies of the covered work
+        conveyed by you (or copies made from those copies), or (b) primarily
+        for and in connection with specific products or compilations that
+        contain the covered work, unless you entered into that arrangement,
+        or that patent license was granted, prior to 28 March 2007.
+        
+          Nothing in this License shall be construed as excluding or limiting
+        any implied license or other defenses to infringement that may
+        otherwise be available to you under applicable patent law.
+        
+          12. No Surrender of Others' Freedom.
+        
+          If conditions are imposed on you (whether by court order, agreement or
+        otherwise) that contradict the conditions of this License, they do not
+        excuse you from the conditions of this License.  If you cannot convey a
+        covered work so as to satisfy simultaneously your obligations under this
+        License and any other pertinent obligations, then as a consequence you may
+        not convey it at all.  For example, if you agree to terms that obligate you
+        to collect a royalty for further conveying from those to whom you convey
+        the Program, the only way you could satisfy both those terms and this
+        License would be to refrain entirely from conveying the Program.
+        
+          13. Use with the GNU Affero General Public License.
+        
+          Notwithstanding any other provision of this License, you have
+        permission to link or combine any covered work with a work licensed
+        under version 3 of the GNU Affero General Public License into a single
+        combined work, and to convey the resulting work.  The terms of this
+        License will continue to apply to the part which is the covered work,
+        but the special requirements of the GNU Affero General Public License,
+        section 13, concerning interaction through a network will apply to the
+        combination as such.
+        
+          14. Revised Versions of this License.
+        
+          The Free Software Foundation may publish revised and/or new versions of
+        the GNU General Public License from time to time.  Such new versions will
+        be similar in spirit to the present version, but may differ in detail to
+        address new problems or concerns.
+        
+          Each version is given a distinguishing version number.  If the
+        Program specifies that a certain numbered version of the GNU General
+        Public License "or any later version" applies to it, you have the
+        option of following the terms and conditions either of that numbered
+        version or of any later version published by the Free Software
+        Foundation.  If the Program does not specify a version number of the
+        GNU General Public License, you may choose any version ever published
+        by the Free Software Foundation.
+        
+          If the Program specifies that a proxy can decide which future
+        versions of the GNU General Public License can be used, that proxy's
+        public statement of acceptance of a version permanently authorizes you
+        to choose that version for the Program.
+        
+          Later license versions may give you additional or different
+        permissions.  However, no additional obligations are imposed on any
+        author or copyright holder as a result of your choosing to follow a
+        later version.
+        
+          15. Disclaimer of Warranty.
+        
+          THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+        APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+        HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+        OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+        THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+        PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+        IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+        ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+        
+          16. Limitation of Liability.
+        
+          IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+        WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+        THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+        GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+        USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+        DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+        PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+        EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+        SUCH DAMAGES.
+        
+          17. Interpretation of Sections 15 and 16.
+        
+          If the disclaimer of warranty and limitation of liability provided
+        above cannot be given local legal effect according to their terms,
+        reviewing courts shall apply local law that most closely approximates
+        an absolute waiver of all civil liability in connection with the
+        Program, unless a warranty or assumption of liability accompanies a
+        copy of the Program in return for a fee.
+        
+                             END OF TERMS AND CONDITIONS
+        
+                    How to Apply These Terms to Your New Programs
+        
+          If you develop a new program, and you want it to be of the greatest
+        possible use to the public, the best way to achieve this is to make it
+        free software which everyone can redistribute and change under these terms.
+        
+          To do so, attach the following notices to the program.  It is safest
+        to attach them to the start of each source file to most effectively
+        state the exclusion of warranty; and each file should have at least
+        the "copyright" line and a pointer to where the full notice is found.
+        
+            <one line to give the program's name and a brief idea of what it does.>
+            Copyright (C) <year>  <name of author>
+        
+            This program is free software: you can redistribute it and/or modify
+            it under the terms of the GNU General Public License as published by
+            the Free Software Foundation, either version 3 of the License, or
+            (at your option) any later version.
+        
+            This program is distributed in the hope that it will be useful,
+            but WITHOUT ANY WARRANTY; without even the implied warranty of
+            MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+            GNU General Public License for more details.
+        
+            You should have received a copy of the GNU General Public License
+            along with this program.  If not, see <https://www.gnu.org/licenses/>.
+        
+        Also add information on how to contact you by electronic and paper mail.
+        
+          If the program does terminal interaction, make it output a short
+        notice like this when it starts in an interactive mode:
+        
+            <program>  Copyright (C) <year>  <name of author>
+            This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+            This is free software, and you are welcome to redistribute it
+            under certain conditions; type `show c' for details.
+        
+        The hypothetical commands `show w' and `show c' should show the appropriate
+        parts of the General Public License.  Of course, your program's commands
+        might be different; for a GUI interface, you would use an "about box".
+        
+          You should also get your employer (if you work as a programmer) or school,
+        if any, to sign a "copyright disclaimer" for the program, if necessary.
+        For more information on this, and how to apply and follow the GNU GPL, see
+        <https://www.gnu.org/licenses/>.
+        
+          The GNU General Public License does not permit incorporating your program
+        into proprietary programs.  If your program is a subroutine library, you
+        may consider it more useful to permit linking proprietary applications with
+        the library.  If this is what you want to do, use the GNU Lesser General
+        Public License instead of this License.  But first, please read
+        <https://www.gnu.org/licenses/why-not-lgpl.html>.
+        
+Project-URL: Homepage, https://github.com/yoterel/icatcher_plus
+Keywords: eyetracker,eyetracking
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: build
+Provides-Extra: dev
+License-File: LICENSE
+
+[![DOI](https://zenodo.org/badge/486841882.svg)](https://zenodo.org/badge/latestdoi/486841882)
+
+# iCatcher+
+
+# Introduction
+This repository contains the official code for [iCatcher+](https://doi.org/10.1177/25152459221147250), a tool for performing automatic annotation of discrete infant gaze directions from videos collected in the lab, field or online (remotely). It also contains code for reproducing the original paper results.
+
+Click below for a video including examples of representative good and poor performance, taken from videos of infants participating in online research (all families featured consented to sharing their video data publicly):
+
+[![iCatcher representative good and poor performance](https://img.youtube.com/vi/iK_T2P2ZDnU/0.jpg)](https://www.youtube.com/watch?v=iK_T2P2ZDnU)
+
+# Installation
+## Quick installation (Windows, Linux, Mac)
+This option will let you use iCatcher+ with minimum effort, but only for predictions (inference).
+We strongly recommend using a virtual environment such as [Miniconda](https://conda.io) or [virtualenv](https://pypi.org/project/virtualenv/) before running the command below.
+
+`pip install icatcher`
+
+You will also need [ffmpeg](https://www.ffmpeg.org/) installed in your system and available (if you used conda, you can quickly install it with `conda install -c conda-forge ffmpeg`).
+
+Note1:
+If you require speedy performance, prior to installing icatcher you should install [PyTorch](https://pytorch.org/) with GPU support (see [here](https://pytorch.org/get-started/locally/) for instructions). This assumes you have a supported GPU on your machine.
+
+Note2:
+When using iCatcher+ for the first time, neural network model files will automatically be downloaded to a local cache folder. To control where they are downloaded to set the "ICATCHER_DATA_DIR" environment variable.
+
+## Reproduction of original research results / retraining on your own dataset
+
+see [reproduce](https://github.com/icatcherplus/icatcher_plus/tree/master/reproduce) for a full set of instructions.
+
+# Running iCatcher+
+
+You can run iCatcher+ with the command:
+
+`icatcher --help`
+
+which will list all available options. Description below will help you get more familiar with some common command line arguments.
+
+To run iCatcher+ with a video file (if a folder is provided, all videos will be used for prediction):
+
+`icatcher /path/to/my/video.mp4`
+
+A common option is to add:
+
+`icatcher /path/to/my/video.mp4 --use_fc_model`
+
+Which enables a child face detector for more robust results (however, sometimes this can result in too much loss of data).
+
+You can save a labeled video by adding:
+
+`--output_video_path /path/to/output_folder`
+
+If you want to output annotations to a file, use:
+
+`--output_annotation /path/to/output_annotation_folder`
+
+To show the predictions online in a seperate window, add the option:
+
+`--show_output`
+
+You can also add parameters to crop the video a given percent before passing to iCatcher: 
+
+`--crop_mode m` where `m` is any of [top, left, right], specifying which side of the video to crop from (if not provided, default is none; if crop_percent is provided but not crop_mode, default is top)
+
+`--crop_percent x` where `x` is an integer (default = 0) specifying what percent of the video size to crop from the specified side. E.g., if `--crop_mode top` is provided with `--crop_percent 10`, 10% of the video height will be cropped from the top. If `--crop_mode left` is provided with `--crop_percent 25`, 25% of the video width will be cropped from the left side, etc. 
+
+# Output format
+
+Currently we supports 2 output formats, though further formats can be added upon request.
+
+- raw_output: a file where each row will contain the frame number, the class prediction and the confidence of that prediction seperated by a comma
+- compressed: a npz file containing two numpy arrays, one encoding the predicted class (n x 1 int32) and another the confidence (n x 1 float32) where n is the number of frames. This file can be loaded into memory using the numpy.load function. For the map between class number and name see test.py ("predict_from_video" function).
+
+# Datasets access
+
+The public videos from the Lookit dataset, along with human annotations and group-level demographics for all datasets, are available at https://osf.io/ujteb/. Videos from the Lookit dataset with permission granted for scientific use are available at https://osf.io/5u9df/. Requests for access can be directed to Junyi Chu (junyichu@mit.edu).
+
+Requests for access to the remainder of the datasets (Cali-BW, Senegal) can be directed to Dr. Katherine Adams Shannon (katashannon@gmail.com). Note that access to raw video files from the California-BW and Senegal datasets *is not available* due to restricted participant privacy agreements. To protect participant privacy, the participant identifiers for the video and demographic data are not linked to each other. However, this information is available upon reasonable request.
+
+# Performance Benchmark
+We benchmarked iCatcher+ performance over 10 videos (res 640 x 480). Reported results are averaged upon all frames.
+
+<table>
+        <tr>
+                <td>iCatcher+ on GPU (NVIDIA GeForce RTX 2060)</td>
+                <td>~45 fps</td>
+        </tr>
+        <tr>
+                <td>iCatcher+ on CPU (Intel Core i7-9700)</td>
+                <td>~17 fps</td>
+        </tr>
+</table>
+
+## Project Structure (subject to change):
+
+    ├── src                     # code for package (inference only)
+    ├── tests                   # tests for package
+    ├── reproduce               # all code used for producing paper results, including training and visualizations.
+    
+# Troubleshooting Issues
+Please open a github issue for any question or problem you encounter. We kindly ask to first skim through closed issues to see if your problem was already addressed.
+
+# Citation
+```
+@article{doi:10.1177/25152459221147250,
+author = {Yotam Erel and Katherine Adams Shannon and Junyi Chu and Kim Scott and Melissa Kline Struhl and Peng Cao and Xincheng Tan and Peter Hart and Gal Raz and Sabrina Piccolo and Catherine Mei and Christine Potter and Sagi Jaffe-Dax and Casey Lew-Williams and Joshua Tenenbaum and Katherine Fairchild and Amit Bermano and Shari Liu},
+title ={iCatcher+: Robust and Automated Annotation of Infants’ and Young Children’s Gaze Behavior From Videos Collected in Laboratory, Field, and Online Studies},
+journal = {Advances in Methods and Practices in Psychological Science},
+volume = {6},
+number = {2},
+pages = {25152459221147250},
+year = {2023},
+doi = {10.1177/25152459221147250},
+URL = { 
+        https://doi.org/10.1177/25152459221147250
+},
+eprint = { 
+        https://doi.org/10.1177/25152459221147250 
+}
+}
+```
+
+
```

### Comparing `icatcher-0.0.9/src/icatcher/cli.py` & `icatcher-0.1.0/src/icatcher/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,497 +1,440 @@
-import logging
-import torch
-import numpy as np
-import cv2
-from PIL import Image
-from pathlib import Path
-from . import options
-from . import draw
-from . import video
-from . import models
-from . import parsers
-from . import version
-import pooch
-
-def detect_face_opencv_dnn(net, frame, conf_threshold):
-    """
-    Uses a pretrained face detection model to generate facial bounding boxes,
-    with the format [x, y, width, height] where [x, y] is the lower left coord
-    :param net:
-    :param frame:
-    :param conf_threshold:
-    :return:
-    """
-    frameHeight = frame.shape[0]
-    frameWidth = frame.shape[1]
-    blob = cv2.dnn.blobFromImage(frame, 1.0, (300, 300), [104, 117, 123], False, False)
-    net.setInput(blob)
-    detections = net.forward()
-    bboxes = []
-    for i in range(detections.shape[2]):
-        confidence = detections[0, 0, i, 2]
-        if confidence > conf_threshold:
-            x1 = max(int(detections[0, 0, i, 3] * frameWidth), 0)  # left side of box
-            y1 = max(int(detections[0, 0, i, 4] * frameHeight), 0)  # top side of box
-            if x1 >= frameWidth or y1 >= frameHeight:  # if they are larger than image size, bbox is invalid
-                continue
-            x2 = min(int(detections[0, 0, i, 5] * frameWidth), frameWidth)  # either right side of box or frame width
-            y2 = min(int(detections[0, 0, i, 6] * frameHeight), frameHeight)  # either the bottom side of box of frame height
-            bboxes.append([x1, y1, x2-x1, y2-y1])  # (left, top, width, height)
-    return bboxes
-
-class FaceClassifierArgs:
-    """
-    encapsulates face classifier arguments
-    """
-    def __init__(self, device):
-        self.device = device
-        self.rotation = False
-        self.cropping = False
-        self.hor_flip = False
-        self.ver_flip = False
-        self.color = False
-        self.erasing = False
-        self.noise = False
-        self.model = "vgg16"
-        self.dropout = 0.0
-
-
-def select_face(bboxes, frame, fc_model, fc_data_transforms, hor, ver, device):
-    """
-    selects a correct face from candidates bbox in frame
-    :param bboxes: the bounding boxes of candidates
-    :param frame: the frame
-    :param fc_model: a classifier model, if passed it is used to decide.
-    :param fc_data_transforms: the transformations to apply to the images before fc_model sees them
-    :param hor: the last known horizontal correct face location
-    :param ver: the last known vertical correct face location
-    :return: the cropped face and its bbox data
-    """
-    if fc_model:
-        centers = []
-        faces = []
-        for box in bboxes:
-            crop_img = frame[box[1]:box[1] + box[3], box[0]:box[0] + box[2]]
-            face_box = np.array([box[1], box[1] + box[3], box[0], box[0] + box[2]])
-            img_shape = np.array(frame.shape)
-            ratio = np.array([face_box[0] / img_shape[0], face_box[1] / img_shape[0],
-                              face_box[2] / img_shape[1], face_box[3] / img_shape[1]])
-            face_ver = (ratio[0] + ratio[1]) / 2
-            face_hor = (ratio[2] + ratio[3]) / 2
-
-            centers.append([face_hor, face_ver])
-            img = crop_img
-            img = fc_data_transforms['val'](img)
-            faces.append(img)
-        centers = np.stack(centers)
-        faces = torch.stack(faces).to(device)
-        output = fc_model(faces)
-        _, preds = torch.max(output, 1)
-        preds = preds.cpu().numpy()
-        idxs = np.where(preds == 0)[0]
-        if idxs.size == 0:
-            bbox = None
-        else:
-            centers = centers[idxs]
-            dis = np.sqrt((centers[:, 0] - hor) ** 2 + (centers[:, 1] - ver) ** 2)
-            i = np.argmin(dis)
-            # crop_img = faces[idxs[i]]
-            bbox = bboxes[idxs[i]]
-            # hor, ver = centers[i]
-    else:   # select lowest face in image, probably belongs to kid
-        bbox = min(bboxes, key=lambda x: x[3] - x[1])
-    return bbox
-
-def fix_illegal_transitions(loc, answers, confidences, illegal_transitions, corrected_transitions):
-    """
-    this method fixes illegal transitions happening in answers at [loc-max_trans_len+1, loc] inclusive
-    """
-    for i, transition in enumerate(illegal_transitions):
-        len_trans = len(transition)
-        buffer = answers[loc-len_trans+1:loc+1]
-        if buffer == transition:
-            buffer_update = corrected_transitions[i]
-            answers[loc-len_trans+1:loc+1] = buffer_update
-            buffer_splits = np.where(np.array(buffer_update) != np.array(buffer))
-            for spot in buffer_splits[0].tolist():
-                confidences[loc - len_trans + 1 + spot] = -1
-    return answers, confidences
-
-def extract_crop(frame, bbox, opt):
-    """
-    extracts a crop from a frame using bbox, and transforms it
-    :param frame: the frame
-    :param bbox: opencv bbox 4x1
-    :param opt: command line options
-    :return: the crop and the 5x1 box features
-    """
-    if bbox is None:
-        return None, None
-    img_shape = np.array(frame.shape)
-    face_box = np.array([bbox[1], bbox[1] + bbox[3], bbox[0], bbox[0] + bbox[2]])
-    crop = frame[bbox[1]:bbox[1] + bbox[3], bbox[0]:bbox[0] + bbox[2]]
-
-    test_transforms = models.DataTransforms(opt.image_size,
-                                          opt.per_channel_mean,
-                                          opt.per_channel_std).transformations["test"]
-    crop = test_transforms(Image.fromarray(crop))
-    crop = crop.permute(1, 2, 0).unsqueeze(0).numpy()
-    ratio = np.array([face_box[0] / img_shape[0], face_box[1] / img_shape[0],
-                      face_box[2] / img_shape[1], face_box[3] / img_shape[1]])
-    face_size = (ratio[1] - ratio[0]) * (ratio[3] - ratio[2])
-    face_ver = (ratio[0] + ratio[1]) / 2
-    face_hor = (ratio[2] + ratio[3]) / 2
-    face_height = ratio[1] - ratio[0]
-    face_width = ratio[3] - ratio[2]
-    my_box = np.array([face_size, face_ver, face_hor, face_height, face_width])
-    return crop, my_box
-
-
-def process_video(video_path, opt):
-    """
-    give a video path, process it and return a generator to iterate over frames
-    :param video_path: the video path
-    :param opt: command line options
-    :return: a generator to iterate over frames, framerate, resolution, and height/width pixel coordinates to crop from
-    """
-    cap = cv2.VideoCapture(str(video_path))
-    # Get some basic info about the video
-
-    vfr, meta_data = video.is_video_vfr(video_path, get_meta_data=True)
-    framerate = video.get_fps(video_path)
-    if vfr:
-        logging.warning("video file: {} has variable frame rate".format(str(video_path.name)))
-        logging.info(str(meta_data))
-        if opt.output_video_path:
-            # todo: support this by extracting frame timestamps
-            # i.e.: frame_info, vfr_frame_counter, _ = video.get_frame_information(video_path)
-            logging.warning("output_video_path argument passed, but input video is VFR !")
-    else:
-        logging.info("video fps: {}".format(framerate))
-    raw_width = meta_data["width"]
-    raw_height = meta_data["height"]
-    cropped_height = raw_height
-    if "top" in opt.crop_mode:
-        cropped_height = int(raw_height * (1 - (opt.crop_percent / 100)))  # x% of the video from the top
-    cropped_width = raw_width
-    if "left" and "right" in opt.crop_mode:
-        cropped_width = int(raw_width * (1 - (2*opt.crop_percent / 100)))  # x% of the video from both left/right
-    elif "left" in opt.crop_mode or "right" in opt.crop_mode:
-        cropped_width = int(raw_width * (1 - (opt.crop_percent / 100)))  # x% of the video from both left/right
-    resolution = (int(cropped_width), int(cropped_height))
-    h_start_at = (raw_height - cropped_height)
-    h_end_at = raw_height
-    if "left" and "right" in opt.crop_mode:
-        w_start_at = (raw_width - cropped_width)//2
-        w_end_at = w_start_at + cropped_width
-    elif "left" in opt.crop_mode:
-        w_start_at = (raw_width - cropped_width)
-        w_end_at = raw_width
-    elif "right" in opt.crop_mode:
-        w_start_at = 0
-        w_end_at = cropped_width
-    elif "top" in opt.crop_mode:
-        w_start_at = 0
-        w_end_at = raw_width
-    return cap, framerate, resolution, h_start_at, h_end_at, w_start_at, w_end_at
-
-def load_models(opt):
-    """
-    loads all relevant neural network models to perform predictions
-    models will be automatically downloaded if not found in the cache,
-    user may overide downloaded location with the env variable ICATCHER_DATA_DIR
-    defaults:
-    :Mac: "~/Library/Caches/<AppName>"
-    :Unix: "~/.cache/<AppName>" or the value of the "XDG_CACHE_HOME"
-    environment variable, if defined.
-    :Windows: "C:\\Users\\<user>\\AppData\\Local\\<AppAuthor>\\<AppName>\\Cache"
-    :param opt: command line options
-    :return all nn models
-    """
-    GOODBOY = pooch.create(path=pooch.os_cache("icatcher_plus"),
-                           base_url="https://osf.io/ycju8/download",
-                           version=version,
-                           version_dev="main",
-                           env="ICATCHER_DATA_DIR",
-                           registry={"zip_content.txt": "d81bfb5a183edea6dc74f7f342d516a9843865570b9ecfbf481209ec5114110a",
-                                     "icatcher+_models.zip": "d78385b3a08f3d55ce75249142d15549e4c5552d5e1231cad3b69063bb778ce9"},
-                           urls={"zip_content.txt":"https://osf.io/v4w53/download",
-                                 "icatcher+_models.zip":"https://osf.io/ycju8/download"})
-    # zip_content_file = GOODBOY.fetch("zip_content.txt")
-    # with open(zip_content_file, "r") as f:
-        # zip_content = [x.strip() for x in f]
-    file_paths = GOODBOY.fetch("icatcher+_models.zip",
-                               processor=pooch.Unzip(),
-                               progressbar=True)
-    file_names = [Path(x).name for x in file_paths]
-    face_detector_model_file = file_paths[file_names.index("face_model.caffemodel")]
-    config_file = file_paths[file_names.index("config.prototxt")]
-    path_to_gaze_model = file_paths[file_names.index("icatcher+_lookit.pth")]
-    if opt.model:
-        path_to_gaze_model = opt.model
-    path_to_fc_model = file_paths[file_names.index("face_classifier_lookit.pth")]
-    if opt.fc_model:
-        path_to_fc_model = opt.fc_model
-    # face_detector_model_file = Path("models", "face_model.caffemodel")
-    # config_file = Path("models", "config.prototxt")
-    # path_to_gaze_model = opt.model
-    gaze_model = models.GazeCodingModel(opt).to(opt.device)
-    if opt.device == 'cpu':
-        state_dict = torch.load(str(path_to_gaze_model), map_location=torch.device(opt.device))
-    else:
-        state_dict = torch.load(str(path_to_gaze_model))
-    try:
-        gaze_model.load_state_dict(state_dict)
-    except RuntimeError as e:  # hack to deal with models trained on distributed setup
-        from collections import OrderedDict
-        new_state_dict = OrderedDict()
-        for k, v in state_dict.items():
-            name = k[7:]  # remove `module.`
-            new_state_dict[name] = v
-        # load params
-        gaze_model.load_state_dict(new_state_dict)
-    gaze_model.eval()
-
-    if opt.fc_model or opt.use_fc_model:
-        face_classifier_model, fc_input_size = models.init_face_classifier(opt.device,
-                                                                           num_classes=2,
-                                                                           resume_from=path_to_fc_model)
-        face_classifier_model.eval()
-        face_classifier_model.to(opt.device)
-        face_classifier_data_transforms = models.get_fc_data_transforms(fc_input_size)
-    else:
-        face_classifier_model = None
-        face_classifier_data_transforms = None
-    # load face extractor model
-    face_detector_model = cv2.dnn.readNetFromCaffe(str(config_file), str(face_detector_model_file))    
-    return gaze_model, face_detector_model, face_classifier_model, face_classifier_data_transforms
-
-def get_video_paths(opt):
-    """
-    obtain the video paths (and possibly video ids) from the source argument
-    :param opt: command line options
-    :return: a list of video paths and a list of video ids
-    """
-    if opt.source_type == 'file':
-        video_path = Path(opt.source)
-        if video_path.is_dir():
-            logging.warning("Video folder provided as source. Make sure it contains video files only.")
-            video_paths = list(video_path.glob("*"))
-            if opt.video_filter:
-                filter_files = [x.stem for x in opt.video_filter.glob("*")]
-                video_paths = [x for x in video_paths if x.stem in filter_files]
-            video_paths = [str(x) for x in video_paths]
-        elif video_path.is_file():
-            video_paths = [str(video_path)]
-        else:
-            raise FileNotFoundError("Couldn't find a file or a directory at {}".format(video_path))
-    else:
-        # video_paths = [int(opt.source)]
-        raise NotImplementedError
-    return video_paths
-
-def create_output_streams(video_path, framerate, resolution, opt):
-    """
-    creates output streams
-    :param video_path: path to video
-    :param framerate: video framerate
-    :param resolution: video resolution
-    :param video_ids: list of video ids
-    :param opt: options
-    :return: video_output_file, prediction_output_file, skip = prediction file already exists
-    """
-    video_output_file = None
-    prediction_output_file = None
-    skip=False
-    if opt.output_video_path:
-        fourcc = cv2.VideoWriter_fourcc(*"MP4V")  # may need to be adjusted per available codecs & OS
-        my_video_path = Path(opt.output_video_path, video_path.stem + "_output.mp4")
-        video_output_file = cv2.VideoWriter(str(my_video_path), fourcc, framerate, resolution, True)
-    if opt.output_annotation:
-        if opt.output_format == "compressed":
-            prediction_output_file = Path(opt.output_annotation, video_path.stem)
-        else:
-            prediction_output_file = Path(opt.output_annotation, video_path.stem + opt.output_file_suffix)
-            if opt.output_format == "PrefLookTimestamp":
-                with open(prediction_output_file, "w", newline="") as f: # Write header
-                    f.write("Tracks: left, right, away, codingactive, outofframe\nTime,Duration,TrackName,comment\n\n")
-    return video_output_file, prediction_output_file, skip
-    
-def cleanup(video_output_file, prediction_output_file, answers, confidences, framerate, frame_count, cap, opt):
-    if opt.show_output:
-        cv2.destroyAllWindows()
-    if opt.output_video_path:
-        video_output_file.release()
-    if opt.output_annotation:  # write footer to file
-        if opt.output_format == "PrefLookTimestamp":
-            start_ms = int((1000. / framerate) * (opt.sliding_window_size // 2))
-            end_ms = int((1000. / framerate) * frame_count)
-            with open(prediction_output_file, "a", newline="") as f:
-                f.write("{},{},codingactive\n".format(start_ms, end_ms))
-        elif opt.output_format == "compressed":
-            np.savez(prediction_output_file, answers, confidences)
-    cap.release()
-
-def predict_from_video(opt):
-    """
-    perform prediction on a stream or video file(s) using a network.
-    output can be of various kinds, see options for details.
-    :param opt: command line arguments
-    :return:
-    """
-    # initialize
-    loc = -5  # where in the sliding window to take the prediction (should be a function of opt.sliding_window_size)
-    cursor = -5 # points to the frame we will write to output relative to current frame
-    classes = {'noface': -2, 'nobabyface': -1, 'away': 0, 'left': 1, 'right': 2}
-    reverse_classes = {-2: 'noface', -1: 'nobabyface', 0: 'away', 1: 'left', 2: 'right'}
-    logging.info("using the following values for per-channel mean: {}".format(opt.per_channel_mean))
-    logging.info("using the following values for per-channel std: {}".format(opt.per_channel_std))
-    gaze_model, face_detector_model, face_classifier_model, face_classifier_data_transforms = load_models(opt)
-    video_paths = get_video_paths(opt)
-    if opt.illegal_transitions_path:
-        illegal_transitions, corrected_transitions = parsers.parse_illegal_transitions_file(opt.illegal_transitions_path)
-        max_illegal_transition_length = max([len(transition) for transition in illegal_transitions])
-        cursor -= max_illegal_transition_length
-        if abs(cursor) > opt.sliding_window_size:
-            raise ValueError("illegal_transitions_path contains transitions longer than the sliding window size")
-    # loop over inputs
-    for i in range(len(video_paths)):
-        video_path = Path(str(video_paths[i]))
-        logging.info("predicting on : {}".format(video_path))
-        cap, framerate, resolution, h_start_at, h_end_at, w_start_at, w_end_at = process_video(video_path, opt)
-        video_output_file, prediction_output_file, skip = create_output_streams(video_path, framerate, resolution, opt)
-        if skip:
-            continue
-        # per video initialization
-        answers = []  # list of answers for each frame
-        confidences = []  # list of confidences for each frame
-        image_sequence = []  # list of (crop, valid) for each frame in the sliding window
-        box_sequence = []  # list of bounding boxes for each frame in the sliding window
-        bbox_sequence = []  # list of bounding boxes for each frame in the sliding window
-        frames = []  # list of frames for each frame in the sliding window
-        from_tracker = []  # list of booleans indicating whether the bounding box was obtained from the tracker
-        last_known_valid_bbox = None  # last known valid bounding box
-        frame_count = 0  # frame counter
-        hor, ver = 0.5, 1  # initial guess for face location
-        cur_fps = video.FPS()  # for debugging purposes
-        last_class_text = ""  # Initialize so that we see the first class assignment as an event to record
-        # loop over frames (refactor !)
-        ret_val, frame = cap.read()
-        while ret_val:
-            frame = draw.mask_regions(frame, h_start_at, h_end_at, w_start_at, w_end_at)  # mask roi
-            # frame = frame[h_start_at:, w_start_at:w_end_at, :]  # crop x% of the video from the top
-            frames.append(frame)
-            cv2_bboxes = detect_face_opencv_dnn(face_detector_model, frame, 0.7)
-            frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)  # network was trained on RGB images.
-            if not cv2_bboxes and (last_known_valid_bbox is None or not opt.track_face):
-                answers.append(classes['noface'])  # if face detector fails, treat as away and mark invalid
-                confidences.append(-1)
-                image = np.zeros((1, opt.image_size, opt.image_size, 3), np.float64)
-                my_box = np.array([0, 0, 0, 0, 0])
-                image_sequence.append((image, True))
-                box_sequence.append(my_box)
-                bbox_sequence.append(None)
-                from_tracker.append(False)
-            else:
-                if cv2_bboxes:
-                    from_tracker.append(False)
-                else:
-                    from_tracker.append(True)
-                    cv2_bboxes = [last_known_valid_bbox]
-                selected_bbox = select_face(cv2_bboxes, frame, face_classifier_model, face_classifier_data_transforms, hor, ver, opt.device)
-                crop, my_box = extract_crop(frame, selected_bbox, opt)
-                if selected_bbox is None:
-                    answers.append(classes['nobabyface'])  # if selecting face fails, treat as away and mark invalid
-                    confidences.append(-1)
-                    image = np.zeros((1, opt.image_size, opt.image_size, 3), np.float64)
-                    my_box = np.array([0, 0, 0, 0, 0])
-                    image_sequence.append((image, True))
-                    box_sequence.append(my_box)
-                    bbox_sequence.append(None)
-                else:
-                    assert crop.size != 0  # what just happened?
-                    answers.append(classes['left'])  # if face detector succeeds, treat as left and mark valid
-                    confidences.append(-1)
-                    image_sequence.append((crop, False))
-                    box_sequence.append(my_box)
-                    bbox_sequence.append(selected_bbox)
-                    if not from_tracker[-1]:
-                        last_known_valid_bbox = selected_bbox.copy()
-            if len(image_sequence) == opt.sliding_window_size:  # we have enough frames for prediction, predict for middle frame
-                cur_frame = frames[cursor]
-                cur_bbox = bbox_sequence[cursor]
-                is_from_tracker = from_tracker[cursor]
-                frames.pop(0)
-                bbox_sequence.pop(0)
-                from_tracker.pop(0)
-                if not image_sequence[opt.sliding_window_size // 2][1]:  # if middle image is valid
-                    to_predict = {"imgs": torch.tensor(np.array([x[0] for x in image_sequence[0::2]]), dtype=torch.float).squeeze().permute(0, 3, 1, 2).to(opt.device),
-                                    "boxs": torch.tensor(np.array(box_sequence[::2]), dtype=torch.float).to(opt.device)
-                                    }
-                    with torch.set_grad_enabled(False):
-                        outputs = gaze_model(to_predict)  # actual gaze prediction
-                        probs = torch.nn.functional.softmax(outputs, dim=1)
-                        _, prediction = torch.max(outputs, 1)
-                        confidence, _ = torch.max(probs, 1)
-                        float32_conf = confidence.cpu().numpy()[0]
-                        int32_pred = prediction.cpu().numpy()[0]
-                    answers[loc] = int32_pred  # update answers for the middle frame
-                    confidences[loc] = float32_conf  # update confidences for the middle frame
-                image_sequence.pop(0)
-                box_sequence.pop(0)
-
-                if opt.illegal_transitions_path:
-                    if len(answers) >= max_illegal_transition_length: 
-                        answers, confidences = fix_illegal_transitions(loc, answers, confidences, illegal_transitions, corrected_transitions)
-                class_text = reverse_classes[answers[cursor]]
-                if opt.on_off:
-                    class_text = "off" if class_text == "away" else "on"
-                if opt.output_video_path:
-                    if is_from_tracker and opt.track_face:
-                        rect_color = (0, 0, 255)
-                    else:
-                        rect_color = (0, 255, 0) 
-                    draw.prepare_frame(cur_frame, cur_bbox, show_arrow=True, rect_color=rect_color,
-                                         conf=confidences[cursor], class_text=class_text,
-                                         frame_number=frame_count, pic_in_pic=opt.pic_in_pic)
-                    video_output_file.write(cur_frame)
-                if opt.show_output:
-                    if is_from_tracker and opt.track_face:
-                        rect_color = (0, 0, 255)
-                    else:
-                        rect_color = (0, 255, 0) 
-                    draw.prepare_frame(cur_frame, cur_bbox, show_arrow=True, rect_color=rect_color,
-                                         conf=confidences[cursor], class_text=class_text,
-                                         frame_number=frame_count, pic_in_pic=opt.pic_in_pic)
-                    
-                    cv2.imshow('frame', cur_frame)
-                    if cv2.waitKey(1) & 0xFF == ord('q'):
-                        break
-                # handle writing output to file
-                if opt.output_annotation:
-                    if opt.output_format == "raw_output":
-                        with open(prediction_output_file, "a", newline="") as f:
-                            f.write("{}, {}, {:.02f}\n".format(str(frame_count + cursor + 1), class_text, confidences[cursor]))
-                    elif opt.output_format == "PrefLookTimestamp":
-                        if class_text != last_class_text:  # Record "event" for change of direction if code has changed
-                            frame_ms = int((frame_count + cursor + 1) * (1000. / framerate))
-                            with open(prediction_output_file, "a", newline="") as f:
-                                f.write("{},0,{}\n".format(frame_ms, class_text))
-                            last_class_text = class_text
-                logging.info("frame: {}, class: {}, confidence: {:.02f}, cur_fps: {:.02f}".format(str(frame_count + cursor + 1), class_text, confidences[cursor], cur_fps()))
-            ret_val, frame = cap.read()
-            frame_count += 1
-        # finished processing a video file, cleanup
-        cleanup(video_output_file, prediction_output_file, answers, confidences, framerate, frame_count, cap, opt)
-
-def main():
-    args = options.parse_arguments()
-    if args.log:
-        args.log.parent.mkdir(parents=True, exist_ok=True)
-        logging.basicConfig(filename=args.log, filemode='w', level=args.verbosity.upper())
-    else:
-        logging.basicConfig(level=args.verbosity.upper())
-    predict_from_video(args)
-
-if __name__ == "__main__":
-    main()
+import logging
+import torch
+import numpy as np
+import cv2
+from PIL import Image
+from pathlib import Path
+import pooch
+from icatcher import version, classes, reverse_classes, options, draw, video, models, parsers
+from icatcher.face_detector import extract_bboxes, process_frames, parallelize_face_detection, detect_face_opencv_dnn
+from pathos.helpers import cpu_count
+from batch_face import RetinaFace
+
+
+def select_face(bboxes, frame, fc_model, fc_data_transforms, hor, ver, device):
+    """
+    selects a correct face from candidates bbox in frame
+    :param bboxes: the bounding boxes of candidates
+    :param frame: the frame
+    :param fc_model: a classifier model, if passed it is used to decide.
+    :param fc_data_transforms: the transformations to apply to the images before fc_model sees them
+    :param hor: the last known horizontal correct face location
+    :param ver: the last known vertical correct face location
+    :return: the cropped face and its bbox data
+    """
+    if fc_model:
+        centers = []
+        faces = []
+        for box in bboxes:
+            crop_img = frame[box[1]:box[1] + box[3], box[0]:box[0] + box[2]]
+            face_box = np.array([box[1], box[1] + box[3], box[0], box[0] + box[2]])
+            img_shape = np.array(frame.shape)
+            ratio = np.array([face_box[0] / img_shape[0], face_box[1] / img_shape[0],
+                              face_box[2] / img_shape[1], face_box[3] / img_shape[1]])
+            face_ver = (ratio[0] + ratio[1]) / 2
+            face_hor = (ratio[2] + ratio[3]) / 2
+
+            centers.append([face_hor, face_ver])
+            img = crop_img
+            img = fc_data_transforms['val'](img)
+            faces.append(img)
+        centers = np.stack(centers)
+        faces = torch.stack(faces).to(device)
+        output = fc_model(faces)
+        _, preds = torch.max(output, 1)
+        preds = preds.cpu().numpy()
+        idxs = np.where(preds == 0)[0]
+        if idxs.size == 0:
+            bbox = None
+        else:
+            centers = centers[idxs]
+            dis = np.sqrt((centers[:, 0] - hor) ** 2 + (centers[:, 1] - ver) ** 2)
+            i = np.argmin(dis)
+            # crop_img = faces[idxs[i]]
+            bbox = bboxes[idxs[i]]
+            # hor, ver = centers[i]
+    else:   # select face based on a mix of the lowest face and the width ratio of the face
+        bbox = None
+        prev_score = 0
+        for box in bboxes:
+            top_left_x, top_left_y, width, height = box
+            # make sure not dividing by zero
+            if width == 0 or height == 0:
+                continue
+            else:
+                # find min ratio of width and height which will weight box score
+                min_ratio = min(width, height) / max(width, height)
+                box_bottom = top_left_y + height
+                box_score = min_ratio * box_bottom
+    
+                # check if score outweighs previous bounding boxes
+                if box_score > prev_score:
+                    prev_score = box_score
+                    bbox = box
+    return bbox
+
+def fix_illegal_transitions(loc, answers, confidences, illegal_transitions, corrected_transitions):
+    """
+    fixes illegal transitions happening in answers at [loc-max_trans_len+1, loc] inclusive
+    """
+    for i, transition in enumerate(illegal_transitions):
+        len_trans = len(transition)
+        buffer = answers[loc-len_trans+1:loc+1]
+        if buffer == transition:
+            buffer_update = corrected_transitions[i]
+            answers[loc-len_trans+1:loc+1] = buffer_update
+            buffer_splits = np.where(np.array(buffer_update) != np.array(buffer))
+            for spot in buffer_splits[0].tolist():
+                confidences[loc - len_trans + 1 + spot] = -1
+    return answers, confidences
+
+def extract_crop(frame, bbox, opt):
+    """
+    extracts a crop from a frame using bbox, and transforms it
+    :param frame: the frame
+    :param bbox: opencv bbox 4x1
+    :param opt: command line options
+    :return: the crop and the 5x1 box features
+    """
+    if bbox is None:
+        return None, None
+
+    # make sure no negatives being fed into extract crop
+    bbox = [0 if x < 0 else x for x in bbox]
+
+    img_shape = np.array(frame.shape)
+    face_box = np.array([bbox[1], bbox[1] + bbox[3], bbox[0], bbox[0] + bbox[2]])
+    crop = frame[bbox[1]:bbox[1] + bbox[3], bbox[0]:bbox[0] + bbox[2]]
+
+    test_transforms = models.DataTransforms(opt.image_size,
+                                          opt.per_channel_mean,
+                                          opt.per_channel_std).transformations["test"]
+    crop = test_transforms(Image.fromarray(crop))
+    crop = crop.permute(1, 2, 0).unsqueeze(0).numpy()
+    ratio = np.array([face_box[0] / img_shape[0], face_box[1] / img_shape[0],
+                      face_box[2] / img_shape[1], face_box[3] / img_shape[1]])
+    face_size = (ratio[1] - ratio[0]) * (ratio[3] - ratio[2])
+    face_ver = (ratio[0] + ratio[1]) / 2
+    face_hor = (ratio[2] + ratio[3]) / 2
+    face_height = ratio[1] - ratio[0]
+    face_width = ratio[3] - ratio[2]
+    my_box = np.array([face_size, face_ver, face_hor, face_height, face_width])
+    return crop, my_box
+
+def load_models(opt):
+    """
+    loads all relevant neural network models to perform predictions
+    models will be automatically downloaded if not found in the cache,
+    user may overide downloaded location with the env variable ICATCHER_DATA_DIR
+    defaults:
+    :Mac: "~/Library/Caches/<AppName>"
+    :Unix: "~/.cache/<AppName>" or the value of the "XDG_CACHE_HOME"
+    environment variable, if defined.
+    :Windows: "C:\\Users\\<user>\\AppData\\Local\\<AppAuthor>\\<AppName>\\Cache"
+    :param opt: command line options
+    :return all nn models
+    """
+    GOODBOY = pooch.create(path=pooch.os_cache("icatcher_plus"),
+                           base_url="https://osf.io/h7svp/download",
+                           version=version,
+                           version_dev="main",
+                           env="ICATCHER_DATA_DIR",
+                           registry={"zip_content.txt": None,
+                                     "icatcher+_models.zip": None},
+                           urls={"zip_content.txt":"https://osf.io/v4w53/download",
+                                 "icatcher+_models.zip":"https://osf.io/h7svp/download"})
+    # zip_content_file = GOODBOY.fetch("zip_content.txt")
+    # with open(zip_content_file, "r") as f:
+        # zip_content = [x.strip() for x in f]
+    file_paths = GOODBOY.fetch("icatcher+_models.zip",
+                               processor=pooch.Unzip(),
+                               progressbar=True)
+    file_names = [Path(x).name for x in file_paths]
+    if opt.fd_model == "retinaface":  # option for retina face vs. previous opencv dnn model
+        face_detector_model_file = file_paths[file_names.index("Resnet50_Final.pth")]
+        face_detector_model = RetinaFace(
+            gpu_id=opt.gpu_id, model_path=face_detector_model_file, network="resnet50"
+        )
+    elif opt.fd_model == "opencv_dnn":
+        face_detector_model_file = file_paths[file_names.index("face_model.caffemodel")]
+        config_file = file_paths[file_names.index("config.prototxt")]
+        face_detector_model = cv2.dnn.readNetFromCaffe(str(config_file), str(face_detector_model_file))
+    else:
+        raise NotImplementedError
+    path_to_gaze_model = file_paths[file_names.index("icatcher+_lookit.pth")]
+    if opt.model:
+        path_to_gaze_model = opt.model
+    path_to_fc_model = file_paths[file_names.index("face_classifier_lookit.pth")]
+    if opt.fc_model:
+        path_to_fc_model = opt.fc_model
+    # face_detector_model_file = Path("models", "face_model.caffemodel")
+    # config_file = Path("models", "config.prototxt")
+    # path_to_gaze_model = opt.model
+    gaze_model = models.GazeCodingModel(opt).to(opt.device)
+    if opt.device == 'cpu':
+        state_dict = torch.load(str(path_to_gaze_model), map_location=torch.device(opt.device))
+    else:
+        state_dict = torch.load(str(path_to_gaze_model))
+    try:
+        gaze_model.load_state_dict(state_dict)
+    except RuntimeError as e:  # hack to deal with models trained on distributed setup
+        from collections import OrderedDict
+        new_state_dict = OrderedDict()
+        for k, v in state_dict.items():
+            name = k[7:]  # remove `module.`
+            new_state_dict[name] = v
+        # load params
+        gaze_model.load_state_dict(new_state_dict)
+    gaze_model.eval()
+
+    if opt.fc_model or opt.use_fc_model:
+        face_classifier_model, fc_input_size = models.init_face_classifier(opt.device,
+                                                                           num_classes=2,
+                                                                           resume_from=path_to_fc_model)
+        face_classifier_model.eval()
+        face_classifier_model.to(opt.device)
+        face_classifier_data_transforms = models.get_fc_data_transforms(fc_input_size)
+    else:
+        face_classifier_model = None
+        face_classifier_data_transforms = None
+    return gaze_model, face_detector_model, face_classifier_model, face_classifier_data_transforms
+
+def create_output_streams(video_path, framerate, resolution, opt):
+    """
+    creates output streams
+    :param video_path: path to video
+    :param framerate: video framerate
+    :param resolution: video resolution
+    :param opt: options
+    :return: video_output_file, prediction_output_file, skip = prediction file already exists
+    """
+    video_output_file = None
+    prediction_output_file = None
+    skip=False
+    if opt.output_video_path:
+        fourcc = cv2.VideoWriter_fourcc(*"MP4V")  # may need to be adjusted per available codecs & OS
+        my_video_path = Path(opt.output_video_path, video_path.stem + "_output.mp4")
+        video_output_file = cv2.VideoWriter(str(my_video_path), fourcc, framerate, resolution, True)
+    if opt.output_annotation:
+        if opt.output_format == "compressed":
+            prediction_output_file = Path(opt.output_annotation, video_path.stem)
+        else:
+            prediction_output_file = Path(opt.output_annotation, video_path.stem + opt.output_file_suffix)
+            if opt.output_format == "PrefLookTimestamp":
+                with open(prediction_output_file, "w", newline="") as f: # Write header
+                    f.write("Tracks: left, right, away, codingactive, outofframe\nTime,Duration,TrackName,comment\n\n")
+    return video_output_file, prediction_output_file, skip
+    
+def predict_from_video(opt):
+    """
+    perform prediction on a stream or video file(s) using a network.
+    output can be of various kinds, see options for details.
+    :param opt: command line arguments
+    :return:
+    """
+    # initialize
+    loc = -5  # where in the sliding window to take the prediction (should be a function of opt.sliding_window_size)
+    cursor = -5 # points to the frame we will write to output relative to current frame
+    logging.debug("using the following values for per-channel mean: {}".format(opt.per_channel_mean))
+    logging.debug("using the following values for per-channel std: {}".format(opt.per_channel_std))
+    gaze_model, face_detector_model, face_classifier_model, face_classifier_data_transforms = load_models(opt)
+    video_paths = video.get_video_paths(opt)
+    if opt.illegal_transitions_path:
+        illegal_transitions, corrected_transitions = parsers.parse_illegal_transitions_file(opt.illegal_transitions_path)
+        max_illegal_transition_length = max([len(transition) for transition in illegal_transitions])
+        cursor -= max_illegal_transition_length  # slide cursor back so all illegal transitions can be fixed on the fly
+        if abs(cursor) > opt.sliding_window_size:
+            raise ValueError("illegal_transitions_path contains transitions longer than the sliding window size")
+    # check if cpu or gpu being used
+    use_cpu = True if opt.gpu_id == -1 else False
+    # loop over inputs
+    for i in range(len(video_paths)):
+        video_path = Path(str(video_paths[i]))
+        logging.debug("predicting on : {}".format(video_path))
+        cap, framerate, resolution, h_start_at, h_end_at, w_start_at, w_end_at = video.process_video(video_path, opt)
+        video_output_file, prediction_output_file, skip = create_output_streams(video_path, framerate, resolution, opt)
+        if skip:
+            continue
+        # per video initialization
+        answers = []  # list of answers for each frame
+        confidences = []  # list of confidences for each frame
+        image_sequence = []  # list of (crop, valid) for each frame in the sliding window
+        box_sequence = []  # list of bounding boxes for each frame in the sliding window
+        bbox_sequence = []  # list of bounding boxes for each frame in the sliding window
+        frames = []  # list of frames for each frame in the sliding window
+        from_tracker = []  # list of booleans indicating whether the bounding box was obtained from the tracker
+        last_known_valid_bbox = None  # last known valid bounding box
+        frame_count = 0  # frame counter
+        hor, ver = 0.5, 1  # initial guess for face location
+        cur_fps = video.FPS()  # for debugging purposes
+        last_class_text = ""  # Initialize so that we see the first class assignment as an event to record
+
+        # if going to use cpu parallelization, don't allow for live stream video
+        if use_cpu and opt.fd_model == "retinaface" and not opt.dont_buffer:
+            # figure out how many cpus can be used
+            num_cpus = cpu_count() - opt.num_cpus_saved
+            assert num_cpus > 0
+
+            # send all frames in to be preprocessed and have faces detected prior to running gaze detection
+            total_frames = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
+            vid_frames = range(0, total_frames, 1 + opt.fd_skip_frames)  # adding step if frames are skipped
+            processed_frames = process_frames(cap, vid_frames, h_start_at, h_end_at, w_start_at, w_end_at)
+            frame_height, frame_width = processed_frames[0].shape[0], processed_frames[0].shape[1]
+            logging.debug("face detection on buffered frames ...")
+            faces = parallelize_face_detection(processed_frames, face_detector_model, num_cpus, opt)
+            del processed_frames
+
+            # flatten the list and extract bounding boxes
+            faces = [item for sublist in faces for item in sublist]
+            master_bboxes = [extract_bboxes(face_group, frame_height, frame_width) for face_group in faces]
+
+            # if frames were skipped, need to repeat binding boxes for that many skips
+            if opt.fd_skip_frames > 0:
+                master_bboxes = np.repeat(master_bboxes, opt.fd_skip_frames + 1)
+
+            cap.set(cv2.CAP_PROP_POS_FRAMES, 0)  # reset frames to 0
+
+        # loop over frames (refactor !)
+        ret_val, frame = cap.read()
+        frame_height, frame_width = frame.shape[0], frame.shape[1]
+        while ret_val:
+            frame = draw.mask_regions(frame, h_start_at, h_end_at, w_start_at, w_end_at)  # mask roi
+            frames.append(frame)
+
+            if use_cpu and opt.fd_model == "retinaface" and not opt.dont_buffer:  # if using cpu, just pull from master
+                bboxes = master_bboxes[frame_count]
+            elif opt.fd_model == "opencv_dnn":
+                bboxes = detect_face_opencv_dnn(face_detector_model, frame, opt.fd_confidence_threshold)
+            else:  # uses retina face, if using gpu, find face as frame is processed... don't need batch inference
+                faces = face_detector_model(frame)
+                faces = [face for face in faces if face[-1] >= opt.fd_confidence_threshold]
+                bboxes = extract_bboxes(faces, frame_height, frame_width)
+            frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)  # network was trained on RGB images.
+            if not bboxes and (last_known_valid_bbox is None or not opt.track_face):
+                answers.append(classes['noface'])  # if face detector fails, treat as away and mark invalid
+                confidences.append(-1)
+                image = np.zeros((1, opt.image_size, opt.image_size, 3), np.float64)
+                my_box = np.array([0, 0, 0, 0, 0])
+                image_sequence.append((image, True))
+                box_sequence.append(my_box)
+                bbox_sequence.append(None)
+                from_tracker.append(False)
+            else:
+                if bboxes:
+                    from_tracker.append(False)
+                else:
+                    from_tracker.append(True)
+                    bboxes = [last_known_valid_bbox]
+                selected_bbox = select_face(bboxes, frame, face_classifier_model, face_classifier_data_transforms, hor, ver, opt.device)
+                crop, my_box = extract_crop(frame, selected_bbox, opt)
+                if selected_bbox is None:
+                    answers.append(classes['nobabyface'])  # if selecting face fails, treat as away and mark invalid
+                    confidences.append(-1)
+                    image = np.zeros((1, opt.image_size, opt.image_size, 3), np.float64)
+                    my_box = np.array([0, 0, 0, 0, 0])
+                    image_sequence.append((image, True))
+                    box_sequence.append(my_box)
+                    bbox_sequence.append(None)
+                else:
+                    if crop.size == 0:
+                        raise ValueError("crop size is 0, what just happend?")
+                    answers.append(classes['left'])  # if face detector succeeds, treat as left and mark valid
+                    confidences.append(-1)
+                    image_sequence.append((crop, False))
+                    box_sequence.append(my_box)
+                    bbox_sequence.append(selected_bbox)
+                    if not from_tracker[-1]:
+                        last_known_valid_bbox = selected_bbox.copy()
+            if len(image_sequence) == opt.sliding_window_size:  # we have enough frames for prediction, predict for middle frame
+                cur_frame = frames[cursor]
+                cur_bbox = bbox_sequence[cursor]
+                is_from_tracker = from_tracker[cursor]
+                frames.pop(0)
+                bbox_sequence.pop(0)
+                from_tracker.pop(0)
+                if not image_sequence[opt.sliding_window_size // 2][1]:  # if middle image is valid
+                    to_predict = {"imgs": torch.tensor(np.array([x[0] for x in image_sequence[0::2]]), dtype=torch.float).squeeze().permute(0, 3, 1, 2).to(opt.device),
+                                    "boxs": torch.tensor(np.array(box_sequence[::2]), dtype=torch.float).to(opt.device)
+                                    }
+                    with torch.set_grad_enabled(False):
+                        outputs = gaze_model(to_predict)  # actual gaze prediction
+                        probs = torch.nn.functional.softmax(outputs, dim=1)
+                        _, prediction = torch.max(outputs, 1)
+                        confidence, _ = torch.max(probs, 1)
+                        float32_conf = confidence.cpu().numpy()[0]
+                        int32_pred = prediction.cpu().numpy()[0]
+                    answers[loc] = int32_pred  # update answers for the middle frame
+                    confidences[loc] = float32_conf  # update confidences for the middle frame
+                image_sequence.pop(0)
+                box_sequence.pop(0)
+
+                if opt.illegal_transitions_path:
+                    if len(answers) >= max_illegal_transition_length: 
+                        answers, confidences = fix_illegal_transitions(loc, answers, confidences, illegal_transitions, corrected_transitions)
+                class_text = reverse_classes[answers[cursor]]
+                if opt.on_off:
+                    class_text = "off" if class_text == "away" else "on"
+                if opt.output_video_path:
+                    if is_from_tracker and opt.track_face:
+                        rect_color = (0, 0, 255)
+                    else:
+                        rect_color = (0, 255, 0) 
+                    draw.prepare_frame(cur_frame, cur_bbox, show_arrow=True, rect_color=rect_color,
+                                         conf=confidences[cursor], class_text=class_text,
+                                         frame_number=frame_count, pic_in_pic=opt.pic_in_pic)
+                    video_output_file.write(cur_frame)
+                if opt.show_output:
+                    if is_from_tracker and opt.track_face:
+                        rect_color = (0, 0, 255)
+                    else:
+                        rect_color = (0, 255, 0)
+                    draw.prepare_frame(cur_frame, cur_bbox, show_arrow=True, rect_color=rect_color,
+                                         conf=confidences[cursor], class_text=class_text,
+                                         frame_number=frame_count, pic_in_pic=opt.pic_in_pic)
+                    
+                    cv2.imshow('frame', cur_frame)
+                    if cv2.waitKey(1) & 0xFF == ord('q'):
+                        break
+                # handle writing output to file
+                if opt.output_annotation:
+                    if opt.output_format == "raw_output":
+                        with open(prediction_output_file, "a", newline="") as f:
+                            f.write("{}, {}, {:.02f}\n".format(str(frame_count + cursor + 1), class_text, confidences[cursor]))
+                    elif opt.output_format == "PrefLookTimestamp":
+                        if class_text != last_class_text:  # Record "event" for change of direction if code has changed
+                            frame_ms = int((frame_count + cursor + 1) * (1000. / framerate))
+                            with open(prediction_output_file, "a", newline="") as f:
+                                f.write("{},0,{}\n".format(frame_ms, class_text))
+                            last_class_text = class_text
+                logging.info("frame: {}, class: {}, confidence: {:.02f}, cur_fps: {:.02f}".format(str(frame_count + cursor + 1), class_text, confidences[cursor], cur_fps()))
+            ret_val, frame = cap.read()
+            frame_count += 1
+        # finished processing a video file, cleanup
+        cleanup(video_output_file, prediction_output_file, answers, confidences, framerate, frame_count, cap, opt)
+
+def cleanup(video_output_file, prediction_output_file, answers, confidences, framerate, frame_count, cap, opt):
+    if opt.show_output:
+        cv2.destroyAllWindows()
+    if opt.output_video_path:
+        video_output_file.release()
+    if opt.output_annotation:  # write footer to file
+        if opt.output_format == "PrefLookTimestamp":
+            start_ms = int((1000. / framerate) * (opt.sliding_window_size // 2))
+            end_ms = int((1000. / framerate) * frame_count)
+            with open(prediction_output_file, "a", newline="") as f:
+                f.write("{},{},codingactive\n".format(start_ms, end_ms))
+        elif opt.output_format == "compressed":
+            np.savez(prediction_output_file, answers, confidences)
+    cap.release()
+
+def main():
+    args = options.parse_arguments()
+    if args.log:
+        args.log.parent.mkdir(parents=True, exist_ok=True)
+        logging.basicConfig(filename=args.log, filemode='w', level=args.verbosity.upper())
+    else:
+        logging.basicConfig(level=args.verbosity.upper())
+    predict_from_video(args)
+
+if __name__ == "__main__":
+    main()
```

### Comparing `icatcher-0.0.9/src/icatcher/draw.py` & `icatcher-0.1.0/src/icatcher/draw.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,123 +1,123 @@
-import cv2
-import numpy as np
-
-
-def put_text(img, text, loc=None):
-    """
-    inserts a text into image
-    :param img:
-    :param class_name:
-    :param loc:
-    :return:
-    """
-    font = cv2.FONT_HERSHEY_DUPLEX
-    if loc is not None:
-        text_location = loc
-    else:
-        text_location = (10, 30)  # top_left_corner_text
-    font_scale = 1
-    font_color = (255, 255, 255)
-    bg_color = (0,0,0)
-    line_type = 2
-    
-    text_size, _ = cv2.getTextSize(text, font, font_scale, line_type)
-    text_w, text_h = text_size
-    
-    cv2.rectangle(img, text_location, (text_location[0] + text_w, text_location[1] + text_h), bg_color, -1)
-
-    cv2.putText(img, text, (text_location[0], text_location[1] + text_h + font_scale - 1),
-                font,
-                font_scale,
-                font_color,
-                line_type)
-    
-    return img
-
-def put_arrow(img, class_name, face):
-    """
-    inserts an arrow into a frame
-    :param img: the frame
-    :param class_name: this will dictate where the arrow will face
-    :param face: bounding box of face in frame
-    :return: the frame with an arrow
-    """
-    arrow_start_x = int(face[0] + 0.5 * face[2])
-    arrow_end_x = int(face[0] + 0.1 * face[2] if class_name == "left" else face[0] + 0.9 * face[2])
-    arrow_y = int(face[1] + 0.8 * face[3])
-    img = cv2.arrowedLine(img,
-                          (arrow_start_x, arrow_y),
-                          (arrow_end_x, arrow_y),
-                          (0, 255, 0),
-                          thickness=3,
-                          tipLength=0.4)
-    return img
-
-def put_rectangle(frame, rec, color=None):
-    """
-    inserts a rectangle in frame
-    :param frame: the frame
-    :param rec: the bounding box of the rectangle
-    :return:
-    """
-    if color is None:
-        color = (0, 255, 0)  # green
-    thickness = 2
-    frame = cv2.rectangle(frame,
-                          (rec[0], rec[1]), (rec[0] + rec[2], rec[1] + rec[3]),
-                          color,
-                          thickness)
-    return frame
-
-def prepare_frame(frame, bbox, show_bbox=True, show_arrow=False, conf=None, class_text=None, rect_color=None, frame_number=None, pic_in_pic=False):
-    """
-    prepares a frame for visualization by adding text, rectangles and arrows.
-    :param frame: the frame for which to add the gizmo's to
-    :param bbox: bbox as in cv2
-    :param show_bbox: to show bbox on face as a green rectangle
-    :param show_arrow: to show arrow indicating direciton of looking
-    :param conf: confidence of the classifier
-    :param class_text: class text to show on top left corner
-    :param rect_color: color of the rectangle
-    :param frame_number: frame number to show on top left corner
-    :param pic_in_pic: to show a small frame of the face
-    :return:
-    """
-    if show_arrow:
-        if class_text is not None:
-            if class_text == "right" or class_text == "left":
-                frame = put_arrow(frame, class_text, bbox)
-    if conf and bbox is not None:
-        frame = put_text(frame, "{:.02f}".format(conf),
-                         loc=(bbox[0], bbox[1] + bbox[3]))
-    if pic_in_pic:
-        pic_in_pic_size = 100
-        if bbox is None:
-            crop_img = np.zeros((pic_in_pic_size, pic_in_pic_size, 3), np.uint8)
-        else:
-            crop_img = frame[bbox[1]:bbox[1] + bbox[3], bbox[0]:bbox[0] + bbox[2]]
-            crop_img = cv2.resize(crop_img, (pic_in_pic_size, pic_in_pic_size))
-        frame[frame.shape[0]-pic_in_pic_size:, :pic_in_pic_size] = crop_img
-    if class_text is not None:
-        frame = put_text(frame, class_text)
-    if show_bbox and bbox is not None:
-        frame = put_rectangle(frame, bbox, rect_color)
-    if frame_number is not None:  # may fail if loc outside resolution
-        frame = put_text(frame, str(frame_number), loc=(10,70))
-    return frame
-
-def mask_regions(image, start_h, end_h, start_w, end_w):
-    """
-    masks a numpy image with black background outside of region of interest (roi)
-    :param image: numpy image h x w x c
-    :param start_h: where does the roi height start
-    :param end_h: where does the roi height end
-    :param start_w: where does the roi width start
-    :param end_w: where does the roi width end
-    :return: masked image
-    """
-    h, w, _ = image.shape
-    if start_h < 0 or start_w < 0 or end_h > h or end_w > w:
-        raise ValueError("Values exceed image resolution")
-    output = np.zeros_like(image)
-    output[start_h:end_h, start_w:end_w, :] = image[start_h:end_h, start_w:end_w, :]
-    return output
+import cv2
+import numpy as np
+
+
+def put_text(img, text, loc=None):
+    """
+    inserts a text into image
+    :param img:
+    :param class_name:
+    :param loc:
+    :return:
+    """
+    font = cv2.FONT_HERSHEY_DUPLEX
+    if loc is not None:
+        text_location = loc
+    else:
+        text_location = (10, 30)  # top_left_corner_text
+    font_scale = 1
+    font_color = (255, 255, 255)
+    bg_color = (0,0,0)
+    line_type = 2
+    
+    text_size, _ = cv2.getTextSize(text, font, font_scale, line_type)
+    text_w, text_h = text_size
+    
+    cv2.rectangle(img, text_location, (text_location[0] + text_w, text_location[1] + text_h), bg_color, -1)
+
+    cv2.putText(img, text, (text_location[0], text_location[1] + text_h + font_scale - 1),
+                font,
+                font_scale,
+                font_color,
+                line_type)
+    
+    return img
+
+def put_arrow(img, class_name, face):
+    """
+    inserts an arrow into a frame
+    :param img: the frame
+    :param class_name: this will dictate where the arrow will face
+    :param face: bounding box of face in frame
+    :return: the frame with an arrow
+    """
+    arrow_start_x = int(face[0] + 0.5 * face[2])
+    arrow_end_x = int(face[0] + 0.1 * face[2] if class_name == "left" else face[0] + 0.9 * face[2])
+    arrow_y = int(face[1] + 0.8 * face[3])
+    img = cv2.arrowedLine(img,
+                          (arrow_start_x, arrow_y),
+                          (arrow_end_x, arrow_y),
+                          (0, 255, 0),
+                          thickness=3,
+                          tipLength=0.4)
+    return img
+
+def put_rectangle(frame, rec, color=None):
+    """
+    inserts a rectangle in frame
+    :param frame: the frame
+    :param rec: the bounding box of the rectangle
+    :return:
+    """
+    if color is None:
+        color = (0, 255, 0)  # green
+    thickness = 2
+    frame = cv2.rectangle(frame,
+                          (rec[0], rec[1]), (rec[0] + rec[2], rec[1] + rec[3]),
+                          color,
+                          thickness)
+    return frame
+
+def prepare_frame(frame, bbox, show_bbox=True, show_arrow=False, conf=None, class_text=None, rect_color=None, frame_number=None, pic_in_pic=False):
+    """
+    prepares a frame for visualization by adding text, rectangles and arrows.
+    :param frame: the frame for which to add the gizmo's to
+    :param bbox: bbox as in cv2
+    :param show_bbox: to show bbox on face as a green rectangle
+    :param show_arrow: to show arrow indicating direciton of looking
+    :param conf: confidence of the classifier
+    :param class_text: class text to show on top left corner
+    :param rect_color: color of the rectangle
+    :param frame_number: frame number to show on top left corner
+    :param pic_in_pic: to show a small frame of the face
+    :return:
+    """
+    if show_arrow:
+        if class_text is not None and bbox is not None:
+            if class_text == "right" or class_text == "left":
+                frame = put_arrow(frame, class_text, bbox)
+    if conf and bbox is not None:
+        frame = put_text(frame, "{:.02f}".format(conf),
+                         loc=(bbox[0], bbox[1] + bbox[3]))
+    if pic_in_pic:
+        pic_in_pic_size = 100
+        if bbox is None:
+            crop_img = np.zeros((pic_in_pic_size, pic_in_pic_size, 3), np.uint8)
+        else:
+            crop_img = frame[bbox[1]:bbox[1] + bbox[3], bbox[0]:bbox[0] + bbox[2]]
+            crop_img = cv2.resize(crop_img, (pic_in_pic_size, pic_in_pic_size))
+        frame[frame.shape[0]-pic_in_pic_size:, :pic_in_pic_size] = crop_img
+    if class_text is not None:
+        frame = put_text(frame, class_text)
+    if show_bbox and bbox is not None:
+        frame = put_rectangle(frame, bbox, rect_color)
+    if frame_number is not None:  # may fail if loc outside resolution
+        frame = put_text(frame, str(frame_number), loc=(10,70))
+    return frame
+
+def mask_regions(image, start_h, end_h, start_w, end_w):
+    """
+    masks a numpy image with black background outside of region of interest (roi)
+    :param image: numpy image h x w x c
+    :param start_h: where does the roi height start
+    :param end_h: where does the roi height end
+    :param start_w: where does the roi width start
+    :param end_w: where does the roi width end
+    :return: masked image
+    """
+    h, w, _ = image.shape
+    if start_h < 0 or start_w < 0 or end_h > h or end_w > w:
+        raise ValueError("Values exceed image resolution")
+    output = np.zeros_like(image)
+    output[start_h:end_h, start_w:end_w, :] = image[start_h:end_h, start_w:end_w, :]
+    return output
```

### Comparing `icatcher-0.0.9/src/icatcher/models.py` & `icatcher-0.1.0/src/icatcher/models.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,123 +1,123 @@
-import torch
-import torch.nn.functional as F
-from torchvision.models.resnet import resnet18
-from torchvision.models import vgg16
-from torchvision import transforms
-
-
-def get_fc_data_transforms(input_size, dt_key=None):
-    if dt_key is not None and dt_key != 'train':
-        return {dt_key: transforms.Compose([
-            transforms.ToTensor(),
-            transforms.Resize((input_size, input_size), antialias=True),
-            transforms.CenterCrop(input_size),
-            transforms.Normalize([0.485, 0.456, 0.406], [0.229, 0.224, 0.225])
-        ])}
-    # Apply data augmentation
-    aug_list = []
-    aug_list.append(transforms.ToTensor())
-    aug_list.append(transforms.Resize((input_size, input_size), antialias=True))
-    aug_list.append(transforms.Normalize([0.485, 0.456, 0.406], [0.229, 0.224, 0.225]))
-    aug_transform = transforms.Compose(aug_list)
-
-    # Define data transformation on train, val, test set respectively
-    data_transforms = {
-        'train': aug_transform,
-        'val': transforms.Compose([
-            transforms.ToTensor(),
-            transforms.Resize((input_size, input_size), antialias=True),
-            transforms.CenterCrop(input_size),
-            transforms.Normalize([0.485, 0.456, 0.406], [0.229, 0.224, 0.225])
-        ]),
-    }
-    return data_transforms
-
-
-def init_face_classifier(device, num_classes=2, resume_from=None):
-    input_size = 100
-    model = vgg16(num_classes=num_classes)
-    num_ftrs = model.classifier[6].in_features
-    model.classifier[6] = torch.nn.Linear(num_ftrs, num_classes)
-    if resume_from is not None:
-        print("Loading weights from %s" % resume_from)
-        model.load_state_dict(torch.load(resume_from, map_location=device))
-    return model, input_size
-
-
-
-class DataTransforms:
-    def __init__(self, img_size, mean, std):
-        self.transformations = {
-            'train': transforms.Compose([
-                transforms.Resize((img_size, img_size)),
-                transforms.ColorJitter(brightness=0.2, contrast=0.2, saturation=0.2, hue=0.05),
-                transforms.ToTensor(),
-                transforms.Normalize(mean, std)
-                # transforms.RandomErasing()
-            ]),
-            'val': transforms.Compose([
-                transforms.Resize((img_size, img_size)),
-                transforms.ToTensor(),
-                transforms.Normalize(mean, std)
-            ]),
-            'test': transforms.Compose([
-                transforms.Resize((img_size, img_size)),
-                transforms.ToTensor(),
-                transforms.Normalize(mean, std)
-            ])
-        }
-
-class Predictor_fc(torch.nn.Module):
-    def __init__(self, n, add_box):
-        super().__init__()
-        in_channel = 512 * n if add_box else 256 * n
-        self.fc1 = torch.nn.Linear(in_channel, 512)
-        self.fc2 = torch.nn.Linear(512, 512)
-        self.fc3 = torch.nn.Linear(512, 3)
-        self.bn1 = torch.nn.BatchNorm1d(512)
-        self.bn2 = torch.nn.BatchNorm1d(512)
-        self.dropout1 = torch.nn.Dropout(0.2)
-        self.dropout2 = torch.nn.Dropout(0.2)
-
-    def forward(self, x):
-        x = self.fc1(x.view(x.size(0), -1))
-        x = self.dropout1(F.relu(self.bn1(x)))
-        x = self.fc2(x)
-        x = self.dropout2(F.relu(self.bn2(x)))
-        x = self.fc3(x)
-        return x
-
-class Encoder_box(torch.nn.Module):
-    def __init__(self):
-        super().__init__()
-        self.fc1 = torch.nn.Linear(5, 256)
-        self.fc2 = torch.nn.Linear(256, 256)
-        self.bn = torch.nn.BatchNorm1d(256)
-        self.dropout = torch.nn.Dropout(0.2)
-
-    def forward(self, x):
-        x = self.fc1(x)
-        x = self.dropout(F.relu(self.bn(x)))
-        x = self.fc2(x)
-
-        return x
-
-class GazeCodingModel(torch.nn.Module):
-    def __init__(self, args, add_box=True):
-        super().__init__()
-        self.args = args
-        self.n = (args.sliding_window_size + 1) // args.window_stride
-        self.add_box = add_box
-        self.encoder_img = resnet18(num_classes=256).to(self.args.device)
-        self.encoder_box = Encoder_box().to(self.args.device)
-        self.predictor = Predictor_fc(self.n, add_box).to(self.args.device)
-
-    def forward(self, data):
-        imgs = data['imgs']  # bs x n x 3 x 100 x 100
-        boxs = data['boxs']  # bs x n x 5
-        embedding = self.encoder_img(imgs.view(-1, 3, 100, 100)).view(-1, self.n, 256)
-        if self.add_box:
-            box_embedding = self.encoder_box(boxs.view(-1, 5)).view(-1, self.n, 256)
-            embedding = torch.cat([embedding, box_embedding], -1)
-        pred = self.predictor(embedding)
+import torch
+import torch.nn.functional as F
+from torchvision.models.resnet import resnet18
+from torchvision.models import vgg16
+from torchvision import transforms
+
+
+def get_fc_data_transforms(input_size, dt_key=None):
+    if dt_key is not None and dt_key != 'train':
+        return {dt_key: transforms.Compose([
+            transforms.ToTensor(),
+            transforms.Resize((input_size, input_size), antialias=True),
+            transforms.CenterCrop(input_size),
+            transforms.Normalize([0.485, 0.456, 0.406], [0.229, 0.224, 0.225])
+        ])}
+    # Apply data augmentation
+    aug_list = []
+    aug_list.append(transforms.ToTensor())
+    aug_list.append(transforms.Resize((input_size, input_size), antialias=True))
+    aug_list.append(transforms.Normalize([0.485, 0.456, 0.406], [0.229, 0.224, 0.225]))
+    aug_transform = transforms.Compose(aug_list)
+
+    # Define data transformation on train, val, test set respectively
+    data_transforms = {
+        'train': aug_transform,
+        'val': transforms.Compose([
+            transforms.ToTensor(),
+            transforms.Resize((input_size, input_size), antialias=True),
+            transforms.CenterCrop(input_size),
+            transforms.Normalize([0.485, 0.456, 0.406], [0.229, 0.224, 0.225])
+        ]),
+    }
+    return data_transforms
+
+
+def init_face_classifier(device, num_classes=2, resume_from=None):
+    input_size = 100
+    model = vgg16(num_classes=num_classes)
+    num_ftrs = model.classifier[6].in_features
+    model.classifier[6] = torch.nn.Linear(num_ftrs, num_classes)
+    if resume_from is not None:
+        print("Loading weights from %s" % resume_from)
+        model.load_state_dict(torch.load(resume_from, map_location=device))
+    return model, input_size
+
+
+
+class DataTransforms:
+    def __init__(self, img_size, mean, std):
+        self.transformations = {
+            'train': transforms.Compose([
+                transforms.Resize((img_size, img_size)),
+                transforms.ColorJitter(brightness=0.2, contrast=0.2, saturation=0.2, hue=0.05),
+                transforms.ToTensor(),
+                transforms.Normalize(mean, std)
+                # transforms.RandomErasing()
+            ]),
+            'val': transforms.Compose([
+                transforms.Resize((img_size, img_size)),
+                transforms.ToTensor(),
+                transforms.Normalize(mean, std)
+            ]),
+            'test': transforms.Compose([
+                transforms.Resize((img_size, img_size)),
+                transforms.ToTensor(),
+                transforms.Normalize(mean, std)
+            ])
+        }
+
+class Predictor_fc(torch.nn.Module):
+    def __init__(self, n, add_box):
+        super().__init__()
+        in_channel = 512 * n if add_box else 256 * n
+        self.fc1 = torch.nn.Linear(in_channel, 512)
+        self.fc2 = torch.nn.Linear(512, 512)
+        self.fc3 = torch.nn.Linear(512, 3)
+        self.bn1 = torch.nn.BatchNorm1d(512)
+        self.bn2 = torch.nn.BatchNorm1d(512)
+        self.dropout1 = torch.nn.Dropout(0.2)
+        self.dropout2 = torch.nn.Dropout(0.2)
+
+    def forward(self, x):
+        x = self.fc1(x.view(x.size(0), -1))
+        x = self.dropout1(F.relu(self.bn1(x)))
+        x = self.fc2(x)
+        x = self.dropout2(F.relu(self.bn2(x)))
+        x = self.fc3(x)
+        return x
+
+class Encoder_box(torch.nn.Module):
+    def __init__(self):
+        super().__init__()
+        self.fc1 = torch.nn.Linear(5, 256)
+        self.fc2 = torch.nn.Linear(256, 256)
+        self.bn = torch.nn.BatchNorm1d(256)
+        self.dropout = torch.nn.Dropout(0.2)
+
+    def forward(self, x):
+        x = self.fc1(x)
+        x = self.dropout(F.relu(self.bn(x)))
+        x = self.fc2(x)
+
+        return x
+
+class GazeCodingModel(torch.nn.Module):
+    def __init__(self, args, add_box=True):
+        super().__init__()
+        self.args = args
+        self.n = (args.sliding_window_size + 1) // args.window_stride
+        self.add_box = add_box
+        self.encoder_img = resnet18(num_classes=256).to(self.args.device)
+        self.encoder_box = Encoder_box().to(self.args.device)
+        self.predictor = Predictor_fc(self.n, add_box).to(self.args.device)
+
+    def forward(self, data):
+        imgs = data['imgs']  # bs x n x 3 x 100 x 100
+        boxs = data['boxs']  # bs x n x 5
+        embedding = self.encoder_img(imgs.view(-1, 3, 100, 100)).view(-1, self.n, 256)
+        if self.add_box:
+            box_embedding = self.encoder_box(boxs.view(-1, 5)).view(-1, self.n, 256)
+            embedding = torch.cat([embedding, box_embedding], -1)
+        pred = self.predictor(embedding)
         return pred
```

### Comparing `icatcher-0.0.9/src/icatcher/options.py` & `icatcher-0.1.0/src/icatcher/options.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,89 +1,118 @@
-import argparse
-from pathlib import Path
-from . import version
-
-def parse_arguments():
-    parser = argparse.ArgumentParser(prog='icatcher')
-    parser.add_argument("source", type=str, help="the source to use (path to video file, folder or webcam id)")
-    parser.add_argument("--model", type=str, help="path to model that will be used for predictions "
-                                                  "if not supplied will use model trained on the lookit dataset")
-    parser.add_argument("--use_fc_model", action="store_true", help="if supplied, will use face classifier "
-                                                                              "to decide which crop to use from every frame.")
-    parser.add_argument("--fc_model", type=str, help="path to face classifier model that will be used for deciding "
-                                                     "which crop should we select from every frame. "
-                                                     "if not supplied but use_fc_model is true, will use the model trained on the lookit dataset.")
-    parser.add_argument("--source_type", type=str, default="file", choices=["file", "webcam"],
-                        help="selects source of stream to use.")
-    parser.add_argument("--crop_percent", type=int, default=0, help="A percent to crop video frames to prevent other people from appearing")
-    parser.add_argument("--crop_mode", type=str, choices=["top", "left", "right"], nargs="+", default=["top"], help="where to crop video from, multi-choice.")
-    parser.add_argument("--track_face", action="store_true", help="if detectin is lost, will keep track of face using last known position.")
-    parser.add_argument("--show_output", action="store_true", help="show results online in a separate window")
-    parser.add_argument("--output_annotation", type=str, help="folder to output annotations to")
-    parser.add_argument("--on_off", action="store_true",
-                        help="left/right/away annotations will be swapped with on/off (only works with icatcher+)")
-    parser.add_argument("--output_format", type=str, default="raw_output", choices=["raw_output",
-                                                                                    "compressed",
-                                                                                    "PrefLookTimestamp"])  # https://osf.io/3n97m/ - PrefLookTimestamp coding standard
-    parser.add_argument("--output_video_path", help="if present, annotated video will be saved to this folder")
-    parser.add_argument("--pic_in_pic", action="store_true", help="if present, a mini picture with detection will be shown in the output video")
-    parser.add_argument("--output_file_suffix", type=str, default=".txt", help="the output file suffix")
-    parser.add_argument("--image_size", type=int, default=100, help="All images will be resized to this size")
-    parser.add_argument("--sliding_window_size", type=int, default=9, help="Number of frames in rolling window of each datapoint")
-    parser.add_argument("--window_stride", type=int, default=2, help="Stride between frames in rolling window")
-    parser.add_argument('--per_channel_mean', nargs=3, metavar=('Channel1_mean', 'Channel2_mean', 'Channel3_mean'),
-                        type=float, default=[0.485, 0.456, 0.406],
-                        help='supply custom per-channel mean of data for normalization')
-    parser.add_argument('--per_channel_std', nargs=3, metavar=('Channel1_std', 'Channel2_std', 'Channel3_std'),
-                        type=float, default=[0.229, 0.224, 0.225],
-                        help='supply custom per-channel std of data for normalization')
-    parser.add_argument("--gpu_id", type=int, default=-1, help="GPU id to use, use -1 for CPU.")
-    parser.add_argument("--log",
-                        help="If present, writes log to this path")
-    parser.add_argument("-v", "--verbosity", type=str, choices=["debug", "info", "warning"], default="info",
-                        help="Selects verbosity level")
-    parser.add_argument("--video_filter", type=str,
-                        help="provided file will be used to filter only test videos,"
-                             " will assume certain file structure using the lookit/cali-bw/senegal datasets")
-    parser.add_argument("--raw_dataset_path", type=str, help="path to raw dataset (required if --video_filter is passed")
-    parser.add_argument("--raw_dataset_type", type=str, choices=["lookit", "cali-bw", "senegal", "generic"], default="lookit",
-                        help="the type of dataset to preprocess")
-    parser.add_argument("--illegal_transitions_path", type=str, help="path to CSV with illegal transitions to 'smooth' over")
-    parser.add_argument('--version', action='version', version="%(prog)s "+version)
-    args = parser.parse_args()
-    if args.model:
-        args.model = Path(args.model)
-    # if not args.model.is_file():
-    #     raise FileNotFoundError("Model file not found")
-    if args.crop_percent not in [x for x in range(100)]:
-        raise ValueError("crop_video must be a percent between 0 - 99")
-    if "left" in args.crop_mode and "right" in args.crop_mode:
-        if args.crop_percent > 49:
-            raise ValueError("crop_video must be a percent between 0 - 49 when cropping both sides")
-    if args.video_filter:
-        args.video_filter = Path(args.video_filter)
-        assert args.video_filter.is_file() or args.video_filter.is_dir()
-    if args.raw_dataset_path:
-        args.raw_dataset_path = Path(args.raw_dataset_path)
-    if args.output_annotation:
-        args.output_annotation = Path(args.output_annotation)
-        args.output_annotation.mkdir(exist_ok=True, parents=True)
-    if args.output_video_path:
-        args.output_video_path = Path(args.output_video_path)
-        args.output_video_path.mkdir(exist_ok=True, parents=True)
-    if args.log:
-        args.log = Path(args.log)
-    if args.on_off:
-        if args.output_format != "raw_output":
-            print("On off mode can only be used with raw output format. Pass raw_output with the --output_format flag.")
-            raise AssertionError
-    if not args.per_channel_mean:
-        args.per_channel_mean = [0.485, 0.456, 0.406]
-    if not args.per_channel_std:
-        args.per_channel_std = [0.229, 0.224, 0.225]
-    if args.gpu_id == -1:
-        args.device = "cpu"
-    else:
-        import os
-        os.environ["CUDA_VISIBLE_DEVICES"] = str(args.gpu_id)
-        args.device = "cuda:{}".format(0)
-    return args
+import argparse
+from pathlib import Path
+from . import version
+
+
+def parse_arguments(my_string=None):
+    """
+    parse command line arguments
+    :param my_string: if provided, will parse this string instead of command line arguments
+    :return: parsed arguments
+    """
+    parser = argparse.ArgumentParser(prog='icatcher')
+    parser.add_argument("source", type=str, help="the source to use (path to video file, folder or webcam id)")
+    parser.add_argument("--model", type=str, help="path to model that will be used for predictions "
+                                                  "if not supplied will use model trained on the lookit dataset")
+    parser.add_argument("--use_fc_model", action="store_true", help="if supplied, will use face classifier "
+                                                                              "to decide which crop to use from every frame.")
+    parser.add_argument("--fc_model", type=str, help="path to face classifier model that will be used for deciding "
+                                                     "which crop should we select from every frame. "
+                                                     "if not supplied but use_fc_model is true, will use the model trained on the lookit dataset.")
+    parser.add_argument("--source_type", type=str, default="file", choices=["file", "webcam"],
+                        help="selects source of stream to use.")
+    parser.add_argument("--crop_percent", type=int, default=0, help="A percent to crop video frames to prevent other people from appearing")
+    parser.add_argument("--crop_mode", type=str, choices=["top", "left", "right"], nargs="+", default=["top"], help="where to crop video from, multi-choice.")
+    parser.add_argument("--track_face", action="store_true", help="if detection is lost, will keep track of face using last known position.")
+    parser.add_argument("--show_output", action="store_true", help="show results online in a separate window")
+    parser.add_argument("--output_annotation", type=str, help="folder to output annotations to")
+    parser.add_argument("--on_off", action="store_true",
+                        help="left/right/away annotations will be swapped with on/off (only works with icatcher+)")
+    parser.add_argument("--output_format", type=str, default="raw_output", choices=["raw_output",
+                                                                                    "compressed",
+                                                                                    "PrefLookTimestamp"])  # https://osf.io/3n97m/ - PrefLookTimestamp coding standard
+    parser.add_argument("--output_video_path", help="if present, annotated video will be saved to this folder")
+    parser.add_argument("--pic_in_pic", action="store_true", help="if present, a mini picture with detection will be shown in the output video")
+    parser.add_argument("--output_file_suffix", type=str, default=".txt", help="the output file suffix")
+    parser.add_argument("--image_size", type=int, default=100, help="All images will be resized to this size")
+    parser.add_argument("--sliding_window_size", type=int, default=9, help="Number of frames in rolling window of each datapoint")
+    parser.add_argument("--window_stride", type=int, default=2, help="Stride between frames in rolling window")
+    parser.add_argument('--per_channel_mean', nargs=3, metavar=('Channel1_mean', 'Channel2_mean', 'Channel3_mean'),
+                        type=float, default=[0.485, 0.456, 0.406],
+                        help='supply custom per-channel mean of data for normalization')
+    parser.add_argument('--per_channel_std', nargs=3, metavar=('Channel1_std', 'Channel2_std', 'Channel3_std'),
+                        type=float, default=[0.229, 0.224, 0.225],
+                        help='supply custom per-channel std of data for normalization')
+    parser.add_argument("--gpu_id", type=int, default=-1, help="GPU id to use, use -1 for CPU.")
+    parser.add_argument("--log",
+                        help="If present, writes log to this path")
+    parser.add_argument("-v", "--verbosity", type=str, choices=["debug", "info", "warning"], default="info",
+                        help="Selects verbosity level")
+    parser.add_argument("--video_filter", type=str,
+                        help="provided file will be used to filter only test videos,"
+                             " will assume certain file structure using the lookit/cali-bw/senegal datasets")
+    parser.add_argument("--raw_dataset_path", type=str, help="path to raw dataset (required if --video_filter is passed")
+    parser.add_argument("--raw_dataset_type", type=str, choices=["lookit", "cali-bw", "senegal", "generic"], default="lookit",
+                        help="the type of dataset to preprocess")
+    parser.add_argument("--illegal_transitions_path", type=str, help="path to CSV with illegal transitions to 'smooth' over")
+    parser.add_argument('--version', action='version', version="%(prog)s "+version)
+    # face detection options:
+    parser.add_argument("--fd_model", type=str, choices=["retinaface", "opencv_dnn"], default="retinaface",
+                        help="the face detector model used. opencv_dnn may be more suitable for cpu usage if speed is priority over accuracy")
+    parser.add_argument("--fd_confidence_threshold", type=float, help="the score confidence threshold that needs to be met for a face to be detected")
+    parser.add_argument("--num_cpus_saved", type=int, default=0,
+                        help="(retinaface only) amount of cpus to not use in parallel processing of face detection")
+    parser.add_argument("--fd_batch_size", type=int, default=16,
+                        help="(retinaface only) amount of frames fed into face detector at one time for batch inference")
+    parser.add_argument("--fd_skip_frames", type=int, default=0,
+                        help="(cpu only) amount of frames to skip between each face detection. previous bbox will be used")
+    parser.add_argument("--dont_buffer", action="store_true", default=False,
+                        help="(cpu, retinaface only) frames will not be buffered, decreasing memory usage, but increasing processing time. Allows live stream of results.")
+    if my_string is not None:
+        args = parser.parse_args(my_string.split())
+    else:
+        args = parser.parse_args()
+    if args.model:
+        args.model = Path(args.model)
+    if args.fd_confidence_threshold is None:  # set defaults outside argparse to avoid complication
+        if args.fd_model == "retinaface":
+            args.fd_confidence_threshold = 0.9
+        elif args.fd_model == "opencv_dnn":
+            args.fd_confidence_threshold = 0.7
+    # if not args.model.is_file():
+    #     raise FileNotFoundError("Model file not found")
+    if args.crop_percent not in [x for x in range(100)]:
+        raise ValueError("crop_video must be a percent between 0 - 99")
+    if "left" in args.crop_mode and "right" in args.crop_mode:
+        if args.crop_percent > 49:
+            raise ValueError("crop_video must be a percent between 0 - 49 when cropping both sides")
+    if args.video_filter:
+        args.video_filter = Path(args.video_filter)
+        if not args.video_filter.is_file() and not args.video_filter.is_dir():
+            raise FileNotFoundError("Video filter is not a file or a folder")
+    if args.raw_dataset_path:
+        args.raw_dataset_path = Path(args.raw_dataset_path)
+    if args.output_annotation:
+        args.output_annotation = Path(args.output_annotation)
+        args.output_annotation.mkdir(exist_ok=True, parents=True)
+    if args.output_video_path:
+        args.output_video_path = Path(args.output_video_path)
+        args.output_video_path.mkdir(exist_ok=True, parents=True)
+    if args.log:
+        args.log = Path(args.log)
+    if args.on_off:
+        if args.output_format != "raw_output":
+            raise ValueError("On off mode can only be used with raw output format. Pass raw_output with the --output_format flag.")
+    if not args.per_channel_mean:
+        args.per_channel_mean = [0.485, 0.456, 0.406]
+    if not args.per_channel_std:
+        args.per_channel_std = [0.229, 0.224, 0.225]
+    if args.gpu_id == -1:
+        args.device = "cpu"
+    else:
+        import os
+        os.environ["CUDA_VISIBLE_DEVICES"] = str(args.gpu_id)
+        args.device = "cuda:{}".format(0)
+        import torch
+        if not torch.cuda.is_available():
+            raise ValueError("GPU is not available. Was torch compiled with CUDA?")
+    return args
```

### Comparing `icatcher-0.0.9/src/icatcher.egg-info/PKG-INFO` & `icatcher-0.1.0/src/icatcher.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,863 +1,813 @@
-Metadata-Version: 2.1
-Name: icatcher
-Version: 0.0.9
-Summary: iCatcher+: Robust and automated annotation of infant gaze from videos collected in laboratory, field, and online studies.
-Author-email: Yotam Erel <erelyotam@gmail.com>
-License:                     GNU GENERAL PUBLIC LICENSE
-                               Version 3, 29 June 2007
-        
-         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
-         Everyone is permitted to copy and distribute verbatim copies
-         of this license document, but changing it is not allowed.
-        
-                                    Preamble
-        
-          The GNU General Public License is a free, copyleft license for
-        software and other kinds of works.
-        
-          The licenses for most software and other practical works are designed
-        to take away your freedom to share and change the works.  By contrast,
-        the GNU General Public License is intended to guarantee your freedom to
-        share and change all versions of a program--to make sure it remains free
-        software for all its users.  We, the Free Software Foundation, use the
-        GNU General Public License for most of our software; it applies also to
-        any other work released this way by its authors.  You can apply it to
-        your programs, too.
-        
-          When we speak of free software, we are referring to freedom, not
-        price.  Our General Public Licenses are designed to make sure that you
-        have the freedom to distribute copies of free software (and charge for
-        them if you wish), that you receive source code or can get it if you
-        want it, that you can change the software or use pieces of it in new
-        free programs, and that you know you can do these things.
-        
-          To protect your rights, we need to prevent others from denying you
-        these rights or asking you to surrender the rights.  Therefore, you have
-        certain responsibilities if you distribute copies of the software, or if
-        you modify it: responsibilities to respect the freedom of others.
-        
-          For example, if you distribute copies of such a program, whether
-        gratis or for a fee, you must pass on to the recipients the same
-        freedoms that you received.  You must make sure that they, too, receive
-        or can get the source code.  And you must show them these terms so they
-        know their rights.
-        
-          Developers that use the GNU GPL protect your rights with two steps:
-        (1) assert copyright on the software, and (2) offer you this License
-        giving you legal permission to copy, distribute and/or modify it.
-        
-          For the developers' and authors' protection, the GPL clearly explains
-        that there is no warranty for this free software.  For both users' and
-        authors' sake, the GPL requires that modified versions be marked as
-        changed, so that their problems will not be attributed erroneously to
-        authors of previous versions.
-        
-          Some devices are designed to deny users access to install or run
-        modified versions of the software inside them, although the manufacturer
-        can do so.  This is fundamentally incompatible with the aim of
-        protecting users' freedom to change the software.  The systematic
-        pattern of such abuse occurs in the area of products for individuals to
-        use, which is precisely where it is most unacceptable.  Therefore, we
-        have designed this version of the GPL to prohibit the practice for those
-        products.  If such problems arise substantially in other domains, we
-        stand ready to extend this provision to those domains in future versions
-        of the GPL, as needed to protect the freedom of users.
-        
-          Finally, every program is threatened constantly by software patents.
-        States should not allow patents to restrict development and use of
-        software on general-purpose computers, but in those that do, we wish to
-        avoid the special danger that patents applied to a free program could
-        make it effectively proprietary.  To prevent this, the GPL assures that
-        patents cannot be used to render the program non-free.
-        
-          The precise terms and conditions for copying, distribution and
-        modification follow.
-        
-                               TERMS AND CONDITIONS
-        
-          0. Definitions.
-        
-          "This License" refers to version 3 of the GNU General Public License.
-        
-          "Copyright" also means copyright-like laws that apply to other kinds of
-        works, such as semiconductor masks.
-        
-          "The Program" refers to any copyrightable work licensed under this
-        License.  Each licensee is addressed as "you".  "Licensees" and
-        "recipients" may be individuals or organizations.
-        
-          To "modify" a work means to copy from or adapt all or part of the work
-        in a fashion requiring copyright permission, other than the making of an
-        exact copy.  The resulting work is called a "modified version" of the
-        earlier work or a work "based on" the earlier work.
-        
-          A "covered work" means either the unmodified Program or a work based
-        on the Program.
-        
-          To "propagate" a work means to do anything with it that, without
-        permission, would make you directly or secondarily liable for
-        infringement under applicable copyright law, except executing it on a
-        computer or modifying a private copy.  Propagation includes copying,
-        distribution (with or without modification), making available to the
-        public, and in some countries other activities as well.
-        
-          To "convey" a work means any kind of propagation that enables other
-        parties to make or receive copies.  Mere interaction with a user through
-        a computer network, with no transfer of a copy, is not conveying.
-        
-          An interactive user interface displays "Appropriate Legal Notices"
-        to the extent that it includes a convenient and prominently visible
-        feature that (1) displays an appropriate copyright notice, and (2)
-        tells the user that there is no warranty for the work (except to the
-        extent that warranties are provided), that licensees may convey the
-        work under this License, and how to view a copy of this License.  If
-        the interface presents a list of user commands or options, such as a
-        menu, a prominent item in the list meets this criterion.
-        
-          1. Source Code.
-        
-          The "source code" for a work means the preferred form of the work
-        for making modifications to it.  "Object code" means any non-source
-        form of a work.
-        
-          A "Standard Interface" means an interface that either is an official
-        standard defined by a recognized standards body, or, in the case of
-        interfaces specified for a particular programming language, one that
-        is widely used among developers working in that language.
-        
-          The "System Libraries" of an executable work include anything, other
-        than the work as a whole, that (a) is included in the normal form of
-        packaging a Major Component, but which is not part of that Major
-        Component, and (b) serves only to enable use of the work with that
-        Major Component, or to implement a Standard Interface for which an
-        implementation is available to the public in source code form.  A
-        "Major Component", in this context, means a major essential component
-        (kernel, window system, and so on) of the specific operating system
-        (if any) on which the executable work runs, or a compiler used to
-        produce the work, or an object code interpreter used to run it.
-        
-          The "Corresponding Source" for a work in object code form means all
-        the source code needed to generate, install, and (for an executable
-        work) run the object code and to modify the work, including scripts to
-        control those activities.  However, it does not include the work's
-        System Libraries, or general-purpose tools or generally available free
-        programs which are used unmodified in performing those activities but
-        which are not part of the work.  For example, Corresponding Source
-        includes interface definition files associated with source files for
-        the work, and the source code for shared libraries and dynamically
-        linked subprograms that the work is specifically designed to require,
-        such as by intimate data communication or control flow between those
-        subprograms and other parts of the work.
-        
-          The Corresponding Source need not include anything that users
-        can regenerate automatically from other parts of the Corresponding
-        Source.
-        
-          The Corresponding Source for a work in source code form is that
-        same work.
-        
-          2. Basic Permissions.
-        
-          All rights granted under this License are granted for the term of
-        copyright on the Program, and are irrevocable provided the stated
-        conditions are met.  This License explicitly affirms your unlimited
-        permission to run the unmodified Program.  The output from running a
-        covered work is covered by this License only if the output, given its
-        content, constitutes a covered work.  This License acknowledges your
-        rights of fair use or other equivalent, as provided by copyright law.
-        
-          You may make, run and propagate covered works that you do not
-        convey, without conditions so long as your license otherwise remains
-        in force.  You may convey covered works to others for the sole purpose
-        of having them make modifications exclusively for you, or provide you
-        with facilities for running those works, provided that you comply with
-        the terms of this License in conveying all material for which you do
-        not control copyright.  Those thus making or running the covered works
-        for you must do so exclusively on your behalf, under your direction
-        and control, on terms that prohibit them from making any copies of
-        your copyrighted material outside their relationship with you.
-        
-          Conveying under any other circumstances is permitted solely under
-        the conditions stated below.  Sublicensing is not allowed; section 10
-        makes it unnecessary.
-        
-          3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-        
-          No covered work shall be deemed part of an effective technological
-        measure under any applicable law fulfilling obligations under article
-        11 of the WIPO copyright treaty adopted on 20 December 1996, or
-        similar laws prohibiting or restricting circumvention of such
-        measures.
-        
-          When you convey a covered work, you waive any legal power to forbid
-        circumvention of technological measures to the extent such circumvention
-        is effected by exercising rights under this License with respect to
-        the covered work, and you disclaim any intention to limit operation or
-        modification of the work as a means of enforcing, against the work's
-        users, your or third parties' legal rights to forbid circumvention of
-        technological measures.
-        
-          4. Conveying Verbatim Copies.
-        
-          You may convey verbatim copies of the Program's source code as you
-        receive it, in any medium, provided that you conspicuously and
-        appropriately publish on each copy an appropriate copyright notice;
-        keep intact all notices stating that this License and any
-        non-permissive terms added in accord with section 7 apply to the code;
-        keep intact all notices of the absence of any warranty; and give all
-        recipients a copy of this License along with the Program.
-        
-          You may charge any price or no price for each copy that you convey,
-        and you may offer support or warranty protection for a fee.
-        
-          5. Conveying Modified Source Versions.
-        
-          You may convey a work based on the Program, or the modifications to
-        produce it from the Program, in the form of source code under the
-        terms of section 4, provided that you also meet all of these conditions:
-        
-            a) The work must carry prominent notices stating that you modified
-            it, and giving a relevant date.
-        
-            b) The work must carry prominent notices stating that it is
-            released under this License and any conditions added under section
-            7.  This requirement modifies the requirement in section 4 to
-            "keep intact all notices".
-        
-            c) You must license the entire work, as a whole, under this
-            License to anyone who comes into possession of a copy.  This
-            License will therefore apply, along with any applicable section 7
-            additional terms, to the whole of the work, and all its parts,
-            regardless of how they are packaged.  This License gives no
-            permission to license the work in any other way, but it does not
-            invalidate such permission if you have separately received it.
-        
-            d) If the work has interactive user interfaces, each must display
-            Appropriate Legal Notices; however, if the Program has interactive
-            interfaces that do not display Appropriate Legal Notices, your
-            work need not make them do so.
-        
-          A compilation of a covered work with other separate and independent
-        works, which are not by their nature extensions of the covered work,
-        and which are not combined with it such as to form a larger program,
-        in or on a volume of a storage or distribution medium, is called an
-        "aggregate" if the compilation and its resulting copyright are not
-        used to limit the access or legal rights of the compilation's users
-        beyond what the individual works permit.  Inclusion of a covered work
-        in an aggregate does not cause this License to apply to the other
-        parts of the aggregate.
-        
-          6. Conveying Non-Source Forms.
-        
-          You may convey a covered work in object code form under the terms
-        of sections 4 and 5, provided that you also convey the
-        machine-readable Corresponding Source under the terms of this License,
-        in one of these ways:
-        
-            a) Convey the object code in, or embodied in, a physical product
-            (including a physical distribution medium), accompanied by the
-            Corresponding Source fixed on a durable physical medium
-            customarily used for software interchange.
-        
-            b) Convey the object code in, or embodied in, a physical product
-            (including a physical distribution medium), accompanied by a
-            written offer, valid for at least three years and valid for as
-            long as you offer spare parts or customer support for that product
-            model, to give anyone who possesses the object code either (1) a
-            copy of the Corresponding Source for all the software in the
-            product that is covered by this License, on a durable physical
-            medium customarily used for software interchange, for a price no
-            more than your reasonable cost of physically performing this
-            conveying of source, or (2) access to copy the
-            Corresponding Source from a network server at no charge.
-        
-            c) Convey individual copies of the object code with a copy of the
-            written offer to provide the Corresponding Source.  This
-            alternative is allowed only occasionally and noncommercially, and
-            only if you received the object code with such an offer, in accord
-            with subsection 6b.
-        
-            d) Convey the object code by offering access from a designated
-            place (gratis or for a charge), and offer equivalent access to the
-            Corresponding Source in the same way through the same place at no
-            further charge.  You need not require recipients to copy the
-            Corresponding Source along with the object code.  If the place to
-            copy the object code is a network server, the Corresponding Source
-            may be on a different server (operated by you or a third party)
-            that supports equivalent copying facilities, provided you maintain
-            clear directions next to the object code saying where to find the
-            Corresponding Source.  Regardless of what server hosts the
-            Corresponding Source, you remain obligated to ensure that it is
-            available for as long as needed to satisfy these requirements.
-        
-            e) Convey the object code using peer-to-peer transmission, provided
-            you inform other peers where the object code and Corresponding
-            Source of the work are being offered to the general public at no
-            charge under subsection 6d.
-        
-          A separable portion of the object code, whose source code is excluded
-        from the Corresponding Source as a System Library, need not be
-        included in conveying the object code work.
-        
-          A "User Product" is either (1) a "consumer product", which means any
-        tangible personal property which is normally used for personal, family,
-        or household purposes, or (2) anything designed or sold for incorporation
-        into a dwelling.  In determining whether a product is a consumer product,
-        doubtful cases shall be resolved in favor of coverage.  For a particular
-        product received by a particular user, "normally used" refers to a
-        typical or common use of that class of product, regardless of the status
-        of the particular user or of the way in which the particular user
-        actually uses, or expects or is expected to use, the product.  A product
-        is a consumer product regardless of whether the product has substantial
-        commercial, industrial or non-consumer uses, unless such uses represent
-        the only significant mode of use of the product.
-        
-          "Installation Information" for a User Product means any methods,
-        procedures, authorization keys, or other information required to install
-        and execute modified versions of a covered work in that User Product from
-        a modified version of its Corresponding Source.  The information must
-        suffice to ensure that the continued functioning of the modified object
-        code is in no case prevented or interfered with solely because
-        modification has been made.
-        
-          If you convey an object code work under this section in, or with, or
-        specifically for use in, a User Product, and the conveying occurs as
-        part of a transaction in which the right of possession and use of the
-        User Product is transferred to the recipient in perpetuity or for a
-        fixed term (regardless of how the transaction is characterized), the
-        Corresponding Source conveyed under this section must be accompanied
-        by the Installation Information.  But this requirement does not apply
-        if neither you nor any third party retains the ability to install
-        modified object code on the User Product (for example, the work has
-        been installed in ROM).
-        
-          The requirement to provide Installation Information does not include a
-        requirement to continue to provide support service, warranty, or updates
-        for a work that has been modified or installed by the recipient, or for
-        the User Product in which it has been modified or installed.  Access to a
-        network may be denied when the modification itself materially and
-        adversely affects the operation of the network or violates the rules and
-        protocols for communication across the network.
-        
-          Corresponding Source conveyed, and Installation Information provided,
-        in accord with this section must be in a format that is publicly
-        documented (and with an implementation available to the public in
-        source code form), and must require no special password or key for
-        unpacking, reading or copying.
-        
-          7. Additional Terms.
-        
-          "Additional permissions" are terms that supplement the terms of this
-        License by making exceptions from one or more of its conditions.
-        Additional permissions that are applicable to the entire Program shall
-        be treated as though they were included in this License, to the extent
-        that they are valid under applicable law.  If additional permissions
-        apply only to part of the Program, that part may be used separately
-        under those permissions, but the entire Program remains governed by
-        this License without regard to the additional permissions.
-        
-          When you convey a copy of a covered work, you may at your option
-        remove any additional permissions from that copy, or from any part of
-        it.  (Additional permissions may be written to require their own
-        removal in certain cases when you modify the work.)  You may place
-        additional permissions on material, added by you to a covered work,
-        for which you have or can give appropriate copyright permission.
-        
-          Notwithstanding any other provision of this License, for material you
-        add to a covered work, you may (if authorized by the copyright holders of
-        that material) supplement the terms of this License with terms:
-        
-            a) Disclaiming warranty or limiting liability differently from the
-            terms of sections 15 and 16 of this License; or
-        
-            b) Requiring preservation of specified reasonable legal notices or
-            author attributions in that material or in the Appropriate Legal
-            Notices displayed by works containing it; or
-        
-            c) Prohibiting misrepresentation of the origin of that material, or
-            requiring that modified versions of such material be marked in
-            reasonable ways as different from the original version; or
-        
-            d) Limiting the use for publicity purposes of names of licensors or
-            authors of the material; or
-        
-            e) Declining to grant rights under trademark law for use of some
-            trade names, trademarks, or service marks; or
-        
-            f) Requiring indemnification of licensors and authors of that
-            material by anyone who conveys the material (or modified versions of
-            it) with contractual assumptions of liability to the recipient, for
-            any liability that these contractual assumptions directly impose on
-            those licensors and authors.
-        
-          All other non-permissive additional terms are considered "further
-        restrictions" within the meaning of section 10.  If the Program as you
-        received it, or any part of it, contains a notice stating that it is
-        governed by this License along with a term that is a further
-        restriction, you may remove that term.  If a license document contains
-        a further restriction but permits relicensing or conveying under this
-        License, you may add to a covered work material governed by the terms
-        of that license document, provided that the further restriction does
-        not survive such relicensing or conveying.
-        
-          If you add terms to a covered work in accord with this section, you
-        must place, in the relevant source files, a statement of the
-        additional terms that apply to those files, or a notice indicating
-        where to find the applicable terms.
-        
-          Additional terms, permissive or non-permissive, may be stated in the
-        form of a separately written license, or stated as exceptions;
-        the above requirements apply either way.
-        
-          8. Termination.
-        
-          You may not propagate or modify a covered work except as expressly
-        provided under this License.  Any attempt otherwise to propagate or
-        modify it is void, and will automatically terminate your rights under
-        this License (including any patent licenses granted under the third
-        paragraph of section 11).
-        
-          However, if you cease all violation of this License, then your
-        license from a particular copyright holder is reinstated (a)
-        provisionally, unless and until the copyright holder explicitly and
-        finally terminates your license, and (b) permanently, if the copyright
-        holder fails to notify you of the violation by some reasonable means
-        prior to 60 days after the cessation.
-        
-          Moreover, your license from a particular copyright holder is
-        reinstated permanently if the copyright holder notifies you of the
-        violation by some reasonable means, this is the first time you have
-        received notice of violation of this License (for any work) from that
-        copyright holder, and you cure the violation prior to 30 days after
-        your receipt of the notice.
-        
-          Termination of your rights under this section does not terminate the
-        licenses of parties who have received copies or rights from you under
-        this License.  If your rights have been terminated and not permanently
-        reinstated, you do not qualify to receive new licenses for the same
-        material under section 10.
-        
-          9. Acceptance Not Required for Having Copies.
-        
-          You are not required to accept this License in order to receive or
-        run a copy of the Program.  Ancillary propagation of a covered work
-        occurring solely as a consequence of using peer-to-peer transmission
-        to receive a copy likewise does not require acceptance.  However,
-        nothing other than this License grants you permission to propagate or
-        modify any covered work.  These actions infringe copyright if you do
-        not accept this License.  Therefore, by modifying or propagating a
-        covered work, you indicate your acceptance of this License to do so.
-        
-          10. Automatic Licensing of Downstream Recipients.
-        
-          Each time you convey a covered work, the recipient automatically
-        receives a license from the original licensors, to run, modify and
-        propagate that work, subject to this License.  You are not responsible
-        for enforcing compliance by third parties with this License.
-        
-          An "entity transaction" is a transaction transferring control of an
-        organization, or substantially all assets of one, or subdividing an
-        organization, or merging organizations.  If propagation of a covered
-        work results from an entity transaction, each party to that
-        transaction who receives a copy of the work also receives whatever
-        licenses to the work the party's predecessor in interest had or could
-        give under the previous paragraph, plus a right to possession of the
-        Corresponding Source of the work from the predecessor in interest, if
-        the predecessor has it or can get it with reasonable efforts.
-        
-          You may not impose any further restrictions on the exercise of the
-        rights granted or affirmed under this License.  For example, you may
-        not impose a license fee, royalty, or other charge for exercise of
-        rights granted under this License, and you may not initiate litigation
-        (including a cross-claim or counterclaim in a lawsuit) alleging that
-        any patent claim is infringed by making, using, selling, offering for
-        sale, or importing the Program or any portion of it.
-        
-          11. Patents.
-        
-          A "contributor" is a copyright holder who authorizes use under this
-        License of the Program or a work on which the Program is based.  The
-        work thus licensed is called the contributor's "contributor version".
-        
-          A contributor's "essential patent claims" are all patent claims
-        owned or controlled by the contributor, whether already acquired or
-        hereafter acquired, that would be infringed by some manner, permitted
-        by this License, of making, using, or selling its contributor version,
-        but do not include claims that would be infringed only as a
-        consequence of further modification of the contributor version.  For
-        purposes of this definition, "control" includes the right to grant
-        patent sublicenses in a manner consistent with the requirements of
-        this License.
-        
-          Each contributor grants you a non-exclusive, worldwide, royalty-free
-        patent license under the contributor's essential patent claims, to
-        make, use, sell, offer for sale, import and otherwise run, modify and
-        propagate the contents of its contributor version.
-        
-          In the following three paragraphs, a "patent license" is any express
-        agreement or commitment, however denominated, not to enforce a patent
-        (such as an express permission to practice a patent or covenant not to
-        sue for patent infringement).  To "grant" such a patent license to a
-        party means to make such an agreement or commitment not to enforce a
-        patent against the party.
-        
-          If you convey a covered work, knowingly relying on a patent license,
-        and the Corresponding Source of the work is not available for anyone
-        to copy, free of charge and under the terms of this License, through a
-        publicly available network server or other readily accessible means,
-        then you must either (1) cause the Corresponding Source to be so
-        available, or (2) arrange to deprive yourself of the benefit of the
-        patent license for this particular work, or (3) arrange, in a manner
-        consistent with the requirements of this License, to extend the patent
-        license to downstream recipients.  "Knowingly relying" means you have
-        actual knowledge that, but for the patent license, your conveying the
-        covered work in a country, or your recipient's use of the covered work
-        in a country, would infringe one or more identifiable patents in that
-        country that you have reason to believe are valid.
-        
-          If, pursuant to or in connection with a single transaction or
-        arrangement, you convey, or propagate by procuring conveyance of, a
-        covered work, and grant a patent license to some of the parties
-        receiving the covered work authorizing them to use, propagate, modify
-        or convey a specific copy of the covered work, then the patent license
-        you grant is automatically extended to all recipients of the covered
-        work and works based on it.
-        
-          A patent license is "discriminatory" if it does not include within
-        the scope of its coverage, prohibits the exercise of, or is
-        conditioned on the non-exercise of one or more of the rights that are
-        specifically granted under this License.  You may not convey a covered
-        work if you are a party to an arrangement with a third party that is
-        in the business of distributing software, under which you make payment
-        to the third party based on the extent of your activity of conveying
-        the work, and under which the third party grants, to any of the
-        parties who would receive the covered work from you, a discriminatory
-        patent license (a) in connection with copies of the covered work
-        conveyed by you (or copies made from those copies), or (b) primarily
-        for and in connection with specific products or compilations that
-        contain the covered work, unless you entered into that arrangement,
-        or that patent license was granted, prior to 28 March 2007.
-        
-          Nothing in this License shall be construed as excluding or limiting
-        any implied license or other defenses to infringement that may
-        otherwise be available to you under applicable patent law.
-        
-          12. No Surrender of Others' Freedom.
-        
-          If conditions are imposed on you (whether by court order, agreement or
-        otherwise) that contradict the conditions of this License, they do not
-        excuse you from the conditions of this License.  If you cannot convey a
-        covered work so as to satisfy simultaneously your obligations under this
-        License and any other pertinent obligations, then as a consequence you may
-        not convey it at all.  For example, if you agree to terms that obligate you
-        to collect a royalty for further conveying from those to whom you convey
-        the Program, the only way you could satisfy both those terms and this
-        License would be to refrain entirely from conveying the Program.
-        
-          13. Use with the GNU Affero General Public License.
-        
-          Notwithstanding any other provision of this License, you have
-        permission to link or combine any covered work with a work licensed
-        under version 3 of the GNU Affero General Public License into a single
-        combined work, and to convey the resulting work.  The terms of this
-        License will continue to apply to the part which is the covered work,
-        but the special requirements of the GNU Affero General Public License,
-        section 13, concerning interaction through a network will apply to the
-        combination as such.
-        
-          14. Revised Versions of this License.
-        
-          The Free Software Foundation may publish revised and/or new versions of
-        the GNU General Public License from time to time.  Such new versions will
-        be similar in spirit to the present version, but may differ in detail to
-        address new problems or concerns.
-        
-          Each version is given a distinguishing version number.  If the
-        Program specifies that a certain numbered version of the GNU General
-        Public License "or any later version" applies to it, you have the
-        option of following the terms and conditions either of that numbered
-        version or of any later version published by the Free Software
-        Foundation.  If the Program does not specify a version number of the
-        GNU General Public License, you may choose any version ever published
-        by the Free Software Foundation.
-        
-          If the Program specifies that a proxy can decide which future
-        versions of the GNU General Public License can be used, that proxy's
-        public statement of acceptance of a version permanently authorizes you
-        to choose that version for the Program.
-        
-          Later license versions may give you additional or different
-        permissions.  However, no additional obligations are imposed on any
-        author or copyright holder as a result of your choosing to follow a
-        later version.
-        
-          15. Disclaimer of Warranty.
-        
-          THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-        APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-        HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-        OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-        THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-        PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-        IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-        ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-        
-          16. Limitation of Liability.
-        
-          IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-        WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-        THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-        GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-        USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-        DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-        PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-        EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-        SUCH DAMAGES.
-        
-          17. Interpretation of Sections 15 and 16.
-        
-          If the disclaimer of warranty and limitation of liability provided
-        above cannot be given local legal effect according to their terms,
-        reviewing courts shall apply local law that most closely approximates
-        an absolute waiver of all civil liability in connection with the
-        Program, unless a warranty or assumption of liability accompanies a
-        copy of the Program in return for a fee.
-        
-                             END OF TERMS AND CONDITIONS
-        
-                    How to Apply These Terms to Your New Programs
-        
-          If you develop a new program, and you want it to be of the greatest
-        possible use to the public, the best way to achieve this is to make it
-        free software which everyone can redistribute and change under these terms.
-        
-          To do so, attach the following notices to the program.  It is safest
-        to attach them to the start of each source file to most effectively
-        state the exclusion of warranty; and each file should have at least
-        the "copyright" line and a pointer to where the full notice is found.
-        
-            <one line to give the program's name and a brief idea of what it does.>
-            Copyright (C) <year>  <name of author>
-        
-            This program is free software: you can redistribute it and/or modify
-            it under the terms of the GNU General Public License as published by
-            the Free Software Foundation, either version 3 of the License, or
-            (at your option) any later version.
-        
-            This program is distributed in the hope that it will be useful,
-            but WITHOUT ANY WARRANTY; without even the implied warranty of
-            MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-            GNU General Public License for more details.
-        
-            You should have received a copy of the GNU General Public License
-            along with this program.  If not, see <https://www.gnu.org/licenses/>.
-        
-        Also add information on how to contact you by electronic and paper mail.
-        
-          If the program does terminal interaction, make it output a short
-        notice like this when it starts in an interactive mode:
-        
-            <program>  Copyright (C) <year>  <name of author>
-            This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-            This is free software, and you are welcome to redistribute it
-            under certain conditions; type `show c' for details.
-        
-        The hypothetical commands `show w' and `show c' should show the appropriate
-        parts of the General Public License.  Of course, your program's commands
-        might be different; for a GUI interface, you would use an "about box".
-        
-          You should also get your employer (if you work as a programmer) or school,
-        if any, to sign a "copyright disclaimer" for the program, if necessary.
-        For more information on this, and how to apply and follow the GNU GPL, see
-        <https://www.gnu.org/licenses/>.
-        
-          The GNU General Public License does not permit incorporating your program
-        into proprietary programs.  If your program is a subroutine library, you
-        may consider it more useful to permit linking proprietary applications with
-        the library.  If this is what you want to do, use the GNU Lesser General
-        Public License instead of this License.  But first, please read
-        <https://www.gnu.org/licenses/why-not-lgpl.html>.
-        
-Project-URL: Homepage, https://github.com/yoterel/icatcher_plus
-Keywords: eyetracker,eyetracking
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: build
-Provides-Extra: dev
-License-File: LICENSE
-
-[![DOI](https://zenodo.org/badge/486841882.svg)](https://zenodo.org/badge/latestdoi/486841882)
-
-# iCatcher+
-
-# Introduction
-This repository contains all the code for [iCatcher+](https://psyarxiv.com/up97k/), a tool for performing automatic annotation of discrete infant gaze directions from videos collected in the lab, field or online (remotely). It also contains code for reproducing the original manuscripts results.
-
-Click below for a video including examples of representative good and poor performance, taken from videos of infants participating in online research (all families featured consented to sharing their video data publicly):
-
-[![iCatcher representative good and poor performance](https://img.youtube.com/vi/iK_T2P2ZDnU/0.jpg)](https://www.youtube.com/watch?v=iK_T2P2ZDnU)
-
-# Installation
-## Quick installation (Windows, Linux, Mac)
-This option will let you use iCatcher+ with minimum effort, but only for predictions (inference).
-We strongly recommend using a virtual environment such as [Miniconda](https://conda.io) or [virtualenv](https://pypi.org/project/virtualenv/) before running the command below.
-
-`pip install icatcher`
-
-You will also need [ffmpeg](https://www.ffmpeg.org/) installed in your system and available. When using for the first time, neural network model files will automatically be downloaded to a local cache folder. To control where they are downloaded to set the "ICATCHER_DATA_DIR" environment variable.
-
-## Installation for reproduction of original research results
-This options allows you to reproduce the paper results, train icatcher on your own dataset, compare and measure performance and visualize results as well.
-
-### Step 1: Clone this repository to get a copy of the code to run locally
-
-`git clone https://github.com/yoterel/icatcher_plus.git`
-
-### Step 2: Create a conda virtual environment
-
-We recommend installing [Miniconda](https://docs.conda.io/en/latest/miniconda.html) for this, then create an environment using the environment.yml file in this repository:
-
-**Note**: conda must be in the PATH envrionment variable for the shell to find it.
-
-Navigate to the icatcher_plus reproduce folder using the Anaconda Prompt:
-
-`cd /path/to/icathcer_plus/reproduce`
-
-Then:
-
-`conda env create -n env -f environment.yml`
-
-Or (if you want to install the environment in a specific location):
-
-`conda env create --prefix /path/to/virtual/environment -f "/path/to/environment.yml"`
-
-**Note for Mac users**: you might need to edit the [environment.yml](https://github.com/yoterel/icatcher_plus/blob/master/environment.yml) file depending on your OS version. see [here](https://github.com/yoterel/icatcher_plus/issues/6#issuecomment-1244125700) for how.
-
-Activate the environment
-
-`conda activate env`
-
-### Step 3: Download the neural network model & weight files
-
-iCatcher+ relies on some neural-network model files to work (or reproduce experiments).
-
-Please download all files from [here](https://osf.io/ycju8/download) and place them in the reproduce/models directory.
-
-
-# Running iCatcher+
-If you installed iCatcher+ from source, the inference file is "test.py". It will require an additional mandatory argument of which model file to use for predicitons.
-Otherwise, using the quick installation, you can run iCatcher+ with the command:
-
-`icatcher --help`
-
-which will list all available options. Description below will help you get more familiar with some common command line arguments.
-
-To run iCatcher+ with a video file (if a folder is provided, all videos will be used for prediction):
-
-`icatcher /path/to/my/video.mp4`
-
-A common option is to add:
-
-`icatcher /path/to/my/video.mp4 --use_fc_model`
-
-Which enables a child face detector for more robust results (however, sometimes this can result in too much loss of data).
-
-You can save a labeled video by adding:
-
-`--output_video_path /path/to/output_folder`
-
-If you want to output annotations to a file, use:
-
-`--output_annotation /path/to/output_annotation_folder`
-
-To show the predictions online in a seperate window, add the option:
-
-`--show_output`
-
-You can also add parameters to crop the video a given percent before passing to iCatcher: 
-
-`--crop_mode m` where `m` is any of [top, left, right], specifying which side of the video to crop from (if not provided, default is none; if crop_percent is provided but not crop_mode, default is top)
-
-`--crop_percent x` where `x` is an integer (default = 0) specifying what percent of the video size to crop from the specified side. E.g., if `--crop_mode top` is provided with `--crop_percent 10`, 10% of the video height will be cropped from the top. If `--crop_mode left` is provided with `--crop_percent 25`, 25% of the video width will be cropped from the left side, etc. 
-
-# Output format
-
-Currently we supports 2 output formats, though further formats can be added upon request.
-
-- raw_output: a file where each row will contain the frame number, the class prediction and the confidence of that prediction seperated by a comma
-- compressed: a npz file containing two numpy arrays, one encoding the predicted class (n x 1 int32) and another the confidence (n x 1 float32) where n is the number of frames. This file can be loaded into memory using the numpy.load function. For the map between class number and name see test.py ("predict_from_video" function).
-
-# Datasets access & reproduction of results
-
-The public videos from the Lookit dataset, along with human annotations and group-level demographics for all datasets, are available at https://osf.io/ujteb/. Videos from the Lookit dataset with permission granted for scientific use are available at https://osf.io/5u9df/. Requests for access can be directed to Junyi Chu (junyichu@mit.edu).
-
-Requests for access to the remainder of the datasets (Cali-BW, Senegal) can be directed to Dr. Katherine Adams Shannon (katashannon@gmail.com). Note that access to raw video files from the California-BW and Senegal datasets *is not available* due to restricted participant privacy agreements. To protect participant privacy, the participant identifiers for the video and demographic data are not linked to each other. However, this information is available upon reasonable request.
-
-We made substantial effort to allow reproduction of results form the paper. True reproduction requires full access to the datasets (including the videos).
-Instead, to reproduce most of the statistics we present in the paper for the Lookit dataset, run visualize.py using the following commands:
-
-First navigate to the reproduce folder:
-
-`cd /path/to/icatcher_plus/reproduce`
-
-Then run:
-
-`python visualize.py output resource/lookit_annotations/coding_human1 resource/lookit_annotations/coding_icatcherplus just_annotations --human2_codings_folder resource/lookit_annotations/coding_human2`
-
-Results will appear in a folder called "output".
-
-## Best Results (test sets)
-To view visualizations of all results, see [plots](https://github.com/yoterel/icatcher_plus/tree/master/reproduce/plots).
-Per-session plots (i.e. per-video) are sorted from 0 to n, where 0 has the lowest agreement (between iCatcher+ and Coder 1) and n the highest.
-### A Note About Data-Leaks
-The test sets were kept "untouched" until the very last stages of submission (i.e. they were not *directly* nor *indirectly* used optimize the network models). Conforming to this methodolgy is encouraged to avoid data leaks, so if you happen to submit improvements made to iCatcher+ in terms of performance, **do not** use the test sets for improving your method. Please consider creating a validation set out of the original training set for that.
-
-<table>
-        <tr>
-                <td align="center"> <img src="https://github.com/yoterel/icatcher_plus/blob/master/resource/agreement.png"  alt="0" width = 400px height = 300px ></td>
-                <td align="center"><img src="https://github.com/yoterel/icatcher_plus/blob/master/resource/agreement_vs_confidence.png"  alt="0" width = 400px height = 300px ></td>
-        </tr>
-        <tr><td colspan=2>Lookit</td></tr>
-        <tr>
-                <td><img src="https://github.com/yoterel/icatcher_plus/blob/master/resource/lookit_bar.png" alt="0" width = 400px height = 300px></td>
-                <td><img src="https://github.com/yoterel/icatcher_plus/blob/master/resource/lookit_conf.png" alt="1" width = 300px height = 300px></td>
-        </tr>
-        <tr><td colspan=2>California-BW</td></tr>
-        <tr>
-                <td><img src="https://github.com/yoterel/icatcher_plus/blob/master/resource/cali-bw_bar.png" alt="0" width = 400px height = 300px></td>
-                <td><img src="https://github.com/yoterel/icatcher_plus/blob/master/resource/cali-bw_conf.png" alt="1" width = 300px height = 300px></td>
-        </tr>
-        <tr><td colspan=2>Senegal</td></tr>
-        <tr>
-                <td><img src="https://github.com/yoterel/icatcher_plus/blob/master/resource/senegal_bar.png" alt="0" width = 400px height = 300px></td>
-                <td><img src="https://github.com/yoterel/icatcher_plus/blob/master/resource/senegal_conf.png" alt="1" width = 300px height = 300px></td>
-        </tr>
-</table>
-
-
-# Performance Benchmark
-We benchmarked iCatcher+ performance over 10 videos (res 640 x 480). Reported results are averaged upon all frames.
-
-<table>
-        <tr>
-                <td>iCatcher+ on GPU (NVIDIA GeForce RTX 2060)</td>
-                <td>~45 fps</td>
-        </tr>
-        <tr>
-                <td>iCatcher+ on CPU (Intel Core i7-9700)</td>
-                <td>~17 fps</td>
-        </tr>
-</table>
-
-## Project Structure (subject to change):
-
-    ├── src                     # code for package (inference only)
-    ├── tests                   # tests for package
-    ├── reproduce               # all code used for producing paper results, including training and visualizations.
-    
-# Contributions
-Feel free to contribute by submitting a pull request. Make sure to run all tests under /tests
-
-
+Metadata-Version: 2.1
+Name: icatcher
+Version: 0.1.0
+Summary: iCatcher+: Robust and automated annotation of infant gaze from videos collected in laboratory, field, and online studies.
+Author-email: Yotam Erel <erelyotam@gmail.com>
+License:                     GNU GENERAL PUBLIC LICENSE
+                               Version 3, 29 June 2007
+        
+         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+         Everyone is permitted to copy and distribute verbatim copies
+         of this license document, but changing it is not allowed.
+        
+                                    Preamble
+        
+          The GNU General Public License is a free, copyleft license for
+        software and other kinds of works.
+        
+          The licenses for most software and other practical works are designed
+        to take away your freedom to share and change the works.  By contrast,
+        the GNU General Public License is intended to guarantee your freedom to
+        share and change all versions of a program--to make sure it remains free
+        software for all its users.  We, the Free Software Foundation, use the
+        GNU General Public License for most of our software; it applies also to
+        any other work released this way by its authors.  You can apply it to
+        your programs, too.
+        
+          When we speak of free software, we are referring to freedom, not
+        price.  Our General Public Licenses are designed to make sure that you
+        have the freedom to distribute copies of free software (and charge for
+        them if you wish), that you receive source code or can get it if you
+        want it, that you can change the software or use pieces of it in new
+        free programs, and that you know you can do these things.
+        
+          To protect your rights, we need to prevent others from denying you
+        these rights or asking you to surrender the rights.  Therefore, you have
+        certain responsibilities if you distribute copies of the software, or if
+        you modify it: responsibilities to respect the freedom of others.
+        
+          For example, if you distribute copies of such a program, whether
+        gratis or for a fee, you must pass on to the recipients the same
+        freedoms that you received.  You must make sure that they, too, receive
+        or can get the source code.  And you must show them these terms so they
+        know their rights.
+        
+          Developers that use the GNU GPL protect your rights with two steps:
+        (1) assert copyright on the software, and (2) offer you this License
+        giving you legal permission to copy, distribute and/or modify it.
+        
+          For the developers' and authors' protection, the GPL clearly explains
+        that there is no warranty for this free software.  For both users' and
+        authors' sake, the GPL requires that modified versions be marked as
+        changed, so that their problems will not be attributed erroneously to
+        authors of previous versions.
+        
+          Some devices are designed to deny users access to install or run
+        modified versions of the software inside them, although the manufacturer
+        can do so.  This is fundamentally incompatible with the aim of
+        protecting users' freedom to change the software.  The systematic
+        pattern of such abuse occurs in the area of products for individuals to
+        use, which is precisely where it is most unacceptable.  Therefore, we
+        have designed this version of the GPL to prohibit the practice for those
+        products.  If such problems arise substantially in other domains, we
+        stand ready to extend this provision to those domains in future versions
+        of the GPL, as needed to protect the freedom of users.
+        
+          Finally, every program is threatened constantly by software patents.
+        States should not allow patents to restrict development and use of
+        software on general-purpose computers, but in those that do, we wish to
+        avoid the special danger that patents applied to a free program could
+        make it effectively proprietary.  To prevent this, the GPL assures that
+        patents cannot be used to render the program non-free.
+        
+          The precise terms and conditions for copying, distribution and
+        modification follow.
+        
+                               TERMS AND CONDITIONS
+        
+          0. Definitions.
+        
+          "This License" refers to version 3 of the GNU General Public License.
+        
+          "Copyright" also means copyright-like laws that apply to other kinds of
+        works, such as semiconductor masks.
+        
+          "The Program" refers to any copyrightable work licensed under this
+        License.  Each licensee is addressed as "you".  "Licensees" and
+        "recipients" may be individuals or organizations.
+        
+          To "modify" a work means to copy from or adapt all or part of the work
+        in a fashion requiring copyright permission, other than the making of an
+        exact copy.  The resulting work is called a "modified version" of the
+        earlier work or a work "based on" the earlier work.
+        
+          A "covered work" means either the unmodified Program or a work based
+        on the Program.
+        
+          To "propagate" a work means to do anything with it that, without
+        permission, would make you directly or secondarily liable for
+        infringement under applicable copyright law, except executing it on a
+        computer or modifying a private copy.  Propagation includes copying,
+        distribution (with or without modification), making available to the
+        public, and in some countries other activities as well.
+        
+          To "convey" a work means any kind of propagation that enables other
+        parties to make or receive copies.  Mere interaction with a user through
+        a computer network, with no transfer of a copy, is not conveying.
+        
+          An interactive user interface displays "Appropriate Legal Notices"
+        to the extent that it includes a convenient and prominently visible
+        feature that (1) displays an appropriate copyright notice, and (2)
+        tells the user that there is no warranty for the work (except to the
+        extent that warranties are provided), that licensees may convey the
+        work under this License, and how to view a copy of this License.  If
+        the interface presents a list of user commands or options, such as a
+        menu, a prominent item in the list meets this criterion.
+        
+          1. Source Code.
+        
+          The "source code" for a work means the preferred form of the work
+        for making modifications to it.  "Object code" means any non-source
+        form of a work.
+        
+          A "Standard Interface" means an interface that either is an official
+        standard defined by a recognized standards body, or, in the case of
+        interfaces specified for a particular programming language, one that
+        is widely used among developers working in that language.
+        
+          The "System Libraries" of an executable work include anything, other
+        than the work as a whole, that (a) is included in the normal form of
+        packaging a Major Component, but which is not part of that Major
+        Component, and (b) serves only to enable use of the work with that
+        Major Component, or to implement a Standard Interface for which an
+        implementation is available to the public in source code form.  A
+        "Major Component", in this context, means a major essential component
+        (kernel, window system, and so on) of the specific operating system
+        (if any) on which the executable work runs, or a compiler used to
+        produce the work, or an object code interpreter used to run it.
+        
+          The "Corresponding Source" for a work in object code form means all
+        the source code needed to generate, install, and (for an executable
+        work) run the object code and to modify the work, including scripts to
+        control those activities.  However, it does not include the work's
+        System Libraries, or general-purpose tools or generally available free
+        programs which are used unmodified in performing those activities but
+        which are not part of the work.  For example, Corresponding Source
+        includes interface definition files associated with source files for
+        the work, and the source code for shared libraries and dynamically
+        linked subprograms that the work is specifically designed to require,
+        such as by intimate data communication or control flow between those
+        subprograms and other parts of the work.
+        
+          The Corresponding Source need not include anything that users
+        can regenerate automatically from other parts of the Corresponding
+        Source.
+        
+          The Corresponding Source for a work in source code form is that
+        same work.
+        
+          2. Basic Permissions.
+        
+          All rights granted under this License are granted for the term of
+        copyright on the Program, and are irrevocable provided the stated
+        conditions are met.  This License explicitly affirms your unlimited
+        permission to run the unmodified Program.  The output from running a
+        covered work is covered by this License only if the output, given its
+        content, constitutes a covered work.  This License acknowledges your
+        rights of fair use or other equivalent, as provided by copyright law.
+        
+          You may make, run and propagate covered works that you do not
+        convey, without conditions so long as your license otherwise remains
+        in force.  You may convey covered works to others for the sole purpose
+        of having them make modifications exclusively for you, or provide you
+        with facilities for running those works, provided that you comply with
+        the terms of this License in conveying all material for which you do
+        not control copyright.  Those thus making or running the covered works
+        for you must do so exclusively on your behalf, under your direction
+        and control, on terms that prohibit them from making any copies of
+        your copyrighted material outside their relationship with you.
+        
+          Conveying under any other circumstances is permitted solely under
+        the conditions stated below.  Sublicensing is not allowed; section 10
+        makes it unnecessary.
+        
+          3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+        
+          No covered work shall be deemed part of an effective technological
+        measure under any applicable law fulfilling obligations under article
+        11 of the WIPO copyright treaty adopted on 20 December 1996, or
+        similar laws prohibiting or restricting circumvention of such
+        measures.
+        
+          When you convey a covered work, you waive any legal power to forbid
+        circumvention of technological measures to the extent such circumvention
+        is effected by exercising rights under this License with respect to
+        the covered work, and you disclaim any intention to limit operation or
+        modification of the work as a means of enforcing, against the work's
+        users, your or third parties' legal rights to forbid circumvention of
+        technological measures.
+        
+          4. Conveying Verbatim Copies.
+        
+          You may convey verbatim copies of the Program's source code as you
+        receive it, in any medium, provided that you conspicuously and
+        appropriately publish on each copy an appropriate copyright notice;
+        keep intact all notices stating that this License and any
+        non-permissive terms added in accord with section 7 apply to the code;
+        keep intact all notices of the absence of any warranty; and give all
+        recipients a copy of this License along with the Program.
+        
+          You may charge any price or no price for each copy that you convey,
+        and you may offer support or warranty protection for a fee.
+        
+          5. Conveying Modified Source Versions.
+        
+          You may convey a work based on the Program, or the modifications to
+        produce it from the Program, in the form of source code under the
+        terms of section 4, provided that you also meet all of these conditions:
+        
+            a) The work must carry prominent notices stating that you modified
+            it, and giving a relevant date.
+        
+            b) The work must carry prominent notices stating that it is
+            released under this License and any conditions added under section
+            7.  This requirement modifies the requirement in section 4 to
+            "keep intact all notices".
+        
+            c) You must license the entire work, as a whole, under this
+            License to anyone who comes into possession of a copy.  This
+            License will therefore apply, along with any applicable section 7
+            additional terms, to the whole of the work, and all its parts,
+            regardless of how they are packaged.  This License gives no
+            permission to license the work in any other way, but it does not
+            invalidate such permission if you have separately received it.
+        
+            d) If the work has interactive user interfaces, each must display
+            Appropriate Legal Notices; however, if the Program has interactive
+            interfaces that do not display Appropriate Legal Notices, your
+            work need not make them do so.
+        
+          A compilation of a covered work with other separate and independent
+        works, which are not by their nature extensions of the covered work,
+        and which are not combined with it such as to form a larger program,
+        in or on a volume of a storage or distribution medium, is called an
+        "aggregate" if the compilation and its resulting copyright are not
+        used to limit the access or legal rights of the compilation's users
+        beyond what the individual works permit.  Inclusion of a covered work
+        in an aggregate does not cause this License to apply to the other
+        parts of the aggregate.
+        
+          6. Conveying Non-Source Forms.
+        
+          You may convey a covered work in object code form under the terms
+        of sections 4 and 5, provided that you also convey the
+        machine-readable Corresponding Source under the terms of this License,
+        in one of these ways:
+        
+            a) Convey the object code in, or embodied in, a physical product
+            (including a physical distribution medium), accompanied by the
+            Corresponding Source fixed on a durable physical medium
+            customarily used for software interchange.
+        
+            b) Convey the object code in, or embodied in, a physical product
+            (including a physical distribution medium), accompanied by a
+            written offer, valid for at least three years and valid for as
+            long as you offer spare parts or customer support for that product
+            model, to give anyone who possesses the object code either (1) a
+            copy of the Corresponding Source for all the software in the
+            product that is covered by this License, on a durable physical
+            medium customarily used for software interchange, for a price no
+            more than your reasonable cost of physically performing this
+            conveying of source, or (2) access to copy the
+            Corresponding Source from a network server at no charge.
+        
+            c) Convey individual copies of the object code with a copy of the
+            written offer to provide the Corresponding Source.  This
+            alternative is allowed only occasionally and noncommercially, and
+            only if you received the object code with such an offer, in accord
+            with subsection 6b.
+        
+            d) Convey the object code by offering access from a designated
+            place (gratis or for a charge), and offer equivalent access to the
+            Corresponding Source in the same way through the same place at no
+            further charge.  You need not require recipients to copy the
+            Corresponding Source along with the object code.  If the place to
+            copy the object code is a network server, the Corresponding Source
+            may be on a different server (operated by you or a third party)
+            that supports equivalent copying facilities, provided you maintain
+            clear directions next to the object code saying where to find the
+            Corresponding Source.  Regardless of what server hosts the
+            Corresponding Source, you remain obligated to ensure that it is
+            available for as long as needed to satisfy these requirements.
+        
+            e) Convey the object code using peer-to-peer transmission, provided
+            you inform other peers where the object code and Corresponding
+            Source of the work are being offered to the general public at no
+            charge under subsection 6d.
+        
+          A separable portion of the object code, whose source code is excluded
+        from the Corresponding Source as a System Library, need not be
+        included in conveying the object code work.
+        
+          A "User Product" is either (1) a "consumer product", which means any
+        tangible personal property which is normally used for personal, family,
+        or household purposes, or (2) anything designed or sold for incorporation
+        into a dwelling.  In determining whether a product is a consumer product,
+        doubtful cases shall be resolved in favor of coverage.  For a particular
+        product received by a particular user, "normally used" refers to a
+        typical or common use of that class of product, regardless of the status
+        of the particular user or of the way in which the particular user
+        actually uses, or expects or is expected to use, the product.  A product
+        is a consumer product regardless of whether the product has substantial
+        commercial, industrial or non-consumer uses, unless such uses represent
+        the only significant mode of use of the product.
+        
+          "Installation Information" for a User Product means any methods,
+        procedures, authorization keys, or other information required to install
+        and execute modified versions of a covered work in that User Product from
+        a modified version of its Corresponding Source.  The information must
+        suffice to ensure that the continued functioning of the modified object
+        code is in no case prevented or interfered with solely because
+        modification has been made.
+        
+          If you convey an object code work under this section in, or with, or
+        specifically for use in, a User Product, and the conveying occurs as
+        part of a transaction in which the right of possession and use of the
+        User Product is transferred to the recipient in perpetuity or for a
+        fixed term (regardless of how the transaction is characterized), the
+        Corresponding Source conveyed under this section must be accompanied
+        by the Installation Information.  But this requirement does not apply
+        if neither you nor any third party retains the ability to install
+        modified object code on the User Product (for example, the work has
+        been installed in ROM).
+        
+          The requirement to provide Installation Information does not include a
+        requirement to continue to provide support service, warranty, or updates
+        for a work that has been modified or installed by the recipient, or for
+        the User Product in which it has been modified or installed.  Access to a
+        network may be denied when the modification itself materially and
+        adversely affects the operation of the network or violates the rules and
+        protocols for communication across the network.
+        
+          Corresponding Source conveyed, and Installation Information provided,
+        in accord with this section must be in a format that is publicly
+        documented (and with an implementation available to the public in
+        source code form), and must require no special password or key for
+        unpacking, reading or copying.
+        
+          7. Additional Terms.
+        
+          "Additional permissions" are terms that supplement the terms of this
+        License by making exceptions from one or more of its conditions.
+        Additional permissions that are applicable to the entire Program shall
+        be treated as though they were included in this License, to the extent
+        that they are valid under applicable law.  If additional permissions
+        apply only to part of the Program, that part may be used separately
+        under those permissions, but the entire Program remains governed by
+        this License without regard to the additional permissions.
+        
+          When you convey a copy of a covered work, you may at your option
+        remove any additional permissions from that copy, or from any part of
+        it.  (Additional permissions may be written to require their own
+        removal in certain cases when you modify the work.)  You may place
+        additional permissions on material, added by you to a covered work,
+        for which you have or can give appropriate copyright permission.
+        
+          Notwithstanding any other provision of this License, for material you
+        add to a covered work, you may (if authorized by the copyright holders of
+        that material) supplement the terms of this License with terms:
+        
+            a) Disclaiming warranty or limiting liability differently from the
+            terms of sections 15 and 16 of this License; or
+        
+            b) Requiring preservation of specified reasonable legal notices or
+            author attributions in that material or in the Appropriate Legal
+            Notices displayed by works containing it; or
+        
+            c) Prohibiting misrepresentation of the origin of that material, or
+            requiring that modified versions of such material be marked in
+            reasonable ways as different from the original version; or
+        
+            d) Limiting the use for publicity purposes of names of licensors or
+            authors of the material; or
+        
+            e) Declining to grant rights under trademark law for use of some
+            trade names, trademarks, or service marks; or
+        
+            f) Requiring indemnification of licensors and authors of that
+            material by anyone who conveys the material (or modified versions of
+            it) with contractual assumptions of liability to the recipient, for
+            any liability that these contractual assumptions directly impose on
+            those licensors and authors.
+        
+          All other non-permissive additional terms are considered "further
+        restrictions" within the meaning of section 10.  If the Program as you
+        received it, or any part of it, contains a notice stating that it is
+        governed by this License along with a term that is a further
+        restriction, you may remove that term.  If a license document contains
+        a further restriction but permits relicensing or conveying under this
+        License, you may add to a covered work material governed by the terms
+        of that license document, provided that the further restriction does
+        not survive such relicensing or conveying.
+        
+          If you add terms to a covered work in accord with this section, you
+        must place, in the relevant source files, a statement of the
+        additional terms that apply to those files, or a notice indicating
+        where to find the applicable terms.
+        
+          Additional terms, permissive or non-permissive, may be stated in the
+        form of a separately written license, or stated as exceptions;
+        the above requirements apply either way.
+        
+          8. Termination.
+        
+          You may not propagate or modify a covered work except as expressly
+        provided under this License.  Any attempt otherwise to propagate or
+        modify it is void, and will automatically terminate your rights under
+        this License (including any patent licenses granted under the third
+        paragraph of section 11).
+        
+          However, if you cease all violation of this License, then your
+        license from a particular copyright holder is reinstated (a)
+        provisionally, unless and until the copyright holder explicitly and
+        finally terminates your license, and (b) permanently, if the copyright
+        holder fails to notify you of the violation by some reasonable means
+        prior to 60 days after the cessation.
+        
+          Moreover, your license from a particular copyright holder is
+        reinstated permanently if the copyright holder notifies you of the
+        violation by some reasonable means, this is the first time you have
+        received notice of violation of this License (for any work) from that
+        copyright holder, and you cure the violation prior to 30 days after
+        your receipt of the notice.
+        
+          Termination of your rights under this section does not terminate the
+        licenses of parties who have received copies or rights from you under
+        this License.  If your rights have been terminated and not permanently
+        reinstated, you do not qualify to receive new licenses for the same
+        material under section 10.
+        
+          9. Acceptance Not Required for Having Copies.
+        
+          You are not required to accept this License in order to receive or
+        run a copy of the Program.  Ancillary propagation of a covered work
+        occurring solely as a consequence of using peer-to-peer transmission
+        to receive a copy likewise does not require acceptance.  However,
+        nothing other than this License grants you permission to propagate or
+        modify any covered work.  These actions infringe copyright if you do
+        not accept this License.  Therefore, by modifying or propagating a
+        covered work, you indicate your acceptance of this License to do so.
+        
+          10. Automatic Licensing of Downstream Recipients.
+        
+          Each time you convey a covered work, the recipient automatically
+        receives a license from the original licensors, to run, modify and
+        propagate that work, subject to this License.  You are not responsible
+        for enforcing compliance by third parties with this License.
+        
+          An "entity transaction" is a transaction transferring control of an
+        organization, or substantially all assets of one, or subdividing an
+        organization, or merging organizations.  If propagation of a covered
+        work results from an entity transaction, each party to that
+        transaction who receives a copy of the work also receives whatever
+        licenses to the work the party's predecessor in interest had or could
+        give under the previous paragraph, plus a right to possession of the
+        Corresponding Source of the work from the predecessor in interest, if
+        the predecessor has it or can get it with reasonable efforts.
+        
+          You may not impose any further restrictions on the exercise of the
+        rights granted or affirmed under this License.  For example, you may
+        not impose a license fee, royalty, or other charge for exercise of
+        rights granted under this License, and you may not initiate litigation
+        (including a cross-claim or counterclaim in a lawsuit) alleging that
+        any patent claim is infringed by making, using, selling, offering for
+        sale, or importing the Program or any portion of it.
+        
+          11. Patents.
+        
+          A "contributor" is a copyright holder who authorizes use under this
+        License of the Program or a work on which the Program is based.  The
+        work thus licensed is called the contributor's "contributor version".
+        
+          A contributor's "essential patent claims" are all patent claims
+        owned or controlled by the contributor, whether already acquired or
+        hereafter acquired, that would be infringed by some manner, permitted
+        by this License, of making, using, or selling its contributor version,
+        but do not include claims that would be infringed only as a
+        consequence of further modification of the contributor version.  For
+        purposes of this definition, "control" includes the right to grant
+        patent sublicenses in a manner consistent with the requirements of
+        this License.
+        
+          Each contributor grants you a non-exclusive, worldwide, royalty-free
+        patent license under the contributor's essential patent claims, to
+        make, use, sell, offer for sale, import and otherwise run, modify and
+        propagate the contents of its contributor version.
+        
+          In the following three paragraphs, a "patent license" is any express
+        agreement or commitment, however denominated, not to enforce a patent
+        (such as an express permission to practice a patent or covenant not to
+        sue for patent infringement).  To "grant" such a patent license to a
+        party means to make such an agreement or commitment not to enforce a
+        patent against the party.
+        
+          If you convey a covered work, knowingly relying on a patent license,
+        and the Corresponding Source of the work is not available for anyone
+        to copy, free of charge and under the terms of this License, through a
+        publicly available network server or other readily accessible means,
+        then you must either (1) cause the Corresponding Source to be so
+        available, or (2) arrange to deprive yourself of the benefit of the
+        patent license for this particular work, or (3) arrange, in a manner
+        consistent with the requirements of this License, to extend the patent
+        license to downstream recipients.  "Knowingly relying" means you have
+        actual knowledge that, but for the patent license, your conveying the
+        covered work in a country, or your recipient's use of the covered work
+        in a country, would infringe one or more identifiable patents in that
+        country that you have reason to believe are valid.
+        
+          If, pursuant to or in connection with a single transaction or
+        arrangement, you convey, or propagate by procuring conveyance of, a
+        covered work, and grant a patent license to some of the parties
+        receiving the covered work authorizing them to use, propagate, modify
+        or convey a specific copy of the covered work, then the patent license
+        you grant is automatically extended to all recipients of the covered
+        work and works based on it.
+        
+          A patent license is "discriminatory" if it does not include within
+        the scope of its coverage, prohibits the exercise of, or is
+        conditioned on the non-exercise of one or more of the rights that are
+        specifically granted under this License.  You may not convey a covered
+        work if you are a party to an arrangement with a third party that is
+        in the business of distributing software, under which you make payment
+        to the third party based on the extent of your activity of conveying
+        the work, and under which the third party grants, to any of the
+        parties who would receive the covered work from you, a discriminatory
+        patent license (a) in connection with copies of the covered work
+        conveyed by you (or copies made from those copies), or (b) primarily
+        for and in connection with specific products or compilations that
+        contain the covered work, unless you entered into that arrangement,
+        or that patent license was granted, prior to 28 March 2007.
+        
+          Nothing in this License shall be construed as excluding or limiting
+        any implied license or other defenses to infringement that may
+        otherwise be available to you under applicable patent law.
+        
+          12. No Surrender of Others' Freedom.
+        
+          If conditions are imposed on you (whether by court order, agreement or
+        otherwise) that contradict the conditions of this License, they do not
+        excuse you from the conditions of this License.  If you cannot convey a
+        covered work so as to satisfy simultaneously your obligations under this
+        License and any other pertinent obligations, then as a consequence you may
+        not convey it at all.  For example, if you agree to terms that obligate you
+        to collect a royalty for further conveying from those to whom you convey
+        the Program, the only way you could satisfy both those terms and this
+        License would be to refrain entirely from conveying the Program.
+        
+          13. Use with the GNU Affero General Public License.
+        
+          Notwithstanding any other provision of this License, you have
+        permission to link or combine any covered work with a work licensed
+        under version 3 of the GNU Affero General Public License into a single
+        combined work, and to convey the resulting work.  The terms of this
+        License will continue to apply to the part which is the covered work,
+        but the special requirements of the GNU Affero General Public License,
+        section 13, concerning interaction through a network will apply to the
+        combination as such.
+        
+          14. Revised Versions of this License.
+        
+          The Free Software Foundation may publish revised and/or new versions of
+        the GNU General Public License from time to time.  Such new versions will
+        be similar in spirit to the present version, but may differ in detail to
+        address new problems or concerns.
+        
+          Each version is given a distinguishing version number.  If the
+        Program specifies that a certain numbered version of the GNU General
+        Public License "or any later version" applies to it, you have the
+        option of following the terms and conditions either of that numbered
+        version or of any later version published by the Free Software
+        Foundation.  If the Program does not specify a version number of the
+        GNU General Public License, you may choose any version ever published
+        by the Free Software Foundation.
+        
+          If the Program specifies that a proxy can decide which future
+        versions of the GNU General Public License can be used, that proxy's
+        public statement of acceptance of a version permanently authorizes you
+        to choose that version for the Program.
+        
+          Later license versions may give you additional or different
+        permissions.  However, no additional obligations are imposed on any
+        author or copyright holder as a result of your choosing to follow a
+        later version.
+        
+          15. Disclaimer of Warranty.
+        
+          THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+        APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+        HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+        OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+        THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+        PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+        IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+        ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+        
+          16. Limitation of Liability.
+        
+          IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+        WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+        THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+        GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+        USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+        DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+        PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+        EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+        SUCH DAMAGES.
+        
+          17. Interpretation of Sections 15 and 16.
+        
+          If the disclaimer of warranty and limitation of liability provided
+        above cannot be given local legal effect according to their terms,
+        reviewing courts shall apply local law that most closely approximates
+        an absolute waiver of all civil liability in connection with the
+        Program, unless a warranty or assumption of liability accompanies a
+        copy of the Program in return for a fee.
+        
+                             END OF TERMS AND CONDITIONS
+        
+                    How to Apply These Terms to Your New Programs
+        
+          If you develop a new program, and you want it to be of the greatest
+        possible use to the public, the best way to achieve this is to make it
+        free software which everyone can redistribute and change under these terms.
+        
+          To do so, attach the following notices to the program.  It is safest
+        to attach them to the start of each source file to most effectively
+        state the exclusion of warranty; and each file should have at least
+        the "copyright" line and a pointer to where the full notice is found.
+        
+            <one line to give the program's name and a brief idea of what it does.>
+            Copyright (C) <year>  <name of author>
+        
+            This program is free software: you can redistribute it and/or modify
+            it under the terms of the GNU General Public License as published by
+            the Free Software Foundation, either version 3 of the License, or
+            (at your option) any later version.
+        
+            This program is distributed in the hope that it will be useful,
+            but WITHOUT ANY WARRANTY; without even the implied warranty of
+            MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+            GNU General Public License for more details.
+        
+            You should have received a copy of the GNU General Public License
+            along with this program.  If not, see <https://www.gnu.org/licenses/>.
+        
+        Also add information on how to contact you by electronic and paper mail.
+        
+          If the program does terminal interaction, make it output a short
+        notice like this when it starts in an interactive mode:
+        
+            <program>  Copyright (C) <year>  <name of author>
+            This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+            This is free software, and you are welcome to redistribute it
+            under certain conditions; type `show c' for details.
+        
+        The hypothetical commands `show w' and `show c' should show the appropriate
+        parts of the General Public License.  Of course, your program's commands
+        might be different; for a GUI interface, you would use an "about box".
+        
+          You should also get your employer (if you work as a programmer) or school,
+        if any, to sign a "copyright disclaimer" for the program, if necessary.
+        For more information on this, and how to apply and follow the GNU GPL, see
+        <https://www.gnu.org/licenses/>.
+        
+          The GNU General Public License does not permit incorporating your program
+        into proprietary programs.  If your program is a subroutine library, you
+        may consider it more useful to permit linking proprietary applications with
+        the library.  If this is what you want to do, use the GNU Lesser General
+        Public License instead of this License.  But first, please read
+        <https://www.gnu.org/licenses/why-not-lgpl.html>.
+        
+Project-URL: Homepage, https://github.com/yoterel/icatcher_plus
+Keywords: eyetracker,eyetracking
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: build
+Provides-Extra: dev
+License-File: LICENSE
+
+[![DOI](https://zenodo.org/badge/486841882.svg)](https://zenodo.org/badge/latestdoi/486841882)
+
+# iCatcher+
+
+# Introduction
+This repository contains the official code for [iCatcher+](https://doi.org/10.1177/25152459221147250), a tool for performing automatic annotation of discrete infant gaze directions from videos collected in the lab, field or online (remotely). It also contains code for reproducing the original paper results.
+
+Click below for a video including examples of representative good and poor performance, taken from videos of infants participating in online research (all families featured consented to sharing their video data publicly):
+
+[![iCatcher representative good and poor performance](https://img.youtube.com/vi/iK_T2P2ZDnU/0.jpg)](https://www.youtube.com/watch?v=iK_T2P2ZDnU)
+
+# Installation
+## Quick installation (Windows, Linux, Mac)
+This option will let you use iCatcher+ with minimum effort, but only for predictions (inference).
+We strongly recommend using a virtual environment such as [Miniconda](https://conda.io) or [virtualenv](https://pypi.org/project/virtualenv/) before running the command below.
+
+`pip install icatcher`
+
+You will also need [ffmpeg](https://www.ffmpeg.org/) installed in your system and available (if you used conda, you can quickly install it with `conda install -c conda-forge ffmpeg`).
+
+Note1:
+If you require speedy performance, prior to installing icatcher you should install [PyTorch](https://pytorch.org/) with GPU support (see [here](https://pytorch.org/get-started/locally/) for instructions). This assumes you have a supported GPU on your machine.
+
+Note2:
+When using iCatcher+ for the first time, neural network model files will automatically be downloaded to a local cache folder. To control where they are downloaded to set the "ICATCHER_DATA_DIR" environment variable.
+
+## Reproduction of original research results / retraining on your own dataset
+
+see [reproduce](https://github.com/icatcherplus/icatcher_plus/tree/master/reproduce) for a full set of instructions.
+
+# Running iCatcher+
+
+You can run iCatcher+ with the command:
+
+`icatcher --help`
+
+which will list all available options. Description below will help you get more familiar with some common command line arguments.
+
+To run iCatcher+ with a video file (if a folder is provided, all videos will be used for prediction):
+
+`icatcher /path/to/my/video.mp4`
+
+A common option is to add:
+
+`icatcher /path/to/my/video.mp4 --use_fc_model`
+
+Which enables a child face detector for more robust results (however, sometimes this can result in too much loss of data).
+
+You can save a labeled video by adding:
+
+`--output_video_path /path/to/output_folder`
+
+If you want to output annotations to a file, use:
+
+`--output_annotation /path/to/output_annotation_folder`
+
+To show the predictions online in a seperate window, add the option:
+
+`--show_output`
+
+You can also add parameters to crop the video a given percent before passing to iCatcher: 
+
+`--crop_mode m` where `m` is any of [top, left, right], specifying which side of the video to crop from (if not provided, default is none; if crop_percent is provided but not crop_mode, default is top)
+
+`--crop_percent x` where `x` is an integer (default = 0) specifying what percent of the video size to crop from the specified side. E.g., if `--crop_mode top` is provided with `--crop_percent 10`, 10% of the video height will be cropped from the top. If `--crop_mode left` is provided with `--crop_percent 25`, 25% of the video width will be cropped from the left side, etc. 
+
+# Output format
+
+Currently we supports 2 output formats, though further formats can be added upon request.
+
+- raw_output: a file where each row will contain the frame number, the class prediction and the confidence of that prediction seperated by a comma
+- compressed: a npz file containing two numpy arrays, one encoding the predicted class (n x 1 int32) and another the confidence (n x 1 float32) where n is the number of frames. This file can be loaded into memory using the numpy.load function. For the map between class number and name see test.py ("predict_from_video" function).
+
+# Datasets access
+
+The public videos from the Lookit dataset, along with human annotations and group-level demographics for all datasets, are available at https://osf.io/ujteb/. Videos from the Lookit dataset with permission granted for scientific use are available at https://osf.io/5u9df/. Requests for access can be directed to Junyi Chu (junyichu@mit.edu).
+
+Requests for access to the remainder of the datasets (Cali-BW, Senegal) can be directed to Dr. Katherine Adams Shannon (katashannon@gmail.com). Note that access to raw video files from the California-BW and Senegal datasets *is not available* due to restricted participant privacy agreements. To protect participant privacy, the participant identifiers for the video and demographic data are not linked to each other. However, this information is available upon reasonable request.
+
+# Performance Benchmark
+We benchmarked iCatcher+ performance over 10 videos (res 640 x 480). Reported results are averaged upon all frames.
+
+<table>
+        <tr>
+                <td>iCatcher+ on GPU (NVIDIA GeForce RTX 2060)</td>
+                <td>~45 fps</td>
+        </tr>
+        <tr>
+                <td>iCatcher+ on CPU (Intel Core i7-9700)</td>
+                <td>~17 fps</td>
+        </tr>
+</table>
+
+## Project Structure (subject to change):
+
+    ├── src                     # code for package (inference only)
+    ├── tests                   # tests for package
+    ├── reproduce               # all code used for producing paper results, including training and visualizations.
+    
+# Troubleshooting Issues
+Please open a github issue for any question or problem you encounter. We kindly ask to first skim through closed issues to see if your problem was already addressed.
+
+# Citation
+```
+@article{doi:10.1177/25152459221147250,
+author = {Yotam Erel and Katherine Adams Shannon and Junyi Chu and Kim Scott and Melissa Kline Struhl and Peng Cao and Xincheng Tan and Peter Hart and Gal Raz and Sabrina Piccolo and Catherine Mei and Christine Potter and Sagi Jaffe-Dax and Casey Lew-Williams and Joshua Tenenbaum and Katherine Fairchild and Amit Bermano and Shari Liu},
+title ={iCatcher+: Robust and Automated Annotation of Infants’ and Young Children’s Gaze Behavior From Videos Collected in Laboratory, Field, and Online Studies},
+journal = {Advances in Methods and Practices in Psychological Science},
+volume = {6},
+number = {2},
+pages = {25152459221147250},
+year = {2023},
+doi = {10.1177/25152459221147250},
+URL = { 
+        https://doi.org/10.1177/25152459221147250
+},
+eprint = { 
+        https://doi.org/10.1177/25152459221147250 
+}
+}
+```
+
+
```

