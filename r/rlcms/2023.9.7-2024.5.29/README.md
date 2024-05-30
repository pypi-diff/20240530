# Comparing `tmp/rlcms-2023.9.7.tar.gz` & `tmp/rlcms-2024.5.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlcms-2023.9.7.tar", last modified: Thu Sep  7 19:03:22 2023, max compression
+gzip compressed data, was "rlcms-2024.5.29.tar", last modified: Thu May 30 14:13:07 2024, max compression
```

## Comparing `rlcms-2023.9.7.tar` & `rlcms-2024.5.29.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-09-07 19:03:22.807619 rlcms-2023.9.7/
--rw-rw-rw-   0        0        0    35801 2023-09-01 20:24:11.000000 rlcms-2023.9.7/LICENSE
--rw-rw-rw-   0        0        0    47726 2023-09-07 19:03:22.806623 rlcms-2023.9.7/PKG-INFO
--rw-rw-rw-   0        0        0     5924 2023-09-07 18:57:41.000000 rlcms-2023.9.7/README.md
--rw-rw-rw-   0        0        0     1044 2023-09-07 18:52:05.000000 rlcms-2023.9.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-09-07 19:03:22.808618 rlcms-2023.9.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-09-07 19:03:22.751768 rlcms-2023.9.7/src/
-drwxrwxrwx   0        0        0        0 2023-09-07 19:03:22.770717 rlcms-2023.9.7/src/rlcms/
--rw-rw-rw-   0        0        0       18 2023-09-07 15:18:05.000000 rlcms-2023.9.7/src/rlcms/__init__.py
--rw-rw-rw-   0        0        0     1335 2023-09-01 19:45:59.000000 rlcms-2023.9.7/src/rlcms/assemblage.py
-drwxrwxrwx   0        0        0        0 2023-09-07 19:03:22.802632 rlcms-2023.9.7/src/rlcms/cli/
--rw-rw-rw-   0        0        0     3821 2023-09-07 17:30:54.000000 rlcms-2023.9.7/src/rlcms/cli/RFprimitives.py
--rw-rw-rw-   0        0        0     4929 2023-09-07 17:28:45.000000 rlcms-2023.9.7/src/rlcms/cli/composite.py
--rw-rw-rw-   0        0        0     2008 2023-09-07 17:30:44.000000 rlcms-2023.9.7/src/rlcms/cli/generate_LC.py
--rw-rw-rw-   0        0        0     7127 2023-09-07 17:31:02.000000 rlcms-2023.9.7/src/rlcms/cli/sample_pts.py
--rw-rw-rw-   0        0        0     5508 2023-09-07 17:31:31.000000 rlcms-2023.9.7/src/rlcms/cli/train_test.py
--rw-rw-rw-   0        0        0     9694 2023-09-07 18:06:21.000000 rlcms-2023.9.7/src/rlcms/composites.py
--rw-rw-rw-   0        0        0    12369 2023-09-07 17:30:27.000000 rlcms-2023.9.7/src/rlcms/covariates.py
--rw-rw-rw-   0        0        0     6581 2023-09-01 19:45:59.000000 rlcms-2023.9.7/src/rlcms/harmonics.py
--rw-rw-rw-   0        0        0     6289 2023-09-07 17:32:04.000000 rlcms-2023.9.7/src/rlcms/primitives.py
--rw-rw-rw-   0        0        0     8457 2023-09-01 19:45:59.000000 rlcms-2023.9.7/src/rlcms/sampling.py
--rw-rw-rw-   0        0        0     2153 2023-09-01 19:45:59.000000 rlcms-2023.9.7/src/rlcms/utils.py
-drwxrwxrwx   0        0        0        0 2023-09-07 19:03:22.795650 rlcms-2023.9.7/src/rlcms.egg-info/
--rw-rw-rw-   0        0        0    47726 2023-09-07 19:03:22.000000 rlcms-2023.9.7/src/rlcms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      581 2023-09-07 19:03:22.000000 rlcms-2023.9.7/src/rlcms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-07 19:03:22.000000 rlcms-2023.9.7/src/rlcms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      215 2023-09-07 19:03:22.000000 rlcms-2023.9.7/src/rlcms.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       49 2023-09-07 19:03:22.000000 rlcms-2023.9.7/src/rlcms.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-09-07 19:03:22.000000 rlcms-2023.9.7/src/rlcms.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-09-07 19:03:22.804627 rlcms-2023.9.7/tests/
--rw-rw-rw-   0        0        0     1654 2023-09-07 18:11:22.000000 rlcms-2023.9.7/tests/test_composites.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:13:07.344457 rlcms-2024.5.29/
+-rw-r--r--   0 runner    (1001) docker     (127)    35128 2024-05-30 14:13:00.000000 rlcms-2024.5.29/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    42573 2024-05-30 14:13:07.344457 rlcms-2024.5.29/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-30 14:13:00.000000 rlcms-2024.5.29/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-30 14:13:00.000000 rlcms-2024.5.29/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 14:13:07.344457 rlcms-2024.5.29/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:13:07.340457 rlcms-2024.5.29/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:13:07.340457 rlcms-2024.5.29/src/rlcms/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 14:13:00.000000 rlcms-2024.5.29/src/rlcms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:13:07.344457 rlcms-2024.5.29/src/rlcms/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-05-30 14:13:00.000000 rlcms-2024.5.29/src/rlcms/cli/composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-30 14:13:00.000000 rlcms-2024.5.29/src/rlcms/cli/landcover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-30 14:13:00.000000 rlcms-2024.5.29/src/rlcms/cli/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-05-30 14:13:00.000000 rlcms-2024.5.29/src/rlcms/cli/sample_pts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-05-30 14:13:00.000000 rlcms-2024.5.29/src/rlcms/cli/train_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8742 2024-05-30 14:13:00.000000 rlcms-2024.5.29/src/rlcms/composites.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12021 2024-05-30 14:13:00.000000 rlcms-2024.5.29/src/rlcms/covariates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-05-30 14:13:00.000000 rlcms-2024.5.29/src/rlcms/harmonics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14717 2024-05-30 14:13:00.000000 rlcms-2024.5.29/src/rlcms/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12778 2024-05-30 14:13:00.000000 rlcms-2024.5.29/src/rlcms/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8390 2024-05-30 14:13:00.000000 rlcms-2024.5.29/src/rlcms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:13:07.344457 rlcms-2024.5.29/src/rlcms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    42573 2024-05-30 14:13:07.000000 rlcms-2024.5.29/src/rlcms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-30 14:13:07.000000 rlcms-2024.5.29/src/rlcms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 14:13:07.000000 rlcms-2024.5.29/src/rlcms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-30 14:13:07.000000 rlcms-2024.5.29/src/rlcms.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 14:13:07.000000 rlcms-2024.5.29/src/rlcms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-30 14:13:07.000000 rlcms-2024.5.29/src/rlcms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:13:07.344457 rlcms-2024.5.29/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-30 14:13:00.000000 rlcms-2024.5.29/tests/test_composites.py
```

### Comparing `rlcms-2023.9.7/LICENSE` & `rlcms-2024.5.29/LICENSE`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-GNU GENERAL PUBLIC LICENSE
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
+GNU GENERAL PUBLIC LICENSE
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
 <https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `rlcms-2023.9.7/PKG-INFO` & `rlcms-2024.5.29/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,800 +1,745 @@
-Metadata-Version: 2.1
-Name: rlcms
-Version: 2023.9.7
-Summary: workflows for regional land cover mapping, built in Google Earth Engine
-Author-email: Kyle Woodward <kw.geospatial@gmail.com>
-License: GNU GENERAL PUBLIC LICENSE
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
-Project-URL: Homepage, https://github.com/sig-gis/rlcms/
-Keywords: land cover,mapping
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: earthengine-api
-Requires-Dist: hydrafloods
-Requires-Dist: pandas
-Provides-Extra: dev
-Requires-Dist: geemap; extra == "dev"
-
-# Running Regional Land Cover Monitoring System Toolset
-## Installation
-Install with pip: 
-```
-pip install rlcms
-```
-
-## GEE Python API Setup
-Earth Engine requires you to authenticate your account credentials to access the Earth Engine python API and your chosen Cloud Project. We do this with the `gcloud` python utility
-1. Download the installer for the `glcoud` command-line python [utility](https://cloud.google.com/sdk/docs/install) from Google
-2. Run the installer
-3. Select Single User and use the default Destination Folder
-4. Leave the Selected Components to Install as-is and click Install
-5. Leave all four boxes checked, and click Finish. This will open a new command-prompt window and auto run gcloud initialization
-6. It asks whether you'd like to log in, type y - this will open a new browser window to a Google Authentication page
-
-![kaza_readme_gcloudInstaller_initializing](https://user-images.githubusercontent.com/51868526/184163126-7505745b-f7c3-4745-bb36-3948d1b9ff76.JPG)
-
-7. Choose your Google account that is linked to your Earth Engine account, then click Allow on the next page.
-
-![kaza_readme_gcloudInstaller_InitializingSignIn](https://user-images.githubusercontent.com/51868526/184163514-4604ac83-cdad-4dd8-bc67-c37224d6aafc.JPG)
-
-8. You will be redirected to a page that says "You are now authenticated with the gcloud CLI!"
-9. Go back to your shell that had been opened for you by gcloud. It asks you to choose a cloud project and lists all available cloud projects that your google account has access to. Decide which project to authenticate with by typing its number in the list.
-
-![kaza_readme_gcloudInstaller_chooseCloudProject_chooseWWF-SIG](https://user-images.githubusercontent.com/51868526/184165192-c602f058-b485-419c-b5ea-401c7087fb9f.JPG)
-
-10. Back in your separate shell window, first ensure you are in your custom conda env (running `conda activate env-name`), then run:
-```
-earthengine authenticate
-```
-11. In the browser window that opens, select the Google account that is tied to your EE account, select the wwf-sig cloud project, then click Generate Token at the bottom of the page.
-12. On the next page, select your Google account again, then click Allow on the next page.
-13. Copy the authorization token it generates to your clipboard and back in your shell, paste it and hit Enter. 
-
-# Testing Your Setup
-Test that earthengine is setup and authenticated by checking the folder contents within the `wwf-sig` cloud project. 
-* In your shell, run:
-```
-earthengine set_project <project-name>
-earthengine ls projects/project-name/assets
-```
-
-If you do not get an error and it returns a list of folders and assets similar to this then you are good to go! :tada:
-
-# Tool Documentation
-
-Each Command Line Interface (CLI) script tool can be run in your command-line terminal of choice. The user must provide values for each required command-line argument to control the analysis.
-You can first run any script, only declaring the `-h` flag. This will bring up the help dialog with a usage example and a description of required command-line arguments. 
-
-## **sample_pts**
-
-Generate Random Sample Points From an ee.Image, Formatted for Collect Earth Online
-
-The points are pre-formatted for use in Collect Earth Online. You can choose to export the points to Google Drive, to GEE Asset or both. 
-
-example:
-```
-sample_pts -im input/path/to/image -band LANDCOVER -o output/path --n_points 100 --to_drive
-```
-
-## **composite**
-
-Creates a Sentinel-2 Composite for an AOI or reference polygons. 
-
-The resulting band stack is needed for both extracting training data information and as input to a trained model's inference. Set the `-p` flag if your AOI is a set of reference polygons and not one contiguous AOI polygon - this will export band information only within each polygon's footprint. 
-
-example:
-```
-composite -a aoi/fc/path -d Landsat8 -s 2020-01-01 -e 2020-12-31 -o output/path --settings path/to/settings/file.txt
-```
-
-**NOTE: The user can control which spectral indices and time series features to generate in this tool by providing a settings txt file, a template of which is located in the repository : [`/template_settings.txt`](/template_settings.txt). See [ProjectWorkflow.md](/ProjectWorkflow.md) for details.**
-
-## **train_test**
-
-Extract Train and Test Point Data from an Input Image within Reference Polygon Areas.
-
-Generates stratified random samples from reference polygons, splitting the sample points into train and test points if desired. The image bands from the provided image are extracted to every point. 
-
-example:
-```
-train_test -rp path/to/reference_polygon_fc -im path/to/input/stack -o unique/output/path --class_values 1 2 3 4 5 6 7 8 --class_points 10 10 10 10 10 10 10
-```
-
-## **primitives**
-
-Create Land Cover Primitives For All Classes in Provided Training Data. 
-
-This script trains probability Random Forest models for each land cover class in your typology as provided by the numeric 'LANDCOVER' property in the provided reference data. It then exports these binary probability images one land cover at a time into a land cover 'Primitives' image collection. While doing so, it also reports out some model performance metrics saved to a new folder created in your *local* `rlcms/metrics` folder on your computer.
-
-example:
-```
-primitives -i input/stack/path -t training/data/path -o output/primitives/imagecollection/path
-```
-
-## **generate_LC**
-
-Generate Single Land Cover Image From Land Cover Primitives Image Collection
-
-This script takes the RF primitives collection generated from the previous script and creates a single-band land cover image from them, taking the highest-probability Primitive at each pixel to assign the Land Cover class.
-
-example:
-```
-generate_LC -i input/primitives/imagecollection/path -o output/path
-```
-
-
+Metadata-Version: 2.1
+Name: rlcms
+Version: 2024.5.29
+Summary: workflows for regional land cover mapping, built in Google Earth Engine
+Author-email: Kyle Woodward <kw.geospatial@gmail.com>
+License: GNU GENERAL PUBLIC LICENSE
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
+Project-URL: Homepage, https://github.com/sig-gis/rlcms/
+Keywords: land cover,mapping
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: earthengine-api
+Requires-Dist: hydrafloods
+Requires-Dist: pandas
+Provides-Extra: dev
+Requires-Dist: geemap; extra == "dev"
+
+# Regional Land Cover Monitoring System
+## Installation
+Install with pip: 
+```
+pip install rlcms
+```
+
+Test that `earthengine-api` is setup and authenticated by checking the folder contents within one of your cloud projects. 
+* In your shell, run:
+```
+earthengine set_project <project-name>
+earthengine ls projects/project-name/assets
+```
+If you do not get an error and it returns a list of folders and assets similar to this then you are good to go! :tada:
+
+## Features
+
+* stratified sampling for use in Collect Earth Online
+* Training and validation data extraction, from points or polygon references
+* Land cover modeling using Primitive ensembles, complete with model metrics for iterative improvements
+
+## Quick Start
+
+```
+from rlcms.composites import Composite
+# Create an annual Sentinel-1 Composite
+c = Composite(dataset='Sentinel1',
+        region=aoi,
+        start_date='2020-01-01',
+        end_date='2021-12-31',
+        composite_mode='annual',
+        reducer='median')
+
+# look at the Composite object
+print(c.__dict__)
+
+# retrieve band names
+print(f"Composite bands:{c.bands}")
+
+# retrieve ee.Image from Composite object 
+image = c.image
+```
+
+## Contributing
+
+We welcome contributions from the community. If there are issues are improvements, please submit an issue on Github: [https://github.com/sig-gis/rlcms](https://github.com/sig-gis/rlcms)
+
+## License
+
+This project is licensed under the GPL-3 License - see the LICENSE file for details.
+
+
+
```

### Comparing `rlcms-2023.9.7/src/rlcms/cli/RFprimitives.py` & `rlcms-2024.5.29/src/rlcms/cli/primitives.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,117 +1,145 @@
-import ee
-import os
-from pathlib import Path
-import argparse
-from rlcms.utils import check_exists
-from rlcms.primitives import primitives_to_collection
-
-def main():
-    ee.Initialize()
-
-    parser = argparse.ArgumentParser(
-    description="Create Land Cover Primitives For All Classes in Provided Training Data",
-    usage = "RFprimitives -i path/to/input_stack -t path/to/training_data -o path/to/output"
-    )
-    
-    parser.add_argument(
-        "-i",
-        "--input_stack",
-        type=str,
-        required=True,
-        help="full asset path to input stack"
-    )
-    
-    parser.add_argument(
-    "-t",
-    "--training_data",
-    type=str, 
-    nargs='+',
-    required=True,
-    help="full asset path(s) to training point dataset(s)"
-    )
-    
-    parser.add_argument(
-    "-c",
-    "--crs",
-    type=str,
-    required=False,
-    help="CRS string in format of EPSG:xxxxx. Defaults to EPSG:4326"
-    )
-    
-    parser.add_argument(
-        "-o",
-        "--output",
-        type=str,
-        required=True,
-        help="The output asset path of the primitives image collection."
-    )
-
-    parser.add_argument(
-        "-d",
-        "--dry_run",
-        dest="dry_run",
-        action="store_true",
-        help="goes through checks and prints paths to outputs but does not export them.",
-        )
-
-    args = parser.parse_args()
-
-    input_stack_path = args.input_stack
-    train_paths = args.training_data
-    output = args.output
-    crs = args.crs
-    dry_run = args.dry_run
-
-    # Run Checks
-    # Check input stack exists
-    assert check_exists(input_stack_path) == 0, f"Check input_stack asset exists: {input_stack_path}"
-    
-    # Check training data exists
-    for train_path in train_paths:
-        assert check_exists(train_path) == 0, f"Check training_data asset exists: {train_path}"
-             
-    img_coll_path = output
-    output_folder = os.path.dirname(output)
-    # check output folder exists
-    assert check_exists(output_folder) == 0, f"Check parent folder exists: {output_folder}"
-    
-    # don't allow ee.Image exports to pre-existing ee.ImageCollections
-    if check_exists(img_coll_path) == 0:
-        raise AssertionError(f"Primitives ImageCollection already exists: {img_coll_path}")
-
-    # Construct local 'metrics' folder path from -o output or a default name if not provided
-    cwd = os.getcwd()
-    metrics_path = os.path.join(cwd,"metrics",os.path.basename(img_coll_path))
-
-    # print output locations and exit
-    if dry_run: 
-        print(f"Would Export Primitives ImageCollection to: {img_coll_path}\n")
-        print(f"Would Export Model Metrics to: {metrics_path}\n")
-        exit()
-    
-    else:
-        # make local metrics folder
-        if not os.path.exists(metrics_path):
-            Path(metrics_path).mkdir(parents=True)
-        print(f"Metrics will be exported to: {metrics_path}\n")
-        
-        input_stack = ee.Image(input_stack_path)
-        
-        if len(train_paths) > 1:
-            print(f'Merging training datasets together: {train_paths}\n')
-            # we must construct the ee.FeatureCollection's and merge them together
-            training_data = ee.FeatureCollection(train_paths[0])
-            for i in train_paths[1:]:
-                training_data = training_data.merge(i)
-        else:
-            training_data = ee.FeatureCollection(train_paths[0])
-        
-        # run primitives models
-        primitives_to_collection(input_stack=input_stack,
-                                 training_pts=training_data,
-                                 output_ic=img_coll_path,
-                                 metrics_path=metrics_path,
-                                 crs=crs)
-
-if __name__=="__main__":
+import ee
+import os
+from pathlib import Path
+import argparse
+from rlcms.utils import check_exists
+from rlcms.primitives import Primitives
+
+def main():
+    ee.Initialize()
+
+    parser = argparse.ArgumentParser(
+    description="Create Land Cover Primitives For All Classes in Provided Training Data",
+    usage = "primitives -i path/to/input_stack -t path/to/training_data -c LANDCOVER -o path/to/output --metrics_folder local/folder/path"
+    )
+    
+    parser.add_argument(
+        "-i",
+        "--input_stack",
+        type=str,
+        required=True,
+        help="full asset path to input stack"
+    )
+    
+    parser.add_argument(
+    "-t",
+    "--training_data",
+    type=str, 
+    nargs='+',
+    required=True,
+    help="full asset path(s) to training point dataset(s)"
+    )
+
+    parser.add_argument(
+    "-c",
+    "--class_name",
+    type=str, 
+    required=True,
+    help="model class label"
+    )
+    
+    parser.add_argument(
+        "-o",
+        "--output",
+        type=str,
+        required=True,
+        help="The output asset path of the primitives image collection."
+    )
+    
+    parser.add_argument(
+    "-crs",
+    type=str,
+    required=False,
+    help="CRS string in format of EPSG:xxxxx. Defaults to EPSG:4326"
+    )
+
+    parser.add_argument(
+    "-scale",
+    type=int,
+    required=False,
+    help="output scale"
+    )
+
+    parser.add_argument(
+        "--metrics_folder",
+        type=str,
+        required=False,
+        help="The local folder to export metrics files."
+    )
+    
+    parser.add_argument(
+        "-d",
+        "--dry_run",
+        dest="dry_run",
+        action="store_true",
+        help="goes through checks and prints paths to outputs but does not export them.",
+        )
+
+    args = parser.parse_args()
+
+    input_stack_path = args.input_stack
+    train_paths = args.training_data
+    class_name =args.class_name
+    output = args.output
+    crs = args.crs
+    scale = args.scale
+    metrics_path = args.metrics_folder
+    dry_run = args.dry_run
+
+    # Run Checks
+    # Check input stack exists
+    assert check_exists(input_stack_path) == 0, f"Check input_stack asset exists: {input_stack_path}"
+    
+    # Check training data exists
+    for train_path in train_paths:
+        assert check_exists(train_path) == 0, f"Check training_data asset exists: {train_path}"
+             
+    img_coll_path = output
+    output_folder = os.path.dirname(output)
+    # check output folder exists
+    assert check_exists(output_folder) == 0, f"Check parent folder exists: {output_folder}"
+    
+    # don't allow ee.Image exports to pre-existing ee.ImageCollections
+    if check_exists(img_coll_path) == 0:
+        raise AssertionError(f"Primitives ImageCollection already exists: {img_coll_path}")
+
+    # Construct local 'metrics' folder path from -o output or a default name if not provided
+    # cwd = os.getcwd()
+    # metrics_path = os.path.join(cwd,"metrics",os.path.basename(img_coll_path))
+
+    # print output locations and exit
+    if dry_run: 
+        print(f"Would Export Primitives ImageCollection to: {img_coll_path}\n")
+        print(f"Would Export Model Metrics to: {metrics_path}\n")
+        exit()
+    
+    else:
+        # make local metrics folder
+        if not os.path.exists(metrics_path):
+            Path(metrics_path).mkdir(parents=True)
+        print(f"Metrics will be exported to: {metrics_path}")
+        
+        input_stack = ee.Image(input_stack_path)
+        
+        if len(train_paths) > 1:
+            print(f'Merging training datasets together: {train_paths}\n')
+            # we must construct the ee.FeatureCollection's and merge them together
+            training_data = ee.FeatureCollection(train_paths[0])
+            for i in train_paths[1:]:
+                training_data = training_data.merge(i)
+        else:
+            training_data = ee.FeatureCollection(train_paths[0])
+        
+        # Construct Primitives
+        prims = Primitives(inputs=input_stack,
+                           training=training_data,
+                           class_name=class_name)
+        # Export as GEE ImgColl asset
+        prims.export_to_asset(collection_assetId=img_coll_path,
+                              crs=crs,
+                              scale=scale)
+        # Export model metrics
+        prims.export_metrics(metrics_path=metrics_path)
+
+if __name__=="__main__":
     main()
```

### Comparing `rlcms-2023.9.7/src/rlcms/cli/composite.py` & `rlcms-2024.5.29/src/rlcms/cli/composite.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,167 +1,165 @@
-import ee
-import os
-import re
-from rlcms.composites import composite
-from rlcms.utils import exportImgToAsset, check_exists
-import argparse
-import json
-
-def main():
-    ee.Initialize()
-    parser = argparse.ArgumentParser(
-    description="Create a Composite from one or multiple datasets",
-    usage = "composite -a aoi/fc/path -d Landsat8 -s 2020-01-01 -e 2020-12-31 -o output/path --settings path/to/settings/file.txt "
-    )
-    
-    parser.add_argument(
-    "-a",
-    "--aoi",
-    type=str,
-    required=True,
-    help="The asset path to an aoi or reference polygon dataset"
-    )
-    
-    parser.add_argument(
-    "-d",
-    "--data",
-    type=str, 
-    nargs='+',
-    required=True,
-    help="Dataset(s) to composite"
-    )
-    
-    parser.add_argument(
-    "-s",
-    "--start",
-    type=str,
-    required=True,
-    help="start date (yyyy-mm-dd)"
-    )
-
-    parser.add_argument(
-    "-e",
-    "--end",
-    type=str,
-    required=True,
-    help="end date (yyyy-mm-dd)"
-    )
-
-    parser.add_argument(
-    "-o",
-    "--output",
-    type=str,
-    required=True,
-    help="The full asset path for export"
-    )
-
-    parser.add_argument(
-    "--settings",
-    type=str,
-    required=True,
-    help="settings .txt file"
-    )
-    
-    parser.add_argument(
-    "--scale",
-    type=int,
-    required=True,
-    help="Scale of output composite."
-    )
-    
-    parser.add_argument(
-    "--crs",
-    type=str,
-    required=False,
-    help="CRS string in format of EPSG:xxxxx. Defaults to EPSG:4326"
-    )
-    
-    parser.add_argument(
-    "--dry_run",
-    dest="dry_run",
-    action="store_true",
-    help="goes through checks and prints output asset path but does not export",
-    )
-    
-    args = parser.parse_args()
-    
-    aoi_path = args.aoi
-    data = args.data
-    start = args.start
-    end = args.end
-    output = args.output
-    scale = args.scale
-    crs = args.crs
-    settings_f = args.settings
-    dry_run = args.dry_run
-    
-    output_folder = os.path.dirname(output)
-   
-    # parse txt file into settings dict that we'll pass to composite()
-    with open(settings_f) as f:
-        settings = json.load(f)
-    
-    # check output doesn't already exist (GEE by default prohibits overwrites)
-    assert check_exists(output), f"Image already exsits: {output}"
-    # check inputs exist
-    assert check_exists(aoi_path) == 0, f"Check aoi exists: {aoi_path}"
-    assert check_exists(output_folder) == 0, f"Check output folder exists: {output_folder}"
-    # ensure start and end dates will work
-    for date in [start,end]:
-        r = re.compile('.{4}-.{2}-.{2}')
-        if len(date) == 10:
-            if r.match(date):
-                pass
-            else:
-                raise ValueError(f"date string(s) don't match required format. Got: {date}")
-        else:
-            raise ValueError(f"date string(s) don't match required format. Got: {date}")
-    
-    aoi = ee.FeatureCollection(aoi_path)
-    
-    # multiple datasets requested, combining multiple composites
-    if len(data) > 1: 
-        composite_list = ([composite(dataset=d,
-                        region=aoi,
-                        start_date=start,
-                        end_date=end,
-                        **settings)
-                        # prefix dataset name to every band, if data is an asset path we swap / for _
-                        .regexpRename('^', f"{d.replace('/','_')}_") 
-                            for d in data])
-        
-        img = ee.Image.cat(composite_list)
-    
-    # only one dataset requested
-    else:
-        img = composite(dataset=data[0],
-                        region=aoi,
-                        start_date=start,
-                        end_date=end,
-                        **settings)
-    
-    print(img.bandNames().getInfo())
-    
-    if dry_run:
-        print(f"would export: {output}")
-    
-    else:
-        if crs == None:
-            task = ee.batch.Export.image.toAsset(image=img,
-                                        description=os.path.basename(output),
-                                        assetId=output,
-                                        region=aoi.geometry(),
-                                        scale=scale,
-                                        maxPixels=1e12)
-        else:
-            task = ee.batch.Export.image.toAsset(image=img,
-                                        description=os.path.basename(output),
-                                        assetId=output,
-                                        region=aoi.geometry(),
-                                        scale=scale,
-                                        maxPixels=1e12,
-                                        crs=crs)
-        task.start()
-        print(f"Export started (Asset): {output}") 
-
-if __name__ == "__main__":
+import ee
+import os
+import re
+from rlcms.composites import Composite
+from rlcms.utils import check_exists
+import argparse
+import json
+
+def main():
+    ee.Initialize()
+    parser = argparse.ArgumentParser(
+    description="Create a Composite from one or multiple datasets",
+    usage = "composite -a aoi/fc/path -d Landsat8 -s 2020-01-01 -e 2020-12-31 -o output/path --settings path/to/settings/file.txt "
+    )
+    
+    parser.add_argument(
+    "-a",
+    "--aoi",
+    type=str,
+    required=True,
+    help="The asset path to an aoi or reference polygon dataset"
+    )
+    
+    parser.add_argument(
+    "-d",
+    "--data",
+    type=str, 
+    nargs='+',
+    required=True,
+    help="Dataset(s) to composite"
+    )
+    
+    parser.add_argument(
+    "-s",
+    "--start",
+    type=str,
+    required=True,
+    help="start date (yyyy-mm-dd)"
+    )
+
+    parser.add_argument(
+    "-e",
+    "--end",
+    type=str,
+    required=True,
+    help="end date (yyyy-mm-dd)"
+    )
+
+    parser.add_argument(
+    "-o",
+    "--output",
+    type=str,
+    required=True,
+    help="The full asset path for export"
+    )
+
+    parser.add_argument(
+    "--settings",
+    type=str,
+    required=True,
+    help="settings .txt file"
+    )
+    
+    parser.add_argument(
+    "--scale",
+    type=int,
+    required=True,
+    help="Scale of output composite."
+    )
+    
+    parser.add_argument(
+    "--crs",
+    type=str,
+    required=False,
+    help="CRS string in format of EPSG:xxxxx. Defaults to EPSG:4326"
+    )
+    
+    parser.add_argument(
+    "--dry_run",
+    dest="dry_run",
+    action="store_true",
+    help="goes through checks and prints output asset path but does not export",
+    )
+    
+    args = parser.parse_args()
+    
+    aoi_path = args.aoi
+    data = args.data
+    start = args.start
+    end = args.end
+    output = args.output
+    scale = args.scale
+    crs = args.crs
+    settings_f = args.settings
+    dry_run = args.dry_run
+    
+    output_folder = os.path.dirname(output)
+   
+    # parse txt file into settings dict that we'll pass to composite()
+    with open(settings_f) as f:
+        settings = json.load(f)
+    
+    # check output doesn't already exist (GEE by default prohibits overwrites)
+    assert check_exists(output), f"Image already exsits: {output}"
+    # check inputs exist
+    assert check_exists(aoi_path) == 0, f"Check aoi exists: {aoi_path}"
+    assert check_exists(output_folder) == 0, f"Check output folder exists: {output_folder}"
+    # ensure start and end dates will work
+    for date in [start,end]:
+        r = re.compile('.{4}-.{2}-.{2}')
+        if len(date) == 10:
+            if r.match(date):
+                pass
+            else:
+                raise ValueError(f"date string(s) don't match required format. Got: {date}")
+        else:
+            raise ValueError(f"date string(s) don't match required format. Got: {date}")
+    
+    aoi = ee.FeatureCollection(aoi_path)
+    
+    # multiple datasets requested, combining multiple composites
+    if len(data) > 1: 
+        composite_list = ([Composite(dataset=d,
+                        region=aoi,
+                        start_date=start,
+                        end_date=end,
+                        **settings)
+                        # prefix dataset name to every band, if data is an asset path we swap / for _
+                        .regexpRename('^', f"{d.replace('/','_')}_") 
+                            for d in data])
+        
+        img = ee.Image.cat(composite_list)
+    
+    # only one dataset requested
+    else:
+        img = Composite(dataset=data[0],
+                        region=aoi,
+                        start_date=start,
+                        end_date=end,
+                        **settings)
+    
+    if dry_run:
+        print(f"would export: {output}")
+    
+    else:
+        if crs == None:
+            task = ee.batch.Export.image.toAsset(image=img.image,
+                                        description=os.path.basename(output),
+                                        assetId=output,
+                                        region=aoi.geometry(),
+                                        scale=scale,
+                                        maxPixels=1e12)
+        else:
+            task = ee.batch.Export.image.toAsset(image=img.image,
+                                        description=os.path.basename(output),
+                                        assetId=output,
+                                        region=aoi.geometry(),
+                                        scale=scale,
+                                        maxPixels=1e12,
+                                        crs=crs)
+        task.start()
+        print(f"Export started (Asset): {output}") 
+
+if __name__ == "__main__":
     main()
```

### Comparing `rlcms-2023.9.7/src/rlcms/cli/sample_pts.py` & `rlcms-2024.5.29/src/rlcms/cli/sample_pts.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,211 +1,201 @@
-#%%
-import os
-import ee
-import argparse
-import numpy as np
-import rlcms.sampling as sampling
-from rlcms.utils import check_exists, exportTableToAsset, exportTableToDrive
-
-## GLOBAL VARS
-scale = 10 # for Sentinel2
-
-def ceoClean(f):
-        # LON,LAT,PLOTID,SAMPLEID.,
-        fid = f.id()
-        coords = f.geometry().coordinates()
-        return f.set('LON',coords.get(0),
-                    'LAT',coords.get(1),
-                    'PLOTID',fid,
-                    'SAMPLEID',fid)
-
-def plot_id_global(n,feat):
-    """takes an index number (n) and adds it to current PLOTID property of a feature 
-            to ensure PLOTID values are globally unique (necessary for multiple sets of AOI sampling)"""
-    aoi_id = ee.String(str(n))
-    f = ee.Feature(feat)
-    gid = aoi_id.cat('_').cat(ee.String(f.get('PLOTID')))
-    f = f.set('PLOTID',gid, 'SAMPLEID', gid)
-    return f
-
-def main():
-    ee.Initialize()
-
-    parser = argparse.ArgumentParser(
-    description="Generate Random Sample Points From an ee.Image, Formatted for Collect Earth Online",
-    usage = "sample_pts -im input/path/to/image -band LANDCOVER -o output/path --n_points 100 --to_drive"
-    )
-    
-    parser.add_argument(
-    "-im",
-    "--input_image",
-    type=str,
-    required=True,
-    help="asset path to image you are sampling from"
-    )
-    
-    # added this required arg for greater flexibility. default behavior of .stratifiedSample() is to use image's first band
-    # most LC images will only have one band but in case the img doesn't this ensures correct behavior..
-    parser.add_argument(
-    "-band",
-    "--class_band",
-    type=str,
-    required=True,
-    help="class band name to use for stratification"
-    )
-
-    parser.add_argument(
-    "-o",
-    "--output",
-    type=str,
-    required=True,
-    help="The output asset path basename for export."
-    )
-    
-    parser.add_argument(
-    "--n_points",
-    type=int,
-    required=False,
-    help="Number of points per class. Default: 100"
-    )
-
-    parser.add_argument(
-    '--class_values', 
-    type=int, 
-    nargs='+',
-    required=False,
-    help="list of unique LANDCOVER values in input Feature Collection"
-    )
-
-    parser.add_argument(
-    "--class_points",
-    type=int,
-    nargs='+',
-    required=False,
-    help="number of samples to collect per class"
-    )
-    
-    parser.add_argument(
-    "-ta",
-    "--to_asset",
-    dest="to_asset",
-    action="store_true",
-    help="exports to GEE Asset only",
-    )
-    
-    parser.add_argument(
-    "-td",
-    "--to_drive",
-    dest="to_drive",
-    action="store_true",
-    help="exports to Google Drive only",
-    )
-    
-    parser.add_argument(
-    "-r",
-    "--reshuffle",
-    dest="reshuffle",
-    action="store_true",
-    help="randomizes seed used in all functions",
-    )
-
-    parser.add_argument(
-    "-d",
-    "--dry_run",
-    dest="dry_run",
-    action="store_true",
-    help="goes through checks and prints output asset path but does not export.",
-    )
-
-    args = parser.parse_args()
-    
-    input_path = args.input_image
-    class_band = args.class_band
-    output = args.output
-    n_points = args.n_points
-    class_values = args.class_values
-    class_points = args.class_points
-    to_asset = args.to_asset
-    to_drive = args.to_drive
-    reshuffle = args.reshuffle
-    dry_run = args.dry_run
-
-    # perform checks
-    output_folder = os.path.dirname(output)
-    assert check_exists(input_path) == 0, f"Check input FeatureCollection exists: {input_path}"
-    assert check_exists(output_folder) == 0, f"Check output folder exists: {output_folder}"
-    
-    # value checks if class_values and class_points args are both provided
-    if ((class_values != None) and (class_points != None)):
-        
-        # class_values and class_points must be equal length
-        if len(class_values) != len(class_points):
-            print(f"Error: class_points and class_values are of unequal length: {class_values} {class_points}")
-            exit()
-        # class_values and class_points provided so we'll override n_points, 
-        # but ee.Image.stratifiedSample() still requires it so we set to default
-        n_points=100
-    
-    # if only one is provided, error 
-    elif (class_values != None and class_points == None) or (class_values == None and class_points != None):
-        print(f"Error: class_values and class_points args are codependent, provide both or neither. class_values:{class_values}, class_points:{class_points}")
-    
-    # if neither class_values nor class_points provided, n_points must be provided, otherwise we set a default n_points value 
-    else:
-        if n_points != None:
-            pass
-        else:
-            n_points=100
-            print(f"Warning: Defaulting to equal allocation of default n: {n_points}. Set n_points or class_values and class_points to control sample allocation.")
-            
-    
-    img = ee.Image(input_path)
-    bbox = img.geometry().bounds() # region
-    # default seed is set, will re-randomize seed if reshuffle==True
-    seed=90210
-    if reshuffle:
-        np.random.RandomState()
-        seed = np.random.randint(low=1,high=1e6)
-        print(f"reshuffled new seed: {seed}")
-    
-    
-    samples = sampling.strat_sample(img=img,
-                                    class_band=class_band,
-                                    region=bbox,
-                                    scale=scale, # 10, hard coded set at top of script, can make this a user arg for greater flexibility
-                                    seed=seed, 
-                                    n_points=n_points,
-                                    class_values=class_values,
-                                    class_points=class_points).map(ceoClean)
-
-    # set up export info
-    description = os.path.basename(output)
-    drive_folder = 'kaza-lc'
-    drive_desc = description+'-Drive'
-    asset_desc = description+'-Asset'
-    selectors = 'LON,LAT,PLOTID,SAMPLEID,'+class_band
-    # will export to drive or asset if you specify one or the other
-    if to_asset==True and to_drive==False:
-        if dry_run:
-            print(f"would export (Asset): {output}")
-            exit()
-        else:
-            exportTableToAsset(samples,asset_desc,output)
-    
-    elif to_drive==True and to_asset==False:
-        if dry_run:
-            print(f"would export (Drive): {drive_folder}/{drive_desc}")
-            exit()
-        else:
-            exportTableToDrive(samples,drive_desc,drive_folder,selectors)
-    
-    else: # export both ways if neither or both of the --to_drive and --to_asset flags are given
-        if dry_run:
-            print(f"would export (Asset): {output}")
-            print(f"would export (Drive): {drive_folder}/{drive_desc}")
-            exit()
-        else:
-            exportTableToAsset(samples,asset_desc,output)
-            exportTableToDrive(samples,drive_desc,drive_folder,selectors)
-        
-if __name__ == "__main__":
-    main()
+#%%
+import os
+import ee
+import argparse
+import numpy as np
+import rlcms.sampling as sampling
+from rlcms.utils import check_exists, exportTableToAsset, exportTableToDrive
+
+def main():
+    ee.Initialize()
+
+    parser = argparse.ArgumentParser(
+    description="Generate Random Sample Points From an ee.Image, Formatted for Collect Earth Online",
+    usage = "sample_pts -im input/path/to/image -band LANDCOVER -o output/path --n_points 100 --to_drive"
+    )
+    
+    parser.add_argument(
+    "-im",
+    "--input_image",
+    type=str,
+    required=True,
+    help="asset path to image you are sampling from"
+    )
+    
+    # added this required arg for greater flexibility. default behavior of .stratifiedSample() is to use image's first band
+    # most LC images will only have one band but in case the img doesn't this ensures correct behavior..
+    parser.add_argument(
+    "-band",
+    "--class_band",
+    type=str,
+    required=True,
+    help="class band name to use for stratification"
+    )
+
+    parser.add_argument(
+        "-s",
+        "--scale",
+        type=int,
+        required=True,
+        help="scale to conduct sampling (meters)"
+        )
+    
+    parser.add_argument(
+    "-oa",
+    "--output_asset",
+    type=str,
+    required=False,
+    help="The output GEE asset path for export."
+    )
+    
+    parser.add_argument(
+    "-od",
+    "--output_drive",
+    type=str,
+    required=False,
+    help="The output google drive path for export."
+    )
+    parser.add_argument(
+    "--n_points",
+    type=int,
+    required=False,
+    help="Number of points per class. Default: 100"
+    )
+
+    parser.add_argument(
+    '--class_values', 
+    type=int, 
+    nargs='+',
+    required=False,
+    help="list of unique LANDCOVER values in input Feature Collection"
+    )
+
+    parser.add_argument(
+    "--class_points",
+    type=int,
+    nargs='+',
+    required=False,
+    help="number of samples to collect per class"
+    )
+    
+    parser.add_argument(
+    "-r",
+    "--reshuffle",
+    dest="reshuffle",
+    action="store_true",
+    help="randomizes seed used in all functions",
+    )
+
+    parser.add_argument(
+    "-d",
+    "--dry_run",
+    dest="dry_run",
+    action="store_true",
+    help="goes through checks and prints output asset path but does not export.",
+    )
+
+    args = parser.parse_args()
+    
+    input_path = args.input_image
+    class_band = args.class_band
+    scale = args.scale
+    output_asset = args.output_asset
+    output_drive = args.output_drive
+    n_points = args.n_points
+    class_values = args.class_values
+    class_points = args.class_points
+    reshuffle = args.reshuffle
+    dry_run = args.dry_run
+
+    # perform checks
+    assert check_exists(input_path) == 0, f"Check input FeatureCollection exists: {input_path}"
+    # GEE won't make parents for you
+    if output_asset:
+        output_asset_folder = os.path.dirname(output_asset)
+        assert check_exists(output_asset_folder) == 0, f"Check GEE output asset's folder exists: {output_asset_folder}"
+    
+    # value checks if class_values and class_points args are both provided
+    if ((class_values != None) and (class_points != None)):
+        
+        # class_values and class_points must be equal length
+        if len(class_values) != len(class_points):
+            print(f"Error: class_points and class_values are of unequal length: {class_values} {class_points}")
+            exit()
+        # class_values and class_points provided so we'll override n_points, 
+        # but ee.Image.stratifiedSample() still requires it so we set to default
+        n_points=100
+    
+    # if only one is provided, error 
+    elif (class_values != None and class_points == None) or (class_values == None and class_points != None):
+        print(f"Error: class_values and class_points args are codependent, provide both or neither. class_values:{class_values}, class_points:{class_points}")
+    
+    # if neither class_values nor class_points provided, n_points must be provided, otherwise we set a default n_points value 
+    else:
+        if n_points != None:
+            pass
+        else:
+            n_points=100
+            print(f"Warning: Defaulting to equal allocation of default n: {n_points}. Set n_points or class_values and class_points to control sample allocation.")
+            
+    
+    img = ee.Image(input_path)
+    bbox = img.geometry().bounds() # region
+    # default seed is set, will re-randomize seed if reshuffle==True
+    seed=90210
+    if reshuffle:
+        np.random.RandomState()
+        seed = np.random.randint(low=1,high=1e6)
+        print(f"reshuffled new seed: {seed}")
+    
+    
+    samples = sampling.strat_sample(img=img,
+                                    class_band=class_band,
+                                    region=bbox,
+                                    scale=scale, # 10, hard coded set at top of script, can make this a user arg for greater flexibility
+                                    seed=seed, 
+                                    n_points=n_points,
+                                    class_values=class_values,
+                                    class_points=class_points)
+
+   
+    selectors = 'LON,LAT,PLOTID,SAMPLEID,'+class_band
+    
+    # to GEE Asset only
+    if output_asset!=None and output_drive==None:
+        desc = os.path.basename(output_asset)+'-Asset'
+        if dry_run:
+            print(f"would export (Asset): {output_asset}")
+            exit()
+        else:
+            exportTableToAsset(samples,desc,output_asset)
+    
+    # to Google Drive only
+    elif output_asset==None and output_drive!=None:
+        # user might not provide a GEE asset conforming path as output if toAsset not their intent
+        drive_folder = os.path.dirname(output_drive)
+        drive_basename = os.path.basename(output_drive)
+        drive_desc = drive_basename+'-Drive'
+        if dry_run:
+            print(f"would export (Drive): {output_drive}")
+            exit()
+        else:
+            exportTableToDrive(samples,drive_desc,drive_folder,drive_basename,selectors)
+    
+    # export both to GEE Asset and Google Drive
+    elif output_asset!=None and output_drive!=None: 
+        asset_desc = os.path.basename(output_asset)+'-Asset'
+        drive_folder = os.path.dirname(output_drive)
+        drive_basename = os.path.basename(output_drive)
+        drive_desc = drive_basename+'-Drive'
+        if dry_run:
+            print(f"would export (Asset): {output_asset}")
+            print(f"would export (Drive): {output_drive}")
+            exit()
+        else:
+            exportTableToAsset(samples,asset_desc,output_asset)
+            exportTableToDrive(samples,drive_desc,drive_folder,drive_basename,selectors)
+    # neither output paths specified
+    else:
+        raise RuntimeError(f"No output paths provided, user must provide at least one of the following two arguments:\n -oa/--output_asset  -od/--output_drive")        
+if __name__ == "__main__":
+    main()
```

### Comparing `rlcms-2023.9.7/src/rlcms/cli/train_test.py` & `rlcms-2024.5.29/src/rlcms/cli/train_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,161 +1,179 @@
-import argparse
-import os
-from rlcms.utils import check_exists, exportTableToAsset
-from rlcms.sampling import strat_sample_w_extraction, split_train_test
-import ee
-import numpy as np
-ee.Initialize()
-
-def main():
-    parser = argparse.ArgumentParser(
-    description="Extract Train and Test Point Data from an Input Image within Reference Polygon Areas",
-    usage = """train_test -rp path/to/reference_polygon_fc -im path/to/input/stack 
-                -o unique/output/path --class_values 1 2 3 4 5 6 7 8 --class_points 10 10 10 10 10 10 10"""
-    )
-    
-    parser.add_argument(
-    "-rp",
-    "--reference_polygons",
-    type=str,
-    required=True,
-    help="The full asset path to the reference polygon ee.FeatureCollection"
-    )
-    
-    parser.add_argument(
-    "-im",
-    "--input_img",
-    type=str,
-    required=True,
-    help="The full asset path to the input stack ee.Image"
-    )
-
-    parser.add_argument(
-    "-c",
-    "--crs",
-    type=str,
-    required=False,
-    help="CRS string in format of EPSG:xxxxx. Defaults to EPSG:4326"
-    )
-    
-    parser.add_argument(
-    "-o",
-    "--output",
-    type=str,
-    required=True,
-    help="The output asset path basename for export"
-    )
-    
-    parser.add_argument(
-    '--class_values', 
-    type=int, 
-    nargs='+',
-    required=True,
-    help="list of unique LANDCOVER values in input Feature Collection"
-    )
-
-    parser.add_argument(
-    "--class_points",
-    type=int,
-    nargs='+',
-    required=True,
-    help="number of samples to collect per class"
-    )
-    
-    parser.add_argument(
-    "-ns",
-    "--no_split",
-    dest="no_split",
-    action="store_true",
-    help="don't split extracted points into train and test",
-    )
-    
-    parser.add_argument(
-    "-r",
-    "--reshuffle",
-    dest="reshuffle",
-    action="store_true",
-    help="randomizes seed used in all functions",
-    )
-
-    parser.add_argument(
-    "-d",
-    "--dry_run",
-    dest="dry_run",
-    action="store_true",
-    help="goes through checks and prints output asset path but does not export",
-    )
-    
-    args = parser.parse_args()
-    
-    input_fc = args.reference_polygons
-    input_img = args.input_img
-    output = args.output
-    crs = args.crs
-    class_values = args.class_values
-    class_points = args.class_points
-    dry_run = args.dry_run
-    no_split = args.no_split
-    reshuffle = args.reshuffle
-
-    # perform checks
-    output_folder = os.path.dirname(output)
-    
-    assert check_exists(input_fc) == 0, f"Check input FeatureCollection exists: {input_fc}"
-    assert check_exists(output_folder) == 0, f"Check output folder exists: {output_folder}"
-    assert check_exists(input_img) == 0, f"Check input image exists: {input_img}"
-
-    # class_values and class_points must be equal length
-    if len(class_values) != len(class_points):
-        raise ValueError(f"Error: class_points and class_values are of unequal length: {class_values} {class_points}")
-        
-    # user may not want to sample all classes, but provide warning to catch user error
-    class_values_actual = ee.FeatureCollection(input_fc).aggregate_array('LANDCOVER').distinct().sort().getInfo()
-    if class_values_actual != class_values:
-        print(f"Warning: All classes in the reference dataset will not be sampled with class_values provided by user (EE-Reported class_values:{class_values_actual}). Processing will continue.")
-
-    if dry_run:
-        if no_split:
-            print(f"would export (Asset): {output}")
-            exit()
-        else:
-            print(f"would export (Asset): {output}_[train|test]_pts")
-            exit()
-    else:
-        # default seed is set, will re-randomize seed if reshuffle==True
-        seed=90210
-        if reshuffle:
-            np.random.RandomState()
-            seed = np.random.randint(low=1,high=1e6)
-            print(f"reshuffled new seed: {seed}")
-        
-        image = ee.Image(input_img)
-        fc = ee.FeatureCollection(input_fc)
-        pts = strat_sample_w_extraction(img=image,
-                                         collection=fc,
-                                         class_band='LANDCOVER', # should this be a CLI arg or set in model_inputs.py? hardcoded for now..
-                                         scale=10, # should this be a CLI arg or set in model_inputs.py? hardcoded for now..
-                                         crs=crs, # this is now a CLI arg
-                                         seed=seed,
-                                         class_values=class_values,
-                                         class_points=class_points)
-        
-        if no_split==False: # split into train and test pts
-            train,test = split_train_test(pts,seed)
-            train_assetid = f"{output}_train_pts"
-            train_description = os.path.basename(train_assetid).replace('/','_')
-            exportTableToAsset(train,train_description,train_assetid)
-
-            test_assetid = f"{output}_test_pts"
-            test_description = os.path.basename(test_assetid).replace('/','_')
-            exportTableToAsset(test,test_description,test_assetid)
-        
-        else: # export all pts as is
-            assetid = f"{output}"
-            description = os.path.basename(assetid).replace('/','_')
-            exportTableToAsset(pts,description,assetid)
-        
-if __name__ == "__main__":
-    main()
-
-
-
+import argparse
+import os
+from rlcms.utils import check_exists, exportTableToAsset
+from rlcms.sampling import strat_sample_w_extraction, strat_sample_from_reference, split_train_test
+import ee
+import numpy as np
+ee.Initialize()
+
+def main():
+    parser = argparse.ArgumentParser(
+    description="Extract Train and Test Point Data from an Input Image within Reference Data Locations",
+    usage = """train_test -ref path/to/reference_fc -im path/to/input/stack -band LANDCOVER --scale 10
+                -o unique/output/path --class_values 1 2 3 4 5 6 7 8 --class_points 10 10 10 10 10 10 10"""
+    )
+    
+    parser.add_argument(
+    "-ref",
+    "--reference_data",
+    type=str,
+    required=True,
+    help="The full GEE asset path to the reference data"
+    )
+    
+    parser.add_argument(
+    "-im",
+    "--input_img",
+    type=str,
+    required=True,
+    help="The full asset path to the input stack ee.Image"
+    )
+
+    parser.add_argument(
+    "-band",
+    "--class_band",
+    type=str,
+    required=True,
+    help="class band name to use for stratification"
+        )
+    
+    parser.add_argument(
+    "-s",
+    "--scale",
+    type=int,
+    required=True,
+    help="scale to conduct sampling (meters)"
+    )
+    
+    parser.add_argument(
+    "-c",
+    "--crs",
+    type=str,
+    required=False,
+    help="CRS string in format of EPSG:xxxxx. Defaults to EPSG:4326"
+    )
+    
+    parser.add_argument(
+    "-o",
+    "--output",
+    type=str,
+    required=True,
+    help="The output asset path basename for export"
+    )
+    
+    parser.add_argument(
+    '--class_values', 
+    type=int, 
+    nargs='+',
+    required=True,
+    help="list of unique LANDCOVER values in input Feature Collection"
+    )
+
+    parser.add_argument(
+    "--class_points",
+    type=int,
+    nargs='+',
+    required=True,
+    help="number of samples to collect per class"
+    )
+    
+    parser.add_argument(
+    "-ns",
+    "--no_split",
+    dest="no_split",
+    action="store_true",
+    help="don't split extracted points into train and test",
+    )
+    
+    parser.add_argument(
+    "-r",
+    "--reshuffle",
+    dest="reshuffle",
+    action="store_true",
+    help="randomizes seed used in all functions",
+    )
+
+    parser.add_argument(
+    "-d",
+    "--dry_run",
+    dest="dry_run",
+    action="store_true",
+    help="goes through checks and prints output asset path but does not export",
+    )
+    
+    args = parser.parse_args()
+    
+    input_fc = args.reference_data
+    input_img = args.input_img
+    class_band = args.class_band
+    output = args.output
+    scale = args.scale
+    crs = args.crs
+    class_values = args.class_values
+    class_points = args.class_points
+    dry_run = args.dry_run
+    no_split = args.no_split
+    reshuffle = args.reshuffle
+
+    # perform checks
+    output_folder = os.path.dirname(output)
+    
+    assert check_exists(input_fc) == 0, f"Check input FeatureCollection exists: {input_fc}"
+    assert check_exists(output_folder) == 0, f"Check output folder exists: {output_folder}"
+    assert check_exists(input_img) == 0, f"Check input image exists: {input_img}"
+
+    # class_values and class_points must be equal length
+    if len(class_values) != len(class_points):
+        raise ValueError(f"Error: class_points and class_values are of unequal length: {class_values} {class_points}")
+        
+    # user may not want to sample all classes, but provide warning to catch user error
+    class_values_actual = ee.FeatureCollection(input_fc).aggregate_array('LANDCOVER').distinct().sort().getInfo()
+    if class_values_actual != class_values:
+        print(f"Warning: All classes in the reference dataset will not be sampled with class_values provided by user (EE-Reported class_values:{class_values_actual}). Processing will continue.")
+
+    if dry_run:
+        if no_split:
+            print(f"would export (Asset): {output}")
+            exit()
+        else:
+            print(f"would export (Asset): {output}_[train|test]_pts")
+            exit()
+    else:
+        # default seed is set, will re-randomize seed if reshuffle==True
+        seed=90210
+        if reshuffle:
+            np.random.RandomState()
+            seed = np.random.randint(low=1,high=1e6)
+            print(f"reshuffled new seed: {seed}")
+        
+        image = ee.Image(input_img)
+        fc = ee.FeatureCollection(input_fc)
+        pts = strat_sample_from_reference(img=image,
+                                         collection=fc,
+                                         class_band=class_band, 
+                                         scale=scale, 
+                                         crs=crs, 
+                                         seed=seed,
+                                         class_values=class_values,
+                                         class_points=class_points)
+        
+        if no_split==False: # split into train and test pts
+            train,test = split_train_test(pts,seed)
+            train_assetid = f"{output}_train_pts"
+            train_description = os.path.basename(train_assetid).replace('/','_')
+            exportTableToAsset(train,train_description,train_assetid)
+
+            test_assetid = f"{output}_test_pts"
+            test_description = os.path.basename(test_assetid).replace('/','_')
+            exportTableToAsset(test,test_description,test_assetid)
+        
+        else: # export all pts as is
+            assetid = f"{output}"
+            description = os.path.basename(assetid).replace('/','_')
+            exportTableToAsset(pts,description,assetid)
+        
+if __name__ == "__main__":
+    main()
+
+
+
```

### Comparing `rlcms-2023.9.7/src/rlcms/composites.py` & `rlcms-2024.5.29/src/rlcms/composites.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,216 +1,206 @@
-import ee
-import hydrafloods as hf
-from rlcms.harmonics import doHarmonicsFromOptions
-from rlcms.covariates import indices
-from rlcms.covariates import returnCovariatesFromOptions
-from ee.ee_exception import EEException
-
-ee.Initialize()
-
-idx = indices()
-
-def get_agg_timing(collection:hf.Dataset,**kwargs):
-    """utility function for hf.Dataset.aggregate_time(). Formats `period`, `period_unit`, and `dates` args
-        to create certain types of composites (defined by `composite_mode`)
-    args:
-        collection (hf.Dataset): Hydrafloods Dataset
-    kwargs:
-        composite_mode (str): one of 'annual' or 'seasonal', Default = 'annual'
-        season (list[str|int]): consecutive list of months (e.g. ['01','02','03']) comprising the season.
-            A required arg if composite_mode == 'seasonal'
-    Returns:
-        tuple(period(int),period_unit(str),dates(list[str]))
-            
-    """
-    if 'composite_mode' not in kwargs:
-        composite_mode = 'annual'
-    else:
-        composite_mode = kwargs['composite_mode']
-    
-    # get unique yyyy strings
-    years = list(set([d.split(' ')[0].split('-')[0] for d in collection.dates])) 
-    years.sort()
-    
-    if composite_mode == 'seasonal':
-        if 'season' not in kwargs:
-            raise ValueError("season arg required if composite_mode == 'seasonal'")
-        else:
-            season = kwargs['season'] # must be consecutive 
-            period = len(season)
-            period_unit = 'month'
-            dates = [f"{y}-{str(season[0])}-01" for y in years]
-    elif composite_mode == 'annual':
-        period = 1
-        period_unit = 'year'
-        dates = [y+'-01-01' for y in years]
-    
-    else:
-        raise ValueError(f"{composite_mode} not a valid 'composite_mode'. Choose one of 'annual' or 'seasonal'")
-    
-    return period,period_unit,dates
-
-class composite:
-    """Initializes Composite class
-    
-        Processes multi-band composite of your chosen dataset(s) within an AOI footprint polygon
-
-        args:
-            dataset (str): one of: 'Landsat5','Landsat7','Landsat8','Sentinel1Asc','Sentinel1Desc','Sentinel2','Modis','Viirs')
-            region (ee.FeatureCollection): area of interest
-            start_date (str): start date
-            end_date (str): end date
-        
-        kwargs:
-            indices:list[str]
-            composite_mode:str One of ['seasonal','annual'] Default = 'annual' 
-            season:list[str|int]
-            reducer:str|ee.Reducer
-            addTasselCap:bool
-            addTopography:bool
-            addJRC:bool
-            harmonicsOptions:dict in this format: {'nir':{'start':int[1:365],'end':[1:365]}}
-        
-        returns:
-            ee.Image: multi-band image composite within region
-        """
-    
-    def __init__(self,dataset:str,
-                    region:ee.FeatureCollection,
-                    start_date:str,
-                    end_date:str,
-                    **kwargs):
-    
-        self.dataset=dataset
-        if isinstance(region, ee.Geometry):
-            self.region=region.getInfo()['coordinates']
-        elif isinstance(region, ee.FeatureCollection):
-            self.region = region.geometry().getInfo()['coordinates']
-        self.start_date=start_date
-        self.end_date=end_date
-        
-        for key, value in kwargs.items():
-            setattr(self, key, value)
-        
-        # testing whether need to go b/w FC and Geometry for multi_poly
-        if isinstance(region,ee.FeatureCollection):
-            region = region.geometry()
-            region_fc = region
-        elif isinstance(region,ee.Geometry):
-            region = region
-        else:
-            raise TypeError(f"{region} must be of type ee.FeatureCollection or ee.Geometry, got {type(region)}")
-        # all hydrafloods.Dataset sub-classes
-        ds_dict = {'Landsat5':hf.Landsat5(region,start_date,end_date),
-                'Landsat7':hf.Landsat7(region,start_date,end_date),
-                'Landsat8':hf.Landsat8(region,start_date,end_date),
-                'Sentinel1':hf.Sentinel1(region,start_date,end_date),
-                'Sentinel1Asc':hf.Sentinel1Asc(region,start_date,end_date),
-                'Sentinel1Desc':hf.Sentinel1Desc(region,start_date,end_date),
-                'Sentinel2':hf.Sentinel2(region,start_date,end_date),
-                'MODIS':hf.Modis(region,start_date,end_date),
-                'VIIRS':hf.Viirs(region,start_date,end_date)}
-        
-        # dataset can either be a named dataset string supported by a hf.Dataset sub-class 
-        # or a GEE Asset path
-        if isinstance(dataset,str):
-            if dataset in ds_dict.keys(): 
-                ds = ds_dict[dataset]
-            else:
-                if '/' in dataset: 
-                    try:
-                        ds = hf.Dataset(asset_id=dataset,region=region,start_time=start_date,end_time=end_date)
-                    except:
-                        raise EEException
-                else: 
-                    raise ValueError(f"Could not construct a hf.Dataset from dataset name provided: {dataset}")
-        else:
-            raise TypeError(f"dataset must be str type, got: {type(dataset)}")
-        
-        # mask imgs to geometries in multi_poly mode
-        if 'multi_poly' in kwargs:
-            if kwargs['multi_poly'] == True:
-                def update_mask(img):
-                    ref_poly_img = ee.Image(1).paint(region_fc).Not().selfMask() # aoi can be ee.Geometry or ee.FeatureCollection for this
-                    return ee.Image(img).updateMask(ref_poly_img)
-                # do we want to warn user against using multi_poly unnecessarily if aoi is a single geometry?
-                # would require another synchronous request of aoi's type/element size
-                ds = ds.apply_func(update_mask)
-        
-        ds = ds.apply_func(returnCovariatesFromOptions,**kwargs)
-        
-        # set reducer passed to aggregate_time(), default mean
-        if 'reducer' in kwargs:
-            reducer=kwargs['reducer']
-        else:
-            reducer = 'mean'
-        
-        period,period_unit,dates = get_agg_timing(ds,**kwargs)
-        
-        # aggregate hf.Dataset
-        agg_time_result = (ds.aggregate_time(reducer=reducer,
-                                        rename=False,
-                                        period_unit=period_unit,
-                                        period=period,
-                                        dates=dates)
-                                        )
-        
-        composite = ee.ImageCollection(agg_time_result.collection).toBands()
-        
-        # rename bands depending on number of resulting images
-        if agg_time_result.n_images > 1:
-            bnames = composite.bandNames().map(lambda b: ee.String('t').cat(b))
-        else:
-            bnames = composite.bandNames().map(lambda b: ee.String(b).slice(2))
-        
-        composite = composite.rename(bnames)
-            
-        # compute harmonics if desired
-        if 'harmonicsOptions' in kwargs:
-            harmonics_features = doHarmonicsFromOptions(ds.collection,**kwargs) # returns an ee.Image, not a hf.Dataset
-            composite = composite.addBands(harmonics_features)
-        
-        # add JRC variables if desired
-        if 'addJRCWater' in kwargs:
-            if kwargs['addJRCWater']:
-                composite = idx.addJRC(composite).unmask(0)
-        
-        # add topography variables if desired     
-        if 'addTopography' in kwargs:
-            if kwargs['addTopography']:
-                composite = idx.addTopography(composite).unmask(0)
-        
-        self.bands = composite.bandNames().getInfo()
-        self.image = (composite.clip(region).set('dataset',dataset,
-                                                     'start',start_date,
-                                                     'end',end_date)
-                                                    .set(kwargs)
-                                                    )
-        return
-
-    def stack(self,other) -> ee.Image:
-        """ stacks composites together, formatting bands and properties
-        
-        args:
-            self (rlcms.composite): RLCMS Composite
-            other (rlcms.composite): RLCMS Composite
-        returns:
-            ee.Image
-        """
-        
-        # prefix dataset name to every band, if data is an asset path we swap / for _
-        self_renamed = self.image.regexpRename('^', f"{self.dataset.replace('/','_')}_")
-        other_renamed = other.image.regexpRename('^', f"{other.dataset.replace('/','_')}_")
-        
-        # Traceback: 'ApiFunction' object has no attribute 'name' at line 209... 
-        # toDictionary() doesn't think it is a method of self.image (ee.Image) but it is
-        # # prefix image property keys with dataset name and set all as new properties 
-        # self_props_names = (self.image.propertyNames()
-        #               .map(lambda s: ee.String(s).replace('^', f"{self.dataset.replace('/','_')}_")))
-        # other_props_names = (other.image.propertyNames()
-        #               .map(lambda s: ee.String(s).replace('^', f"{other.dataset.replace('/','_')}_")))
-        
-        # self_props = ee.Image(self.image).toDictionary().rename(self_props_names)
-        # other_props = ee.Image(other.image).toDictionary().rename(other_props_names)
-        
-        # _dict = ee.Dictionary(self_props).combine(other_props)
-        return ee.Image.cat([self_renamed,other_renamed])#.set(_dict)
+import ee
+import hydrafloods as hf
+from rlcms.harmonics import doHarmonicsFromOptions
+from rlcms.covariates import indices
+from rlcms.covariates import returnCovariatesFromOptions
+from ee.ee_exception import EEException
+
+ee.Initialize()
+
+idx = indices()
+
+def get_agg_timing(collection:hf.Dataset,**kwargs):
+    """utility function for hf.Dataset.aggregate_time(). Formats `period`, `period_unit`, and `dates` args
+        to create certain types of composites (defined by `composite_mode`)
+    args:
+        collection (hf.Dataset): Hydrafloods Dataset
+    kwargs:
+        composite_mode (str): one of 'annual' or 'seasonal', Default = 'annual'
+        season (list[str|int]): consecutive list of months (e.g. ['01','02','03']) comprising the season.
+            A required arg if composite_mode == 'seasonal'
+    Returns:
+        tuple(period(int),period_unit(str),dates(list[str]))
+            
+    """
+    if 'composite_mode' not in kwargs:
+        composite_mode = 'annual'
+    else:
+        composite_mode = kwargs['composite_mode']
+    
+    # get unique yyyy strings
+    years = list(set([d.split(' ')[0].split('-')[0] for d in collection.dates])) 
+    years.sort()
+    
+    if composite_mode == 'seasonal':
+        if 'season' not in kwargs:
+            raise ValueError("season arg required if composite_mode == 'seasonal'")
+        else:
+            season = kwargs['season'] # must be consecutive 
+            period = len(season)
+            period_unit = 'month'
+            dates = [f"{y}-{str(season[0])}-01" for y in years]
+    elif composite_mode == 'annual':
+        period = 1
+        period_unit = 'year'
+        dates = [y+'-01-01' for y in years]
+    
+    else:
+        raise ValueError(f"{composite_mode} not a valid 'composite_mode'. Choose one of 'annual' or 'seasonal'")
+    
+    return period,period_unit,dates
+
+class Composite:
+    """Initializes Composite class
+    
+        Processes multi-band composite of your chosen dataset(s) within an AOI footprint polygon
+
+        args:
+            dataset (str): one of: 'Landsat5','Landsat7','Landsat8','Sentinel1Asc','Sentinel1Desc','Sentinel2','Modis','Viirs')
+            region (ee.FeatureCollection): area of interest
+            start_date (str): start date
+            end_date (str): end date
+        
+        kwargs:
+            indices:list[str]
+            composite_mode:str One of ['seasonal','annual'] Default = 'annual' 
+            season:list[str|int]
+            reducer:str|ee.Reducer
+            addTasselCap:bool
+            addTopography:bool
+            addJRC:bool
+            harmonicsOptions:dict in this format: {'nir':{'start':int[1:365],'end':[1:365]}}
+        
+        returns:
+            ee.Image: multi-band image composite within region
+        """
+    
+    def __init__(self,dataset:str,
+                    region:ee.FeatureCollection,
+                    start_date:str,
+                    end_date:str,
+                    **kwargs):
+    
+        self.dataset=dataset
+        if isinstance(region, ee.Geometry):
+            self.region=region.getInfo()['coordinates']
+        elif isinstance(region, ee.FeatureCollection):
+            self.region = region.geometry().getInfo()['coordinates']
+        self.start_date=start_date
+        self.end_date=end_date
+        
+        for key, value in kwargs.items():
+            setattr(self, key, value)
+        
+        # testing whether need to go b/w FC and Geometry for multi_poly
+        if isinstance(region,ee.FeatureCollection):
+            region = region.geometry()
+            region_fc = region
+        elif isinstance(region,ee.Geometry):
+            region = region
+        else:
+            raise TypeError(f"{region} must be of type ee.FeatureCollection or ee.Geometry, got {type(region)}")
+        # all hydrafloods.Dataset sub-classes
+        ds_dict = {'Landsat5':hf.Landsat5(region,start_date,end_date),
+                'Landsat7':hf.Landsat7(region,start_date,end_date),
+                'Landsat8':hf.Landsat8(region,start_date,end_date),
+                'Landsat9':hf.Landsat9(region,start_date,end_date),
+                'Sentinel1':hf.Sentinel1(region,start_date,end_date),
+                'Sentinel1Asc':hf.Sentinel1Asc(region,start_date,end_date),
+                'Sentinel1Desc':hf.Sentinel1Desc(region,start_date,end_date),
+                'Sentinel2':hf.Sentinel2(region,start_date,end_date),
+                'MODIS':hf.Modis(region,start_date,end_date),
+                'VIIRS':hf.Viirs(region,start_date,end_date)}
+        
+        # dataset can either be a named dataset string supported by a hf.Dataset sub-class 
+        # or a GEE Asset path
+        if isinstance(dataset,str):
+            if dataset in ds_dict.keys(): 
+                ds = ds_dict[dataset]
+            else:
+                if '/' in dataset: 
+                    try:
+                        ds = hf.Dataset(asset_id=dataset,region=region,start_time=start_date,end_time=end_date)
+                    except:
+                        raise EEException
+                else: 
+                    raise ValueError(f"Could not construct a hf.Dataset from dataset name provided: {dataset}")
+        else:
+            raise TypeError(f"dataset must be str type, got: {type(dataset)}")
+        
+        # mask imgs to geometries in multi_poly mode
+        if 'multi_poly' in kwargs:
+            if kwargs['multi_poly'] == True:
+                def update_mask(img):
+                    ref_poly_img = ee.Image(1).paint(region_fc).Not().selfMask() # aoi can be ee.Geometry or ee.FeatureCollection for this
+                    return ee.Image(img).updateMask(ref_poly_img)
+                # do we want to warn user against using multi_poly unnecessarily if aoi is a single geometry?
+                # would require another synchronous request of aoi's type/element size
+                ds = ds.apply_func(update_mask)
+        
+        ds = ds.apply_func(returnCovariatesFromOptions,**kwargs)
+        
+        # set reducer passed to aggregate_time(), default mean
+        if 'reducer' in kwargs:
+            reducer=kwargs['reducer']
+        else:
+            reducer = 'mean'
+        
+        period,period_unit,dates = get_agg_timing(ds,**kwargs)
+        
+        # aggregate hf.Dataset
+        agg_time_result = (ds.aggregate_time(reducer=reducer,
+                                        rename=False,
+                                        period_unit=period_unit,
+                                        period=period,
+                                        dates=dates)
+                                        )
+        
+        composite = ee.ImageCollection(agg_time_result.collection).toBands()
+        
+        # rename bands depending on number of resulting images
+        if agg_time_result.n_images > 1:
+            bnames = composite.bandNames().map(lambda b: ee.String('t').cat(b))
+        else:
+            bnames = composite.bandNames().map(lambda b: ee.String(b).slice(2))
+        
+        composite = composite.rename(bnames)
+            
+        # compute harmonics if desired
+        if 'harmonicsOptions' in kwargs:
+            harmonics_features = doHarmonicsFromOptions(ds.collection,**kwargs) # returns an ee.Image, not a hf.Dataset
+            composite = composite.addBands(harmonics_features)
+        
+        # add JRC variables if desired
+        if 'addJRCWater' in kwargs:
+            if kwargs['addJRCWater']:
+                composite = idx.addJRC(composite).unmask(0)
+        
+        # add topography variables if desired     
+        if 'addTopography' in kwargs:
+            if kwargs['addTopography']:
+                composite = idx.addTopography(composite).unmask(0)
+        
+        self.bands = composite.bandNames().getInfo()
+        self.image = (composite.clip(region).set('dataset',dataset,
+                                                     'start',start_date,
+                                                     'end',end_date)
+                                                    .set(kwargs)
+                                                    )
+        return
+
+def stack(composites:list):
+    """
+    stacks a list of rlcms.Composites together, prefixing each band with the Composite's dataset name
+    args:
+        composites: list[rlcms.Composite]
+    returns:
+        ee.Image
+    """
+    if len(composites) < 2 or not all(isinstance(c,Composite) for c in composites):
+        raise ValueError("composites must be a list of 2 or more rlcms.Composites")
+    else:
+        # returns list of ee.Images with renamed bands
+        renamed = [c.image.regexpRename('^', f"{c.dataset.replace('/','_')}_") for c in composites]
+        # stack renamed image list into one ee.Image
+        stacked = ee.Image.cat(renamed)
+        return stacked
```

### Comparing `rlcms-2023.9.7/src/rlcms/covariates.py` & `rlcms-2024.5.29/src/rlcms/covariates.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,349 +1,349 @@
-import ee, math
-from rlcms.utils import parse_settings
-class indices():
-
-	def __init__(self):
-		
-		
-		 
-		# list with functions to call for each index
-		self.functionList = {"ND_blue_green" : self.ND_blue_green, \
-							 "ND_blue_red" : self.ND_blue_red, \
-							 "ND_blue_nir" : self.ND_blue_nir, \
-							 "ND_blue_swir1" : self.ND_blue_swir1, \
-							 "ND_blue_swir2" : self.ND_blue_swir2, \
-							 "ND_green_red" : self.ND_green_red, \
-							 "ND_green_nir" : self.ND_green_nir, \
-							 "ND_green_swir1" : self.ND_green_swir1, \
-							 "ND_green_swir2" : self.ND_green_swir2, \
-							 "ND_red_swir1" : self.ND_red_swir1, \
-							 "ND_red_swir2" : self.ND_red_swir2, \
-							 "ND_nir_red" : self.ND_nir_red, \
-							 "ND_nir_swir1" : self.ND_nir_swir1, \
-							 "ND_nir_swir2" : self.ND_nir_swir2, \
-							 "ND_swir1_swir2" : self.ND_swir1_swir2, \
-							 "R_swir1_nir" : self.R_swir1_nir, \
-							 "R_red_swir1" : self.R_red_swir1, \
-							 "EVI" : self.EVI, \
-							 "SAVI" : self.SAVI, \
-							 "IBI" : self.IBI}
-
-
-	def addAllTasselCapIndices(self,img): 
-		""" Function to get all tasselCap indices """
-		
-		def getTasseledCap(img):
-			"""Function to compute the Tasseled Cap transformation and return an image"""
-			
-			coefficients = ee.Array([
-				[0.3037, 0.2793, 0.4743, 0.5585, 0.5082, 0.1863],
-				[-0.2848, -0.2435, -0.5436, 0.7243, 0.0840, -0.1800],
-				[0.1509, 0.1973, 0.3279, 0.3406, -0.7112, -0.4572],
-				[-0.8242, 0.0849, 0.4392, -0.0580, 0.2012, -0.2768],
-				[-0.3280, 0.0549, 0.1075, 0.1855, -0.4357, 0.8085],
-				[0.1084, -0.9022, 0.4120, 0.0573, -0.0251, 0.0238]
-			])
-		
-			bands=ee.List(['blue','green','red','nir','swir1','swir2'])
-			
-			# Make an Array Image, with a 1-D Array per pixel.
-			arrayImage1D = img.select(bands).toArray()
-		
-			# Make an Array Image with a 2-D Array per pixel, 6x1.
-			arrayImage2D = arrayImage1D.toArray(1)
-		
-			componentsImage = ee.Image(coefficients).matrixMultiply(arrayImage2D).arrayProject([0]).arrayFlatten([['brightness', 'greenness', 'wetness', 'fourth', 'fifth', 'sixth']]).float()
-	  
-			# Get a multi-band image with TC-named bands.
-			return img.addBands(componentsImage);	
-			
-			
-		def addTCAngles(img):
-
-			""" Function to add Tasseled Cap angles and distances to an image. Assumes image has bands: 'brightness', 'greenness', and 'wetness'."""
-			
-			# Select brightness, greenness, and wetness bands	
-			brightness = img.select('brightness')
-			greenness = img.select('greenness')
-			wetness = img.select('wetness')
-	  
-			# Calculate Tasseled Cap angles and distances
-			tcAngleBG = brightness.atan2(greenness).divide(math.pi).rename(['tcAngleBG'])
-			tcAngleGW = greenness.atan2(wetness).divide(math.pi).rename(['tcAngleGW'])
-			tcAngleBW = brightness.atan2(wetness).divide(math.pi).rename(['tcAngleBW'])
-			tcDistBG = brightness.hypot(greenness).rename(['tcDistBG'])
-			tcDistGW = greenness.hypot(wetness).rename(['tcDistGW'])
-			tcDistBW = brightness.hypot(wetness).rename(['tcDistBW'])
-			img = img.addBands(tcAngleBG).addBands(tcAngleGW).addBands(tcAngleBW).addBands(tcDistBG).addBands(tcDistGW).addBands(tcDistBW)
-			
-			return img
-	
-		img = getTasseledCap(img)
-		img = addTCAngles(img)
-		return img
-
-	def ND_blue_green(self,img):
-		img = img.addBands(img.normalizedDifference(['blue','green']).rename(['ND_blue_green']))
-		return img
-	
-	def ND_blue_red(self,img):
-		img = img.addBands(img.normalizedDifference(['blue','red']).rename(['ND_blue_red']))
-		return img
-	
-	def ND_blue_nir(self,img):
-		img = img.addBands(img.normalizedDifference(['blue','nir']).rename(['ND_blue_nir']))
-		return img
-	
-	def ND_blue_swir1(self,img):
-		img = img.addBands(img.normalizedDifference(['blue','swir1']).rename(['ND_blue_swir1']))
-		return img
-	
-	def ND_blue_swir2(self,img):
-		img = img.addBands(img.normalizedDifference(['blue','swir2']).rename(['ND_blue_swir2']))
-		return img
-
-	def ND_green_red(self,img):
-		img = img.addBands(img.normalizedDifference(['green','red']).rename(['ND_green_red']))
-		return img
-	
-	def ND_green_nir(self,img):
-		img = img.addBands(img.normalizedDifference(['green','nir']).rename(['ND_green_nir']))  # NDWBI
-		return img
-	
-	def ND_green_swir1(self,img):
-		img = img.addBands(img.normalizedDifference(['green','swir1']).rename(['ND_green_swir1']))  # NDSI, MNDWI
-		return img
-	
-	def ND_green_swir2(self,img):
-		img = img.addBands(img.normalizedDifference(['green','swir2']).rename(['ND_green_swir2']))
-		return img
-		
-	def ND_red_swir1(self,img):
-		img = img.addBands(img.normalizedDifference(['red','swir1']).rename(['ND_red_swir1']))
-		return img
-			
-	def ND_red_swir2(self,img):
-		img = img.addBands(img.normalizedDifference(['red','swir2']).rename(['ND_red_swir2']))
-		return img
-
-	def ND_nir_red(self,img):
-		img = img.addBands(img.normalizedDifference(['nir','red']).rename(['ND_nir_red']))  # NDVI
-		return img
-	
-	def ND_nir_swir1(self,img):
-		img = img.addBands(img.normalizedDifference(['nir','swir1']).rename(['ND_nir_swir1']))  # NDWI, LSWI, -NDBI
-		return img
-	
-	def ND_nir_swir2(self,img):
-		img = img.addBands(img.normalizedDifference(['nir','swir2']).rename(['ND_nir_swir2'])) # NBR, MNDVI
-		return img
-
-	def ND_swir1_swir2(self,img):
-		img = img.addBands(img.normalizedDifference(['swir1','swir2']).rename(['ND_swir1_swir2']))
-		return img
-  
-	def R_swir1_nir(self,img):
-		# Add ratios
-		img = img.addBands(img.select('swir1').divide(img.select('nir')).rename(['R_swir1_nir']));  # ratio 5/4
-		return img
-			
-	def R_red_swir1(self,img):
-		img = img.addBands(img.select('red').divide(img.select('swir1')).rename(['R_red_swir1']));  # ratio 3/5
-		return img
-
-	def EVI(self,img):
-		#Add Enhanced Vegetation Index (EVI)
-		evi = img.expression(
-			'2.5 * ((NIR - RED) / (NIR + 6 * RED - 7.5 * BLUE + 1))', {
-			  'NIR': img.select('nir'),
-			  'RED': img.select('red'),
-			  'BLUE': img.select('blue')
-		  }).float()
-	
-		img = img.addBands(evi.rename(['EVI']))
-
-		return img
-	  
-	def SAVI(self,img):
-		# Add Soil Adjust Vegetation Index (SAVI)
-		# using L = 0.5;
-		savi = img.expression(
-			'(NIR - RED) * (1 + 0.5)/(NIR + RED + 0.5)', {
-			  'NIR': img.select('nir'),
-			  'RED': img.select('red')
-		  }).float()
-		img = img.addBands(savi.rename(['SAVI']))
-
-		return img
-	  
-	def IBI(self,img):
-		# Add Index-Based Built-Up Index (IBI)
-		ibi_a = img.expression(
-			'2*SWIR1/(SWIR1 + NIR)', {
-			  'SWIR1': img.select('swir1'),
-			  'NIR': img.select('nir')
-			}).rename(['IBI_A'])
-	
-
-		ibi_b = img.expression(
-			'(NIR/(NIR + RED)) + (GREEN/(GREEN + SWIR1))', {
-			  'NIR': img.select('nir'),
-			  'RED': img.select('red'),
-			  'GREEN': img.select('green'),
-			  'SWIR1': img.select('swir1')
-			}).rename(['IBI_B'])
-		
-		ibi_a = ibi_a.addBands(ibi_b)
-		ibi = ibi_a.normalizedDifference(['IBI_A','IBI_B'])
-		img = img.addBands(ibi.rename(['IBI']))
-		
-		return img
-
-	def addTopography(self,img): 
-		"""  Function to add 30m SRTM elevation and derived slope, aspect, eastness, and 
-		northness to an image. Elevation is in meters, slope is between 0 and 90 deg,
-		aspect is between 0 and 359 deg. Eastness and northness are unitless and are
-		between -1 and 1. """
-
-		# Import SRTM elevation data
-		elevation = ee.Image("USGS/SRTMGL1_003")
-		
-		# Calculate slope, aspect, and hillshade
-		topo = ee.Algorithms.Terrain(elevation)
-		
-		# From aspect (a), calculate eastness (sin a), northness (cos a)
-		deg2rad = ee.Number(math.pi).divide(180)
-		aspect = topo.select(['aspect'])
-		aspect_rad = aspect.multiply(deg2rad)
-		eastness = aspect_rad.sin().rename(['eastness']).float()
-		northness = aspect_rad.cos().rename(['northness']).float()
-		
-		# Add topography bands to image
-		topo = topo.select(['elevation','slope','aspect']).addBands(eastness).addBands(northness)
-		img = img.addBands(topo)
-		return img
-
-	def addJRC(self,img):
-		""" Function to add JRC Water layers: 'occurrence', 'change_abs', 
-			'change_norm', 'seasonality','transition', 'max_extent' """
-		
-		jrcImage = ee.Image("JRC/GSW1_0/GlobalSurfaceWater")
-		
-		img = img.addBands(jrcImage.select(['occurrence']).rename(['occurrence']))
-		img = img.addBands(jrcImage.select(['change_abs']).rename(['change_abs']))
-		img = img.addBands(jrcImage.select(['change_norm']).rename(['change_norm']))
-		img = img.addBands(jrcImage.select(['seasonality']).rename(['seasonality']))
-		img = img.addBands(jrcImage.select(['transition']).rename(['transition']))
-		img = img.addBands(jrcImage.select(['max_extent']).rename(['max_extent']))
-		
-		return img
-
-
-	def getIndices(self,img,covariates):	
-		""" add indices to image"""
-		# self = indices()
-		# no need to add indices that are already there
-		# see TODO below, can't use removeDuplicates in .map()
-		# indices = self.removeDuplicates(covariates,img.bandNames().getInfo())
-		indices = covariates
-		
-		for item in indices:
-			img = self.functionList[item](img)
-
-		return img
-
-	def removeDuplicates(self,covariateList,bands):
-		""" function to remove duplicates, i.e. existing bands do not need to be calculated """
-		# TODO: this does not scale to being mappable server side (can't use getInfo in mapped functions)
-		# would need to EEify this logic to use with ee.List()'s
-		return [elem for elem in covariateList if elem not in bands]
-
-	def renameBands(self,image,prefix):
-		""" renames bands with prefix """
-		
-		bandnames = image.bandNames()
-
-		def mapBands(band):
-			band = ee.String(prefix).cat('_').cat(band)
-			return band
-			
-		bandnames = bandnames.map(mapBands)
-		
-		image = image.rename(bandnames)
-
-		return image
-
-
-def returnCovariates(img):
-	"""Workflow for computing Landsat and covariates. bands and covariates are hardcoded inside the function."""
-	# hard coded for now
-	bands = ['blue','green','red','nir','swir1', 'swir2']	
-	bandLow = ['p20_blue','p20_green','p20_red','p20_nir','p20_swir1', 'p20_swir2']
-	bandHigh = ['p80_blue','p80_green','p80_red','p80_nir','p80_swir1', 'p80_swir2']
-
-	"""Calculate the urban, builtup cropland rice and barren primitives """
-	covariates = ["ND_blue_green","ND_blue_red","ND_blue_nir","ND_blue_swir1","ND_blue_swir2", \
-				  "ND_green_red","ND_green_nir","ND_green_swir1","ND_green_swir2","ND_red_swir1",\
-				  "ND_red_swir2","ND_nir_red","ND_nir_swir1","ND_nir_swir2","ND_swir1_swir2",\
-				  "R_swir1_nir","R_red_swir1","EVI","SAVI","IBI"]
-		
-	index = indices()
-	
-	def scaleLandsat(img):
-		"""Landast is scaled by factor 0.0001 """
-		thermalBand = ee.List(['thermal'])
-		thermal = ee.Image(img).select(thermalBand).divide(10)
-					
-		otherBands = ee.Image(img).bandNames().removeAll(thermalBand)
-		
-		scaled = ee.Image(img).select(otherBands).multiply(0.0001)
-		image = ee.Image(scaled.addBands(thermal))        
-	    
-		return ee.Image(image.copyProperties(img))
-
-	img = scaleLandsat(img)
-		
-	def addIndices(img,prefix):
-		img = index.addAllTasselCapIndices(img)
-		img = index.getIndices(img,covariates)
-		img = index.addJRC(img).unmask(0)
-		img = index.addTopography(img).unmask(0)	
-		if len(prefix) > 0:	
-			img = index.renameBands(img,prefix)
-		return img
-			
-		
-	down = addIndices(img.select(bandLow,bands),"p20")
-	middle = addIndices(img.select(bands),"")
-	up = addIndices(img.select(bandHigh,bands),"p80")
-		
-	img = down.addBands(middle).addBands(up)
-	
-	return img
-
-# TODO: can't figure out how to detangle getIndices() and addAllTasselCapIndices() 
-# so that they can be directly passed as func to hf.Dataset.apply_func()
-# so we have this function that takes unnamed kwargs, passed to apply_func()..
-def returnCovariatesFromOptions(img,**kwargs):
-	"""
-	Computes and adds image covariates according to user settings
-	args:
-		img (ee.Image): image to compute covariates 
-		kwargs (dict): a settings dictionary 
-	returns:
-		img (ee.Image): multi-band image with all desired covariates
-	"""
-	settings = kwargs
-	if 'indices' in kwargs.keys():
-		if len(kwargs['indices']) > 0:
-			covariates = settings['indices']
-			index = indices()
-		
-		img = ee.Image(img)
-		img = index.getIndices(img,covariates)
-	
-	if 'addTasselCap' in kwargs.keys():
-		if kwargs['addTasselCap']:
-			img = index.addAllTasselCapIndices(img)
-	
+import ee, math
+from rlcms.utils import parse_settings
+class indices():
+
+	def __init__(self):
+		
+		
+		 
+		# list with functions to call for each index
+		self.functionList = {"ND_blue_green" : self.ND_blue_green, \
+							 "ND_blue_red" : self.ND_blue_red, \
+							 "ND_blue_nir" : self.ND_blue_nir, \
+							 "ND_blue_swir1" : self.ND_blue_swir1, \
+							 "ND_blue_swir2" : self.ND_blue_swir2, \
+							 "ND_green_red" : self.ND_green_red, \
+							 "ND_green_nir" : self.ND_green_nir, \
+							 "ND_green_swir1" : self.ND_green_swir1, \
+							 "ND_green_swir2" : self.ND_green_swir2, \
+							 "ND_red_swir1" : self.ND_red_swir1, \
+							 "ND_red_swir2" : self.ND_red_swir2, \
+							 "ND_nir_red" : self.ND_nir_red, \
+							 "ND_nir_swir1" : self.ND_nir_swir1, \
+							 "ND_nir_swir2" : self.ND_nir_swir2, \
+							 "ND_swir1_swir2" : self.ND_swir1_swir2, \
+							 "R_swir1_nir" : self.R_swir1_nir, \
+							 "R_red_swir1" : self.R_red_swir1, \
+							 "EVI" : self.EVI, \
+							 "SAVI" : self.SAVI, \
+							 "IBI" : self.IBI}
+
+
+	def addAllTasselCapIndices(self,img): 
+		""" Function to get all tasselCap indices """
+		
+		def getTasseledCap(img):
+			"""Function to compute the Tasseled Cap transformation and return an image"""
+			
+			coefficients = ee.Array([
+				[0.3037, 0.2793, 0.4743, 0.5585, 0.5082, 0.1863],
+				[-0.2848, -0.2435, -0.5436, 0.7243, 0.0840, -0.1800],
+				[0.1509, 0.1973, 0.3279, 0.3406, -0.7112, -0.4572],
+				[-0.8242, 0.0849, 0.4392, -0.0580, 0.2012, -0.2768],
+				[-0.3280, 0.0549, 0.1075, 0.1855, -0.4357, 0.8085],
+				[0.1084, -0.9022, 0.4120, 0.0573, -0.0251, 0.0238]
+			])
+		
+			bands=ee.List(['blue','green','red','nir','swir1','swir2'])
+			
+			# Make an Array Image, with a 1-D Array per pixel.
+			arrayImage1D = img.select(bands).toArray()
+		
+			# Make an Array Image with a 2-D Array per pixel, 6x1.
+			arrayImage2D = arrayImage1D.toArray(1)
+		
+			componentsImage = ee.Image(coefficients).matrixMultiply(arrayImage2D).arrayProject([0]).arrayFlatten([['brightness', 'greenness', 'wetness', 'fourth', 'fifth', 'sixth']]).float()
+	  
+			# Get a multi-band image with TC-named bands.
+			return img.addBands(componentsImage);	
+			
+			
+		def addTCAngles(img):
+
+			""" Function to add Tasseled Cap angles and distances to an image. Assumes image has bands: 'brightness', 'greenness', and 'wetness'."""
+			
+			# Select brightness, greenness, and wetness bands	
+			brightness = img.select('brightness')
+			greenness = img.select('greenness')
+			wetness = img.select('wetness')
+	  
+			# Calculate Tasseled Cap angles and distances
+			tcAngleBG = brightness.atan2(greenness).divide(math.pi).rename(['tcAngleBG'])
+			tcAngleGW = greenness.atan2(wetness).divide(math.pi).rename(['tcAngleGW'])
+			tcAngleBW = brightness.atan2(wetness).divide(math.pi).rename(['tcAngleBW'])
+			tcDistBG = brightness.hypot(greenness).rename(['tcDistBG'])
+			tcDistGW = greenness.hypot(wetness).rename(['tcDistGW'])
+			tcDistBW = brightness.hypot(wetness).rename(['tcDistBW'])
+			img = img.addBands(tcAngleBG).addBands(tcAngleGW).addBands(tcAngleBW).addBands(tcDistBG).addBands(tcDistGW).addBands(tcDistBW)
+			
+			return img
+	
+		img = getTasseledCap(img)
+		img = addTCAngles(img)
+		return img
+
+	def ND_blue_green(self,img):
+		img = img.addBands(img.normalizedDifference(['blue','green']).rename(['ND_blue_green']))
+		return img
+	
+	def ND_blue_red(self,img):
+		img = img.addBands(img.normalizedDifference(['blue','red']).rename(['ND_blue_red']))
+		return img
+	
+	def ND_blue_nir(self,img):
+		img = img.addBands(img.normalizedDifference(['blue','nir']).rename(['ND_blue_nir']))
+		return img
+	
+	def ND_blue_swir1(self,img):
+		img = img.addBands(img.normalizedDifference(['blue','swir1']).rename(['ND_blue_swir1']))
+		return img
+	
+	def ND_blue_swir2(self,img):
+		img = img.addBands(img.normalizedDifference(['blue','swir2']).rename(['ND_blue_swir2']))
+		return img
+
+	def ND_green_red(self,img):
+		img = img.addBands(img.normalizedDifference(['green','red']).rename(['ND_green_red']))
+		return img
+	
+	def ND_green_nir(self,img):
+		img = img.addBands(img.normalizedDifference(['green','nir']).rename(['ND_green_nir']))  # NDWBI
+		return img
+	
+	def ND_green_swir1(self,img):
+		img = img.addBands(img.normalizedDifference(['green','swir1']).rename(['ND_green_swir1']))  # NDSI, MNDWI
+		return img
+	
+	def ND_green_swir2(self,img):
+		img = img.addBands(img.normalizedDifference(['green','swir2']).rename(['ND_green_swir2']))
+		return img
+		
+	def ND_red_swir1(self,img):
+		img = img.addBands(img.normalizedDifference(['red','swir1']).rename(['ND_red_swir1']))
+		return img
+			
+	def ND_red_swir2(self,img):
+		img = img.addBands(img.normalizedDifference(['red','swir2']).rename(['ND_red_swir2']))
+		return img
+
+	def ND_nir_red(self,img):
+		img = img.addBands(img.normalizedDifference(['nir','red']).rename(['ND_nir_red']))  # NDVI
+		return img
+	
+	def ND_nir_swir1(self,img):
+		img = img.addBands(img.normalizedDifference(['nir','swir1']).rename(['ND_nir_swir1']))  # NDWI, LSWI, -NDBI
+		return img
+	
+	def ND_nir_swir2(self,img):
+		img = img.addBands(img.normalizedDifference(['nir','swir2']).rename(['ND_nir_swir2'])) # NBR, MNDVI
+		return img
+
+	def ND_swir1_swir2(self,img):
+		img = img.addBands(img.normalizedDifference(['swir1','swir2']).rename(['ND_swir1_swir2']))
+		return img
+  
+	def R_swir1_nir(self,img):
+		# Add ratios
+		img = img.addBands(img.select('swir1').divide(img.select('nir')).rename(['R_swir1_nir']));  # ratio 5/4
+		return img
+			
+	def R_red_swir1(self,img):
+		img = img.addBands(img.select('red').divide(img.select('swir1')).rename(['R_red_swir1']));  # ratio 3/5
+		return img
+
+	def EVI(self,img):
+		#Add Enhanced Vegetation Index (EVI)
+		evi = img.expression(
+			'2.5 * ((NIR - RED) / (NIR + 6 * RED - 7.5 * BLUE + 1))', {
+			  'NIR': img.select('nir'),
+			  'RED': img.select('red'),
+			  'BLUE': img.select('blue')
+		  }).float()
+	
+		img = img.addBands(evi.rename(['EVI']))
+
+		return img
+	  
+	def SAVI(self,img):
+		# Add Soil Adjust Vegetation Index (SAVI)
+		# using L = 0.5;
+		savi = img.expression(
+			'(NIR - RED) * (1 + 0.5)/(NIR + RED + 0.5)', {
+			  'NIR': img.select('nir'),
+			  'RED': img.select('red')
+		  }).float()
+		img = img.addBands(savi.rename(['SAVI']))
+
+		return img
+	  
+	def IBI(self,img):
+		# Add Index-Based Built-Up Index (IBI)
+		ibi_a = img.expression(
+			'2*SWIR1/(SWIR1 + NIR)', {
+			  'SWIR1': img.select('swir1'),
+			  'NIR': img.select('nir')
+			}).rename(['IBI_A'])
+	
+
+		ibi_b = img.expression(
+			'(NIR/(NIR + RED)) + (GREEN/(GREEN + SWIR1))', {
+			  'NIR': img.select('nir'),
+			  'RED': img.select('red'),
+			  'GREEN': img.select('green'),
+			  'SWIR1': img.select('swir1')
+			}).rename(['IBI_B'])
+		
+		ibi_a = ibi_a.addBands(ibi_b)
+		ibi = ibi_a.normalizedDifference(['IBI_A','IBI_B'])
+		img = img.addBands(ibi.rename(['IBI']))
+		
+		return img
+
+	def addTopography(self,img): 
+		"""  Function to add 30m SRTM elevation and derived slope, aspect, eastness, and 
+		northness to an image. Elevation is in meters, slope is between 0 and 90 deg,
+		aspect is between 0 and 359 deg. Eastness and northness are unitless and are
+		between -1 and 1. """
+
+		# Import SRTM elevation data
+		elevation = ee.Image("USGS/SRTMGL1_003")
+		
+		# Calculate slope, aspect, and hillshade
+		topo = ee.Algorithms.Terrain(elevation)
+		
+		# From aspect (a), calculate eastness (sin a), northness (cos a)
+		deg2rad = ee.Number(math.pi).divide(180)
+		aspect = topo.select(['aspect'])
+		aspect_rad = aspect.multiply(deg2rad)
+		eastness = aspect_rad.sin().rename(['eastness']).float()
+		northness = aspect_rad.cos().rename(['northness']).float()
+		
+		# Add topography bands to image
+		topo = topo.select(['elevation','slope','aspect']).addBands(eastness).addBands(northness)
+		img = img.addBands(topo)
+		return img
+
+	def addJRC(self,img):
+		""" Function to add JRC Water layers: 'occurrence', 'change_abs', 
+			'change_norm', 'seasonality','transition', 'max_extent' """
+		
+		jrcImage = ee.Image("JRC/GSW1_0/GlobalSurfaceWater")
+		
+		img = img.addBands(jrcImage.select(['occurrence']).rename(['occurrence']))
+		img = img.addBands(jrcImage.select(['change_abs']).rename(['change_abs']))
+		img = img.addBands(jrcImage.select(['change_norm']).rename(['change_norm']))
+		img = img.addBands(jrcImage.select(['seasonality']).rename(['seasonality']))
+		img = img.addBands(jrcImage.select(['transition']).rename(['transition']))
+		img = img.addBands(jrcImage.select(['max_extent']).rename(['max_extent']))
+		
+		return img
+
+
+	def getIndices(self,img,covariates):	
+		""" add indices to image"""
+		# self = indices()
+		# no need to add indices that are already there
+		# see TODO below, can't use removeDuplicates in .map()
+		# indices = self.removeDuplicates(covariates,img.bandNames().getInfo())
+		indices = covariates
+		
+		for item in indices:
+			img = self.functionList[item](img)
+
+		return img
+
+	def removeDuplicates(self,covariateList,bands):
+		""" function to remove duplicates, i.e. existing bands do not need to be calculated """
+		# TODO: this does not scale to being mappable server side (can't use getInfo in mapped functions)
+		# would need to EEify this logic to use with ee.List()'s
+		return [elem for elem in covariateList if elem not in bands]
+
+	def renameBands(self,image,prefix):
+		""" renames bands with prefix """
+		
+		bandnames = image.bandNames()
+
+		def mapBands(band):
+			band = ee.String(prefix).cat('_').cat(band)
+			return band
+			
+		bandnames = bandnames.map(mapBands)
+		
+		image = image.rename(bandnames)
+
+		return image
+
+
+def returnCovariates(img):
+	"""Workflow for computing Landsat and covariates. bands and covariates are hardcoded inside the function."""
+	# hard coded for now
+	bands = ['blue','green','red','nir','swir1', 'swir2']	
+	bandLow = ['p20_blue','p20_green','p20_red','p20_nir','p20_swir1', 'p20_swir2']
+	bandHigh = ['p80_blue','p80_green','p80_red','p80_nir','p80_swir1', 'p80_swir2']
+
+	"""Calculate the urban, builtup cropland rice and barren primitives """
+	covariates = ["ND_blue_green","ND_blue_red","ND_blue_nir","ND_blue_swir1","ND_blue_swir2", \
+				  "ND_green_red","ND_green_nir","ND_green_swir1","ND_green_swir2","ND_red_swir1",\
+				  "ND_red_swir2","ND_nir_red","ND_nir_swir1","ND_nir_swir2","ND_swir1_swir2",\
+				  "R_swir1_nir","R_red_swir1","EVI","SAVI","IBI"]
+		
+	index = indices()
+	
+	def scaleLandsat(img):
+		"""Landast is scaled by factor 0.0001 """
+		thermalBand = ee.List(['thermal'])
+		thermal = ee.Image(img).select(thermalBand).divide(10)
+					
+		otherBands = ee.Image(img).bandNames().removeAll(thermalBand)
+		
+		scaled = ee.Image(img).select(otherBands).multiply(0.0001)
+		image = ee.Image(scaled.addBands(thermal))        
+	    
+		return ee.Image(image.copyProperties(img))
+
+	img = scaleLandsat(img)
+		
+	def addIndices(img,prefix):
+		img = index.addAllTasselCapIndices(img)
+		img = index.getIndices(img,covariates)
+		img = index.addJRC(img).unmask(0)
+		img = index.addTopography(img).unmask(0)	
+		if len(prefix) > 0:	
+			img = index.renameBands(img,prefix)
+		return img
+			
+		
+	down = addIndices(img.select(bandLow,bands),"p20")
+	middle = addIndices(img.select(bands),"")
+	up = addIndices(img.select(bandHigh,bands),"p80")
+		
+	img = down.addBands(middle).addBands(up)
+	
+	return img
+
+# TODO: can't figure out how to detangle getIndices() and addAllTasselCapIndices() 
+# so that they can be directly passed as func to hf.Dataset.apply_func()
+# so we have this function that takes unnamed kwargs, passed to apply_func()..
+def returnCovariatesFromOptions(img,**kwargs):
+	"""
+	Computes and adds image covariates according to user settings
+	args:
+		img (ee.Image): image to compute covariates 
+		kwargs (dict): a settings dictionary 
+	returns:
+		img (ee.Image): multi-band image with all desired covariates
+	"""
+	settings = kwargs
+	if 'indices' in kwargs.keys():
+		if len(kwargs['indices']) > 0:
+			covariates = settings['indices']
+			index = indices()
+		
+		img = ee.Image(img)
+		img = index.getIndices(img,covariates)
+	
+	if 'addTasselCap' in kwargs.keys():
+		if kwargs['addTasselCap']:
+			img = index.addAllTasselCapIndices(img)
+	
 	return img
```

### Comparing `rlcms-2023.9.7/src/rlcms/harmonics.py` & `rlcms-2024.5.29/src/rlcms/harmonics.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,174 +1,174 @@
-import ee
-import math
-
-ee.Initialize()
-
-def addHarmonicTerms(image):
-    """add Time bands to image"""
-    timeRadians = image.select("t").multiply(2 * math.pi)
-    return image.addBands(timeRadians.cos().rename("cos")).addBands(
-        timeRadians.sin().rename("sin")
-    )
-
-def calculateHarmonic(imageCollection: ee.ImageCollection, dependent: ee.String):
-    """
-    Calculate harmonic coefficients (phase and amplitude) off of an ImageCollection
-    dependent: band that you fit the harmonic model for, must be contained in ImageCollection
-    """
-    harmonicIndependents = ee.List(["constant", "t", "cos", "sin"])
-    #  Add harmonic terms as new image bands.
-    harmonicLandsat = imageCollection.map(addHarmonicTerms)
-    # The output of the regression reduction is a 4x1 array image.
-    harmonicTrend = harmonicLandsat.select(harmonicIndependents.add(dependent)).reduce(
-        ee.Reducer.linearRegression(harmonicIndependents.length(), 1)
-    )
-
-    # Turn the array image into a multi-band image of coefficients.
-    harmonicTrendCoefficients = (
-        harmonicTrend.select("coefficients")
-        .arrayProject([0])
-        .arrayFlatten([harmonicIndependents])
-    )
-
-    # // Compute phase and amplitude.
-    phase = (
-        harmonicTrendCoefficients.select("cos")
-        .atan2(harmonicTrendCoefficients.select("sin"))
-        .rename(dependent.cat("_phase"))
-    )
-
-    amplitude = (
-        harmonicTrendCoefficients.select("cos")
-        .hypot(harmonicTrendCoefficients.select("sin"))
-        .rename(dependent.cat("_amplitude"))
-    )
-    return ee.Image.cat(phase, amplitude)
-
-
-def harmonicRGB(harmonics: ee.Image):
-    """Use the HSV to RGB transform to display phase and amplitude"""
-    amplitude = harmonics.select(".*amplitude")
-    phase = harmonics.select(".*phase")
-
-    rgb = (
-        phase.unitScale(-math.pi, math.pi)
-        .addBands(amplitude.multiply(2.5))
-        .addBands(ee.Image(1))
-        .hsvToRgb()
-    )
-    return rgb
-
-
-def addTimeConstant(imageCollection: ee.ImageCollection, timeField: str):
-    """
-    Add time constant to images in an ImageCollection
-    timeField: time stamp property name (typically is the 'system:time_start' property of an image)
-    """
-    def _(image, timeField):
-        # // Compute time in fractional years since the epoch.
-        date = ee.Date(image.get(timeField))
-        years = date.difference(ee.Date("1970-01-01"), "year")
-        # // Return the image with the added bands.
-        return image.addBands(ee.Image(years).rename("t").float()).addBands(
-            ee.Image.constant(1)
-        )
-
-    return imageCollection.map(lambda i: _(i, timeField))
-
-# TODO: consider using hf.timeseries module instead,
-#  but doesn't look like the methods are exact same as defined here
-#   ht.timeseries functions don't return phase and amplitude..
-def doHarmonicsFromOptions(imgColl:ee.ImageCollection,**kwargs):
-    """
-    calculateHarmonic function band-wise
-    
-    args:
-        imgColl (ee.ImageCollection)
-    kwargs:
-        harmonicsOptions (dict): which band(s) and the DOY start and end date to compute harmonics on
-            formatted like: 
-            {
-                'red':{'start':1,'end':365},
-                'blue':{'start':1,'end':365}
-                }
-    returns:
-        ee.Image containing bands [band_phase, band_amplitude]
-    """
-    imgColl = ee.ImageCollection(imgColl)
-    harmonicsOptions = kwargs['harmonicsOptions']
-
-    # get harmonicsOptions dictionary
-    if isinstance(harmonicsOptions,dict):
-    
-        # get band keys as list
-        bands = ee.Dictionary(harmonicsOptions).keys()
-        
-        def harmonicByBand(band):
-            band = ee.String(band)
-            # get the params for that band
-            bandwiseParams = ee.Dictionary(harmonicsOptions).get(band)
-            
-            # get the start and end DOY parameters
-            start = ee.Dictionary(bandwiseParams).get('start')
-            end = ee.Dictionary(bandwiseParams).get('end')
-            
-            # create temporal filtered imgColl for that band
-            imgCollByBand = (ee.ImageCollection(imgColl)
-                                .select(band)
-                                .filter(ee.Filter.dayOfYear(start,end)))
-            # add time bands
-            timeField = "system:time_start"
-            timeCollection = addTimeConstant(imgCollByBand, timeField)
-        
-            return ee.Image(calculateHarmonic(timeCollection,band))
-    else:
-        raise TypeError(f"harmonicsOptions expects dict type, got: {type(harmonicsOptions)}")
-    
-    # do harmonics by band key in model_inputs dictionary
-    listOfImages = ee.Image.cat(ee.List(bands).map(harmonicByBand))
-    bandStack = ee.Image(ee.ImageCollection.fromImages(listOfImages).toBands())
-    
-    # to remove srcImg band name indexing resulting from .toBands() 
-    # (i.e. [0_swir1_phase, 0_swir1_amplitude] -> [swir1_phase, swir1_amplitude] )
-    bandNames = bandStack.bandNames()
-    fixedBandNames = bandNames.map(lambda e: ee.String(e).split("_").slice(-2).join("_"))
-    return bandStack.rename(fixedBandNames)
-
-if __name__ == "__main__":
-    # inputs
-    roi = ee.Geometry.Point([22.5019, -17.9789])
-    imageCollection = ee.ImageCollection("COPERNICUS/S2_SR")
-    timeField = "system:time_start"
-    dependent = ee.String("B8")
-
-    # Napkin tests...
-    # prep image collection for test
-    filteredCollection = imageCollection.filterBounds(roi).filterDate(
-        "2019-01-01", "2021-01-01"
-    )
-
-    # test add time bands
-    timeCollection = addTimeConstant(filteredCollection, timeField)
-
-    assert timeCollection.select("t", "constant").first().bandNames().getInfo() == [
-        "t",
-        "constant",
-    ]
-
-    harmonics = calculateHarmonic(timeCollection, dependent)
-    # test harmonics returns correect bands
-    assert (
-        harmonics.bandNames().getInfo()
-        == ee.List([dependent.cat("_phase"), dependent.cat("_amplitude")]).getInfo()
-    )
-
-    rgb = harmonicRGB(harmonics)
-    # test rgb returns correct bands
-    eetest = ee.Algorithms.IsEqual(rgb.bandNames(), ["red", "green", "blue"]).getInfo()
-    assert eetest is True
-
-    harmonicsByOptions = doHarmonicsFromOptions(imageCollection)
-    optionBands = 'swir1'
-    assert (harmonicsByOptions.bandNames().getInfo() 
-            == ee.List([optionBands.cat("_phase"), optionBands.cat("_amplitude")]).getInfo()
+import ee
+import math
+
+ee.Initialize()
+
+def addHarmonicTerms(image):
+    """add Time bands to image"""
+    timeRadians = image.select("t").multiply(2 * math.pi)
+    return image.addBands(timeRadians.cos().rename("cos")).addBands(
+        timeRadians.sin().rename("sin")
+    )
+
+def calculateHarmonic(imageCollection: ee.ImageCollection, dependent: ee.String):
+    """
+    Calculate harmonic coefficients (phase and amplitude) off of an ImageCollection
+    dependent: band that you fit the harmonic model for, must be contained in ImageCollection
+    """
+    harmonicIndependents = ee.List(["constant", "t", "cos", "sin"])
+    #  Add harmonic terms as new image bands.
+    harmonicLandsat = imageCollection.map(addHarmonicTerms)
+    # The output of the regression reduction is a 4x1 array image.
+    harmonicTrend = harmonicLandsat.select(harmonicIndependents.add(dependent)).reduce(
+        ee.Reducer.linearRegression(harmonicIndependents.length(), 1)
+    )
+
+    # Turn the array image into a multi-band image of coefficients.
+    harmonicTrendCoefficients = (
+        harmonicTrend.select("coefficients")
+        .arrayProject([0])
+        .arrayFlatten([harmonicIndependents])
+    )
+
+    # // Compute phase and amplitude.
+    phase = (
+        harmonicTrendCoefficients.select("cos")
+        .atan2(harmonicTrendCoefficients.select("sin"))
+        .rename(dependent.cat("_phase"))
+    )
+
+    amplitude = (
+        harmonicTrendCoefficients.select("cos")
+        .hypot(harmonicTrendCoefficients.select("sin"))
+        .rename(dependent.cat("_amplitude"))
+    )
+    return ee.Image.cat(phase, amplitude)
+
+
+def harmonicRGB(harmonics: ee.Image):
+    """Use the HSV to RGB transform to display phase and amplitude"""
+    amplitude = harmonics.select(".*amplitude")
+    phase = harmonics.select(".*phase")
+
+    rgb = (
+        phase.unitScale(-math.pi, math.pi)
+        .addBands(amplitude.multiply(2.5))
+        .addBands(ee.Image(1))
+        .hsvToRgb()
+    )
+    return rgb
+
+
+def addTimeConstant(imageCollection: ee.ImageCollection, timeField: str):
+    """
+    Add time constant to images in an ImageCollection
+    timeField: time stamp property name (typically is the 'system:time_start' property of an image)
+    """
+    def _(image, timeField):
+        # // Compute time in fractional years since the epoch.
+        date = ee.Date(image.get(timeField))
+        years = date.difference(ee.Date("1970-01-01"), "year")
+        # // Return the image with the added bands.
+        return image.addBands(ee.Image(years).rename("t").float()).addBands(
+            ee.Image.constant(1)
+        )
+
+    return imageCollection.map(lambda i: _(i, timeField))
+
+# TODO: consider using hf.timeseries module instead,
+#  but doesn't look like the methods are exact same as defined here
+#   ht.timeseries functions don't return phase and amplitude..
+def doHarmonicsFromOptions(imgColl:ee.ImageCollection,**kwargs):
+    """
+    calculateHarmonic function band-wise
+    
+    args:
+        imgColl (ee.ImageCollection)
+    kwargs:
+        harmonicsOptions (dict): which band(s) and the DOY start and end date to compute harmonics on
+            formatted like: 
+            {
+                'red':{'start':1,'end':365},
+                'blue':{'start':1,'end':365}
+                }
+    returns:
+        ee.Image containing bands [band_phase, band_amplitude]
+    """
+    imgColl = ee.ImageCollection(imgColl)
+    harmonicsOptions = kwargs['harmonicsOptions']
+
+    # get harmonicsOptions dictionary
+    if isinstance(harmonicsOptions,dict):
+    
+        # get band keys as list
+        bands = ee.Dictionary(harmonicsOptions).keys()
+        
+        def harmonicByBand(band):
+            band = ee.String(band)
+            # get the params for that band
+            bandwiseParams = ee.Dictionary(harmonicsOptions).get(band)
+            
+            # get the start and end DOY parameters
+            start = ee.Dictionary(bandwiseParams).get('start')
+            end = ee.Dictionary(bandwiseParams).get('end')
+            
+            # create temporal filtered imgColl for that band
+            imgCollByBand = (ee.ImageCollection(imgColl)
+                                .select(band)
+                                .filter(ee.Filter.dayOfYear(start,end)))
+            # add time bands
+            timeField = "system:time_start"
+            timeCollection = addTimeConstant(imgCollByBand, timeField)
+        
+            return ee.Image(calculateHarmonic(timeCollection,band))
+    else:
+        raise TypeError(f"harmonicsOptions expects dict type, got: {type(harmonicsOptions)}")
+    
+    # do harmonics by band key in model_inputs dictionary
+    listOfImages = ee.Image.cat(ee.List(bands).map(harmonicByBand))
+    bandStack = ee.Image(ee.ImageCollection.fromImages(listOfImages).toBands())
+    
+    # to remove srcImg band name indexing resulting from .toBands() 
+    # (i.e. [0_swir1_phase, 0_swir1_amplitude] -> [swir1_phase, swir1_amplitude] )
+    bandNames = bandStack.bandNames()
+    fixedBandNames = bandNames.map(lambda e: ee.String(e).split("_").slice(-2).join("_"))
+    return bandStack.rename(fixedBandNames)
+
+if __name__ == "__main__":
+    # inputs
+    roi = ee.Geometry.Point([22.5019, -17.9789])
+    imageCollection = ee.ImageCollection("COPERNICUS/S2_SR")
+    timeField = "system:time_start"
+    dependent = ee.String("B8")
+
+    # Napkin tests...
+    # prep image collection for test
+    filteredCollection = imageCollection.filterBounds(roi).filterDate(
+        "2019-01-01", "2021-01-01"
+    )
+
+    # test add time bands
+    timeCollection = addTimeConstant(filteredCollection, timeField)
+
+    assert timeCollection.select("t", "constant").first().bandNames().getInfo() == [
+        "t",
+        "constant",
+    ]
+
+    harmonics = calculateHarmonic(timeCollection, dependent)
+    # test harmonics returns correect bands
+    assert (
+        harmonics.bandNames().getInfo()
+        == ee.List([dependent.cat("_phase"), dependent.cat("_amplitude")]).getInfo()
+    )
+
+    rgb = harmonicRGB(harmonics)
+    # test rgb returns correct bands
+    eetest = ee.Algorithms.IsEqual(rgb.bandNames(), ["red", "green", "blue"]).getInfo()
+    assert eetest is True
+
+    harmonicsByOptions = doHarmonicsFromOptions(imageCollection)
+    optionBands = 'swir1'
+    assert (harmonicsByOptions.bandNames().getInfo() 
+            == ee.List([optionBands.cat("_phase"), optionBands.cat("_amplitude")]).getInfo()
             )
```

### Comparing `rlcms-2023.9.7/src/rlcms.egg-info/PKG-INFO` & `rlcms-2024.5.29/src/rlcms.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,800 +1,745 @@
-Metadata-Version: 2.1
-Name: rlcms
-Version: 2023.9.7
-Summary: workflows for regional land cover mapping, built in Google Earth Engine
-Author-email: Kyle Woodward <kw.geospatial@gmail.com>
-License: GNU GENERAL PUBLIC LICENSE
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
-Project-URL: Homepage, https://github.com/sig-gis/rlcms/
-Keywords: land cover,mapping
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: earthengine-api
-Requires-Dist: hydrafloods
-Requires-Dist: pandas
-Provides-Extra: dev
-Requires-Dist: geemap; extra == "dev"
-
-# Running Regional Land Cover Monitoring System Toolset
-## Installation
-Install with pip: 
-```
-pip install rlcms
-```
-
-## GEE Python API Setup
-Earth Engine requires you to authenticate your account credentials to access the Earth Engine python API and your chosen Cloud Project. We do this with the `gcloud` python utility
-1. Download the installer for the `glcoud` command-line python [utility](https://cloud.google.com/sdk/docs/install) from Google
-2. Run the installer
-3. Select Single User and use the default Destination Folder
-4. Leave the Selected Components to Install as-is and click Install
-5. Leave all four boxes checked, and click Finish. This will open a new command-prompt window and auto run gcloud initialization
-6. It asks whether you'd like to log in, type y - this will open a new browser window to a Google Authentication page
-
-![kaza_readme_gcloudInstaller_initializing](https://user-images.githubusercontent.com/51868526/184163126-7505745b-f7c3-4745-bb36-3948d1b9ff76.JPG)
-
-7. Choose your Google account that is linked to your Earth Engine account, then click Allow on the next page.
-
-![kaza_readme_gcloudInstaller_InitializingSignIn](https://user-images.githubusercontent.com/51868526/184163514-4604ac83-cdad-4dd8-bc67-c37224d6aafc.JPG)
-
-8. You will be redirected to a page that says "You are now authenticated with the gcloud CLI!"
-9. Go back to your shell that had been opened for you by gcloud. It asks you to choose a cloud project and lists all available cloud projects that your google account has access to. Decide which project to authenticate with by typing its number in the list.
-
-![kaza_readme_gcloudInstaller_chooseCloudProject_chooseWWF-SIG](https://user-images.githubusercontent.com/51868526/184165192-c602f058-b485-419c-b5ea-401c7087fb9f.JPG)
-
-10. Back in your separate shell window, first ensure you are in your custom conda env (running `conda activate env-name`), then run:
-```
-earthengine authenticate
-```
-11. In the browser window that opens, select the Google account that is tied to your EE account, select the wwf-sig cloud project, then click Generate Token at the bottom of the page.
-12. On the next page, select your Google account again, then click Allow on the next page.
-13. Copy the authorization token it generates to your clipboard and back in your shell, paste it and hit Enter. 
-
-# Testing Your Setup
-Test that earthengine is setup and authenticated by checking the folder contents within the `wwf-sig` cloud project. 
-* In your shell, run:
-```
-earthengine set_project <project-name>
-earthengine ls projects/project-name/assets
-```
-
-If you do not get an error and it returns a list of folders and assets similar to this then you are good to go! :tada:
-
-# Tool Documentation
-
-Each Command Line Interface (CLI) script tool can be run in your command-line terminal of choice. The user must provide values for each required command-line argument to control the analysis.
-You can first run any script, only declaring the `-h` flag. This will bring up the help dialog with a usage example and a description of required command-line arguments. 
-
-## **sample_pts**
-
-Generate Random Sample Points From an ee.Image, Formatted for Collect Earth Online
-
-The points are pre-formatted for use in Collect Earth Online. You can choose to export the points to Google Drive, to GEE Asset or both. 
-
-example:
-```
-sample_pts -im input/path/to/image -band LANDCOVER -o output/path --n_points 100 --to_drive
-```
-
-## **composite**
-
-Creates a Sentinel-2 Composite for an AOI or reference polygons. 
-
-The resulting band stack is needed for both extracting training data information and as input to a trained model's inference. Set the `-p` flag if your AOI is a set of reference polygons and not one contiguous AOI polygon - this will export band information only within each polygon's footprint. 
-
-example:
-```
-composite -a aoi/fc/path -d Landsat8 -s 2020-01-01 -e 2020-12-31 -o output/path --settings path/to/settings/file.txt
-```
-
-**NOTE: The user can control which spectral indices and time series features to generate in this tool by providing a settings txt file, a template of which is located in the repository : [`/template_settings.txt`](/template_settings.txt). See [ProjectWorkflow.md](/ProjectWorkflow.md) for details.**
-
-## **train_test**
-
-Extract Train and Test Point Data from an Input Image within Reference Polygon Areas.
-
-Generates stratified random samples from reference polygons, splitting the sample points into train and test points if desired. The image bands from the provided image are extracted to every point. 
-
-example:
-```
-train_test -rp path/to/reference_polygon_fc -im path/to/input/stack -o unique/output/path --class_values 1 2 3 4 5 6 7 8 --class_points 10 10 10 10 10 10 10
-```
-
-## **primitives**
-
-Create Land Cover Primitives For All Classes in Provided Training Data. 
-
-This script trains probability Random Forest models for each land cover class in your typology as provided by the numeric 'LANDCOVER' property in the provided reference data. It then exports these binary probability images one land cover at a time into a land cover 'Primitives' image collection. While doing so, it also reports out some model performance metrics saved to a new folder created in your *local* `rlcms/metrics` folder on your computer.
-
-example:
-```
-primitives -i input/stack/path -t training/data/path -o output/primitives/imagecollection/path
-```
-
-## **generate_LC**
-
-Generate Single Land Cover Image From Land Cover Primitives Image Collection
-
-This script takes the RF primitives collection generated from the previous script and creates a single-band land cover image from them, taking the highest-probability Primitive at each pixel to assign the Land Cover class.
-
-example:
-```
-generate_LC -i input/primitives/imagecollection/path -o output/path
-```
-
-
+Metadata-Version: 2.1
+Name: rlcms
+Version: 2024.5.29
+Summary: workflows for regional land cover mapping, built in Google Earth Engine
+Author-email: Kyle Woodward <kw.geospatial@gmail.com>
+License: GNU GENERAL PUBLIC LICENSE
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
+Project-URL: Homepage, https://github.com/sig-gis/rlcms/
+Keywords: land cover,mapping
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: earthengine-api
+Requires-Dist: hydrafloods
+Requires-Dist: pandas
+Provides-Extra: dev
+Requires-Dist: geemap; extra == "dev"
+
+# Regional Land Cover Monitoring System
+## Installation
+Install with pip: 
+```
+pip install rlcms
+```
+
+Test that `earthengine-api` is setup and authenticated by checking the folder contents within one of your cloud projects. 
+* In your shell, run:
+```
+earthengine set_project <project-name>
+earthengine ls projects/project-name/assets
+```
+If you do not get an error and it returns a list of folders and assets similar to this then you are good to go! :tada:
+
+## Features
+
+* stratified sampling for use in Collect Earth Online
+* Training and validation data extraction, from points or polygon references
+* Land cover modeling using Primitive ensembles, complete with model metrics for iterative improvements
+
+## Quick Start
+
+```
+from rlcms.composites import Composite
+# Create an annual Sentinel-1 Composite
+c = Composite(dataset='Sentinel1',
+        region=aoi,
+        start_date='2020-01-01',
+        end_date='2021-12-31',
+        composite_mode='annual',
+        reducer='median')
+
+# look at the Composite object
+print(c.__dict__)
+
+# retrieve band names
+print(f"Composite bands:{c.bands}")
+
+# retrieve ee.Image from Composite object 
+image = c.image
+```
+
+## Contributing
+
+We welcome contributions from the community. If there are issues are improvements, please submit an issue on Github: [https://github.com/sig-gis/rlcms](https://github.com/sig-gis/rlcms)
+
+## License
+
+This project is licensed under the GPL-3 License - see the LICENSE file for details.
+
+
+
```

### Comparing `rlcms-2023.9.7/src/rlcms.egg-info/SOURCES.txt` & `rlcms-2024.5.29/src/rlcms.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 LICENSE
 README.md
 pyproject.toml
 src/rlcms/__init__.py
-src/rlcms/assemblage.py
 src/rlcms/composites.py
 src/rlcms/covariates.py
 src/rlcms/harmonics.py
 src/rlcms/primitives.py
 src/rlcms/sampling.py
 src/rlcms/utils.py
 src/rlcms.egg-info/PKG-INFO
 src/rlcms.egg-info/SOURCES.txt
 src/rlcms.egg-info/dependency_links.txt
 src/rlcms.egg-info/entry_points.txt
 src/rlcms.egg-info/requires.txt
 src/rlcms.egg-info/top_level.txt
-src/rlcms/cli/RFprimitives.py
 src/rlcms/cli/composite.py
-src/rlcms/cli/generate_LC.py
+src/rlcms/cli/landcover.py
+src/rlcms/cli/primitives.py
 src/rlcms/cli/sample_pts.py
 src/rlcms/cli/train_test.py
 tests/test_composites.py
```

### Comparing `rlcms-2023.9.7/tests/test_composites.py` & `rlcms-2024.5.29/tests/test_composites.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from rlcms import composites
-import ee
-import hydrafloods as hf
-ee.Initialize()
-
-# tiny test rect in CA
-region = ee.Geometry.Polygon([[-120.70162384826843,36.658181801020476],
-                               [-120.65218537170593,36.658181801020476],
-                               [-120.65218537170593,36.68461734040718],
-                               [-120.70162384826843,36.68461734040718],
-                               [-120.70162384826843,36.658181801020476]])
-aoi = ee.FeatureCollection("projects/wwf-sig/assets/kaza-lc/aoi/testSeshekeWater")#.geometry()
-start_date = '2021-01-01'
-end_date='2021-12-31'
-
-# class TestComposites:
-def test_composite_bands():
-  
-  # default behavior of composite() is annual mean composite
-  composite = composites.composite(dataset='Sentinel2',
-                                region=aoi,
-                                start_date=start_date,
-                                end_date=end_date)
-  assert composite.bands == ['blue_mean','green_mean','red_mean',
-                                            'nir_mean','swir1_mean','swir2_mean']
-def test_composite_values():
-  composite = composites.composite(dataset='Sentinel2',
-                                region=region,
-                                start_date=start_date,
-                                end_date=end_date)
-  points = ee.FeatureCollection.randomPoints(region,2)
-  comparison_pts = composite.image.sampleRegions(collection=points,scale=10)
-  
-  assert comparison_pts.aggregate_array('blue_mean').getInfo() == [363.6774193548387, 655.3863636363636]
-
-test_composite_bands()
-test_composite_values()
-
-
-
-
-
+from rlcms import composites
+import ee
+import hydrafloods as hf
+ee.Initialize()
+
+# tiny test rect in CA
+region = ee.Geometry.Polygon([[-120.70162384826843,36.658181801020476],
+                               [-120.65218537170593,36.658181801020476],
+                               [-120.65218537170593,36.68461734040718],
+                               [-120.70162384826843,36.68461734040718],
+                               [-120.70162384826843,36.658181801020476]])
+aoi = ee.FeatureCollection("projects/wwf-sig/assets/kaza-lc/aoi/testSeshekeWater")#.geometry()
+start_date = '2021-01-01'
+end_date='2021-12-31'
+
+# class TestComposites:
+def test_composite_bands():
+  
+  # default behavior of composite() is annual mean composite
+  composite = composites.composite(dataset='Sentinel2',
+                                region=aoi,
+                                start_date=start_date,
+                                end_date=end_date)
+  assert composite.bands == ['blue_mean','green_mean','red_mean',
+                                            'nir_mean','swir1_mean','swir2_mean']
+def test_composite_values():
+  composite = composites.composite(dataset='Sentinel2',
+                                region=region,
+                                start_date=start_date,
+                                end_date=end_date)
+  points = ee.FeatureCollection.randomPoints(region,2)
+  comparison_pts = composite.image.sampleRegions(collection=points,scale=10)
+  
+  assert comparison_pts.aggregate_array('blue_mean').getInfo() == [363.6774193548387, 655.3863636363636]
+
+test_composite_bands()
+test_composite_values()
+
+
+
+
+
```

