# Comparing `tmp/cryosieve-1.2.4.tar.gz` & `tmp/cryosieve-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryosieve-1.2.4.tar", last modified: Wed Jan 24 14:43:09 2024, max compression
+gzip compressed data, was "cryosieve-1.2.5.tar", last modified: Sat Apr  6 03:50:01 2024, max compression
```

## Comparing `cryosieve-1.2.4.tar` & `cryosieve-1.2.5.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-01-24 14:43:09.100856 cryosieve-1.2.4/
--rw-rw-rw-   0        0        0      246 2023-08-15 12:04:59.000000 cryosieve-1.2.4/AUTHORS
--rw-rw-rw-   0        0        0    35149 2023-08-15 12:04:59.000000 cryosieve-1.2.4/LICENSE
--rw-rw-rw-   0        0        0    60553 2024-01-24 14:43:09.100856 cryosieve-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0    18012 2024-01-18 02:15:54.000000 cryosieve-1.2.4/README.md
--rw-rw-rw-   0        0        0     1278 2024-01-18 02:15:55.000000 cryosieve-1.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-24 14:43:09.100856 cryosieve-1.2.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-01-24 14:43:09.047786 cryosieve-1.2.4/src/
-drwxrwxrwx   0        0        0        0 2024-01-24 14:43:09.085235 cryosieve-1.2.4/src/cryosieve/
--rw-rw-rw-   0        0        0     6215 2024-01-18 02:15:55.000000 cryosieve-1.2.4/src/cryosieve/ParticleDataset.py
--rw-rw-rw-   0        0        0      247 2023-08-22 11:31:28.000000 cryosieve-1.2.4/src/cryosieve/__init__.py
--rw-rw-rw-   0        0        0     4388 2023-08-22 11:31:28.000000 cryosieve-1.2.4/src/cryosieve/__main__.py
--rw-rw-rw-   0        0        0     4672 2024-01-18 02:15:55.000000 cryosieve-1.2.4/src/cryosieve/core.py
--rw-rw-rw-   0        0        0     6045 2023-08-15 12:04:59.000000 cryosieve-1.2.4/src/cryosieve/kernels.py
--rw-rw-rw-   0        0        0     1554 2024-01-18 02:15:55.000000 cryosieve-1.2.4/src/cryosieve/sieve.py
--rw-rw-rw-   0        0        0     1114 2023-08-15 12:04:59.000000 cryosieve-1.2.4/src/cryosieve/utility.py
-drwxrwxrwx   0        0        0        0 2024-01-24 14:43:09.100856 cryosieve-1.2.4/src/cryosieve.egg-info/
--rw-rw-rw-   0        0        0    60553 2024-01-24 14:43:09.000000 cryosieve-1.2.4/src/cryosieve.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      444 2024-01-24 14:43:09.000000 cryosieve-1.2.4/src/cryosieve.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-24 14:43:09.000000 cryosieve-1.2.4/src/cryosieve.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2024-01-24 14:43:09.000000 cryosieve-1.2.4/src/cryosieve.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       65 2024-01-24 14:43:09.000000 cryosieve-1.2.4/src/cryosieve.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-01-24 14:43:09.000000 cryosieve-1.2.4/src/cryosieve.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:50:01.315893 cryosieve-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-06 03:49:46.000000 cryosieve-1.2.5/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-06 03:49:46.000000 cryosieve-1.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    63573 2024-04-06 03:50:01.315893 cryosieve-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21986 2024-04-06 03:49:46.000000 cryosieve-1.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-06 03:49:46.000000 cryosieve-1.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 03:50:01.315893 cryosieve-1.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:50:01.311893 cryosieve-1.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:50:01.315893 cryosieve-1.2.5/src/cryosieve/
+-rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-04-06 03:49:46.000000 cryosieve-1.2.5/src/cryosieve/ParticleDataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 03:49:46.000000 cryosieve-1.2.5/src/cryosieve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-04-06 03:49:46.000000 cryosieve-1.2.5/src/cryosieve/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-04-06 03:49:46.000000 cryosieve-1.2.5/src/cryosieve/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8033 2024-04-06 03:49:46.000000 cryosieve-1.2.5/src/cryosieve/cs_refine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-04-06 03:49:46.000000 cryosieve-1.2.5/src/cryosieve/cs_rhbfactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-04-06 03:49:46.000000 cryosieve-1.2.5/src/cryosieve/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-06 03:49:46.000000 cryosieve-1.2.5/src/cryosieve/sieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-06 03:49:46.000000 cryosieve-1.2.5/src/cryosieve/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:50:01.315893 cryosieve-1.2.5/src/cryosieve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    63573 2024-04-06 03:50:01.000000 cryosieve-1.2.5/src/cryosieve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-06 03:50:01.000000 cryosieve-1.2.5/src/cryosieve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 03:50:01.000000 cryosieve-1.2.5/src/cryosieve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-06 03:50:01.000000 cryosieve-1.2.5/src/cryosieve.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-06 03:50:01.000000 cryosieve-1.2.5/src/cryosieve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-06 03:50:01.000000 cryosieve-1.2.5/src/cryosieve.egg-info/top_level.txt
```

### Comparing `cryosieve-1.2.4/LICENSE` & `cryosieve-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cryosieve-1.2.4/PKG-INFO` & `cryosieve-1.2.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,980 +1,1038 @@
-Metadata-Version: 2.1
-Name: cryosieve
-Version: 1.2.4
-Summary: CryoSieve: a particle sorting and sieving algorithm for single particle analysis in cryo-EM
-Author-email: Jianying Zhu <zhu-jy20@mails.tsinghua.edu.cn>, Qi Zhang <q-zhang20@mails.tsinghua.edu.cn>, Hui Zhang <zhanghui198@mails.ucas.ac.cn>, Zuoqiang Shi <zqshi@tsinghua.edu.cn>, Mingxu Hu <humingxu@mail.tsinghua.edu.cn>, Chenglong Bao <clbao@tsinghua.edu.cn>
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
-Project-URL: Homepage, https://github.com/mxhulab/cryosieve
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Environment :: GPU :: NVIDIA CUDA
-Classifier: Topic :: Scientific/Engineering :: Image Processing
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS
-Requires-Dist: numpy>=1.18
-Requires-Dist: mrcfile>=1.2
-Requires-Dist: starfile<0.5,>=0.4
-Requires-Dist: cupy>=10
-Requires-Dist: torch>=1.10
-
-![featured image](featured_image.jpg)
-
-# CryoSieve Overview
-
-CryoSieve is an advanced software solution designed for particle sorting/sieving in single particle analysis (SPA) for Cryogenic Electron Microscopy (cryo-EM). Supported by extensive experimental results, CryoSieve has demonstrated superior performance and efficiency compared to other cryo-EM particle sorting algorithms.
-
-Its unique ability to eliminate unnecessary particles from final stacks significantly optimizes the data analysis process. The refined selection of particles that remain contribute to a notably higher resolution output in reconstructed density maps.
-
-For certain datasets, the precision of CryoSieve's particle subset selection is so refined that it approaches the theoretical limit, delivering unprecedented detail and accuracy.
-
-## Video Tutorial
-
-A video tutorial is available within this repository. You can directly download it [here](cryosieve_video_tutorial.mp4).
-
-## Publications
-
-For more details, please refer to the paper ["A minority of final stacks yields superior amplitude in single-particle cryo-EM"](https://www.nature.com/articles/s41467-023-43555-x). If you find that CryoSieve contributes to your work, we kindly request you to cite this paper.
-
-## The List of Available Demo Cases
-
-| dataset | number of particles | molecular weight (kDa) | EMPIAR link | expected result link
-| ------- | ------------------- | --------------------- | ----------- | --------------- |
-| TRPA1 | 43,585 | 688 | [EMPIAR-10024](https://www.ebi.ac.uk/empiar/EMPIAR-10024/) | [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-10024) |
-| hemagglutinin | 130,000 | 150 | [EMPIAR-10097](https://www.ebi.ac.uk/empiar/EMPIAR-10097/) | [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-10097) |
-| LAT1 | 250,712 | 172 | [EMPIAR-10264](https://www.ebi.ac.uk/empiar/EMPIAR-10264/) | [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-10264) |
-| pfCRT | 16,905 | 102 | [EMPIAR-10330](https://www.ebi.ac.uk/empiar/EMPIAR-10330/) | [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-10330) |
-| TSHR-Gs | 41,054 | 125 | [EMPIAR-11120](https://www.ebi.ac.uk/empiar/EMPIAR-11120/) | [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-11120) |
-| TRPM8 | 42,040 | 513 | [EMPIAR-11233](https://www.ebi.ac.uk/empiar/EMPIAR-11233/) | [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-11233) |
-| apoferritin | 382,391 | 440 | [EMPIAR-10200](https://www.ebi.ac.uk/empiar/EMPIAR-10200/) | [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-10200) |
-| streptavidin | 23,991 | 52 | [EMPIAR-10269](https://www.ebi.ac.uk/empiar/EMPIAR-10269/)  | [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-10269) |
-
-![main figure](main_figure.png)
-
-# Installation
-
-CryoSieve is an open-source software, developed using Python, and is available as a Python package. You can access our source code [on GitHub](https://github.com/mxhulab/cryosieve).
-
-## Prerequisites
-
-- Python version 3.7 or later.
-- NVIDIA CUDA library installed in the user's environment.
-
-## Dependencies
-
-The CryoSieve package depends on the following libraries:
-
-```
-numpy>=1.18
-mrcfile>=1.2
-starfile>=0.4,<0.5
-cupy>=10
-torch>=1.10
-```
-
-## Preparation of CUDA Environment
-
-We recommend you install CuPy and PyTorch initially, as their installation largely depends on your CUDA environment. Please note, your PyTorch package should be CUDA-capable.
-
-To streamline this process, we suggest preparing a conda environment with the following command:
-```
-conda create -n CRYOSIEVE_ENV python=3.10 cupy=10.2 cudatoolkit=10.2 pytorch=1.12.1=py3.10_cuda10.2_cudnn7.6.5_0 -c conda-forge -c pytorch
-```
-
-This command is specifically for a CUDA environment version 10.2. If your CUDA environment is higher than 10.2, adjust the command based on the suitable variants and versions recommended by the [CuPy](https://cupy.dev) and [PyTorch](https://pytorch.org) developers for your specific CUDA environment.
-
-## Installing CryoSieve
-
-After preparing CuPy and PyTorch according to your CUDA environment, it is crucial to activate it before proceeding with the CryoSieve installation.
-
-We recommend using the following command to activate it directly. (replace CRYOSIEVE_ENV with the name of your custom environment).
-
-```
-conda activate CRYOSIEVE_ENV
-```
-
-Then, we turn to the step of installing CryoSieve. CryoSieve can be installed either via `pip` or `conda`.
-
-To install CryoSieve using `pip`, execute the following command:
-
-```
-pip install cryosieve
-```
-
-Alternatively, to install CryoSieve using `conda`, execute the following command:
-
-```
-conda install -c mxhulab cryosieve
-```
-
-## Verifying Installation
-
-You can verify whether CryoSieve has been installed successfully by running the following command:
-
-```
-cryosieve -h
-```
-
-This should display the help information for CryoSieve, indicating a successful installation.
-
-# Tutorial
-
-## Quickstart: A Toy Example
-
-To validate your successful installation of CryoSieve and familiarize yourself with its functionalities, we highly recommend trying CryoSieve on this [toy example](https://github.com/mxhulab/cryosieve-demos/tree/master/toy). Please follow the steps below:
-
-1. Download the dataset and place it into any directory of your choice, e.g., `~/toy/`.
-2. Navigate to this directory by executing the following command:
-```
-cd ~/toy/
-```
-3. Initiate CryoSieve with the following command:
-```
-cryosieve-core --i CNG.star --o my_CNG_1.star --angpix 1.32 --volume CNG_A.mrc --volume CNG_B.mrc --mask CNG_mask.mrc --retention_ratio 0.8 --frequency 40
-```
-You may find explanation for each option of `cryosieve-core` [in the following section](#cryosieve-core).
-
-When the `--num_gpus` parameter is used with a value larger than 1, CryoSieve's core program will leverage multiple GPUs to expedite the sieving process. It accomplishes this by using PyTorch's [elastic launch](https://pytorch.org/docs/1.10/elastic/run.html?highlight=torchrun) feature to initiate multiple processes. Each of these processes will use exactly one GPU.
-
-For instance, on a machine equipped with 4 GPUs, you can use the following command to run the toy example:
-```
-cryosieve-core --i CNG.star --o my_CNG_1.star --angpix 1.32 --volume CNG_A.mrc --volume CNG_B.mrc --mask CNG_mask.mrc --retention_ratio 0.8 --frequency 40 --num_gpus 4
-```
-
-Upon successful execution, the command will generate two star files, `my_CNG_1.star` and `my_CNG_1_sieved.star`. These files contain the information of the remaining particles and the sieved particles, respectively. You can compare them with the provided `CNG_1.star` and `CNG_1_sieved.star` files. If executed correctly, they should contain the same particles.
-
-## Processing Real-World Dataset
-
-In this section, we provide a hands-on example of how to utilize CryoSieve for processing the final stack in a real-world experimental dataset.
-
-### Download the Dataset
-
-For this tutorial, we'll be using the final particle stack from the [EMPIAR-11233](https://www.ebi.ac.uk/empiar/EMPIAR-11233/) dataset. This dataset includes a final particle stack of TRPM8 bound to calcium, collected on a 300 kV FEI Titan Krios microscope.
-
-To download the final particle stack, navigate to your desired working directory and execute the following command:
-
-```
-wget -nH -m ftp://ftp.ebi.ac.uk/empiar/world_availability/11233/data/Final_Particle_Stack/
-```
-
-Upon completion, you'll find a new directory named `XXX/data/Final_Particle_Stack` in your working directory. This directory contains a star file with all particle information and an mrcs file representing the final stack.
-
-Additionally, you'll need a mask file. You can generate a mask file using any cryo-EM software, based on the reconstructed volume. If you prefer not to generate a mask file, we've provided one used in our experiments which you can download from this [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-11233). Once you have the mask file, move it into the `Final_Particle_Stack` directory.
-
-You can find additional demonstration data, along with expected results, in [this repository](https://github.com/mxhulab/cryosieve-demos/tree/master).
-
-### Iterative Reconstruction and Sieving
-
-To achieve optimal results with real-world datasets, the sieving process generally involves several iterations. In each iteration, we perform 3D reconstruction (and perhaps postprocessing to derive the Fourier Shell Correlation (FSC) curve and resolution). We then apply CryoSieve to sieve a fraction of the particles based on the reconstructed map. The highpass cut-off frequency typically increases with each round.
-
-For your convenience, we've developed an automatic command `cryosieve` which performs all these steps in a single run. To use it, please follow these steps:
-
-1. Change the working directory to `XXX/data/Final_Particle_Stack`:
-```
-cd XXX/data/Final_Particle_Stack
-```
-2. Our automatic program currently uses Relion for 3D reconstruction and postprocessing. Therefore, make sure that `relion_reconstruct` or `relion_reconstruct_mpi` and `relion_postprocess` are accessible. Once confirmed, run the following command:
-```
-cryosieve --reconstruct_software relion_reconstruct --postprocess_software relion_postprocess --i diver2019_pmTRPM8_calcium_Krios_6Feb18_finalParticleStack_EMPIAR_composite.star --o output/ --mask mask.mrc --angpix 1.059 --num_iters 10 --frequency_start 40 --frequency_end 3 --retention_ratio 0.8 --sym C4
-```
-
-For a detailed explanation of each `cryosieve` option, please refer to the following section [Options/Arguments of `cryosieve`](#cryosieve).
-
-The entire process may take over an hour, depending on your system resources. Multiple result files will be generated and saved in the `output/` directory. For instance, the `_iter{n}.star` file contains particles that remain after the n-th sieving iteration, and the `_postprocess_iter{n}` folder houses the postprocessing result after the n-th iteration.
-
-### [Recommended] Re-estimate poses by CryoSPARC
-
-The objective of re-estimating poses using CryoSPARC is to prevent the unintentional transfer of information from the discarded particles to those that are retained. This process of re-estimating poses with CryoSPARC can be conducted either manually or through automation using a Python script. The script, named `cryosieve_auto_cryosparc.py`, is provided by us in this repository.
-
-For manually re-estimating poses with CryoSPARC, particles must be imported using CryoSPARC’s `import particle stack` job. This importation is from the `_iter{n}.star` file, which contains particles remaining after the n-th sieving iteration. Subsequently, the process involves conducting sequential `ab-initio` jobs, followed by either `homogeneous refinement` or `non-uniform refinement` jobs.
-
-Alternatively, users can utilize the `cryosieve_auto_cryosparc.py` script, available in this repository, to circumvent the labor-intensive manual operations in CryoSPARC. The prerequisite for executing the `cryosieve_auto_cryosparc.py` script is the loading of CryoSPARC’s environment variables. This can be accomplished by executing the command `eval $(cryosparcm env)` in the shell. The successful loading of this environment can be verified by using the `which python` command. Upon successful execution, this command should point to a Python interpreter located within CryoSPARC’s installation path. Utilizing this Python interpreter, users can execute the `cryosieve_auto_cryosparc.py` script to automatically and sequentially carry out `import particle stack`, `ab-initio`, `homogenous refinement`, and `non-uniform refinement` jobs. These operations are performed for each particle stack listed in a sheet, which is provided as an argument to the `cryosieve_auto_cryosparc.py` script. For a detailed explanation of each `cryosieve_auto_cryosparc.py` option, please refer to the following section [Options/Arguments of `cryosieve_auto_cryosparc.py`](#cryosieve_auto_cryosparc).
-
-# Options/Arguments of `cryosive-core`, `cryosieve` and `cryosieve_auto_cryosparc.py`
-
-<a name="cryosieve-core"></a>
-## Options/Arguments of `cryosieve-core`
-
-The program `cryosieve-core` is the core particle sieving module.
-
-```
-$ cryosieve-core -h
-usage: cryosieve-core [-h] --i I --o O [--directory DIRECTORY] --angpix ANGPIX --volume VOLUME [--mask MASK] [--retention_ratio RETENTION_RATIO] --frequency
-                      FREQUENCY [--balance] [--num_gpus NUM_GPUS]
-
-CryoSieve core.
-
-options:
-  -h, --help            show this help message and exit
-  --i I                 input star file path.
-  --o O                 output star file path.
-  --directory DIRECTORY
-                        directory of particles, empty (current directory) by default.
-  --angpix ANGPIX       pixelsize in Angstrom.
-  --volume VOLUME       list of volume file paths.
-  --mask MASK           mask file path.
-  --retention_ratio RETENTION_RATIO
-                        fraction of retained particles, 0.8 by default.
-  --frequency FREQUENCY
-                        cut-off highpass frequency.
-  --balance             make retained particles in different subsets in same size.
-  --num_gpus NUM_GPUS   number of GPUs to execute the cryosieve program, 1 by default.
-```
-
-<a name="cryosieve"></a>
-## Options/Arguments of `cryosieve`
-
-The program `cryosieve` is an integreted program iteratively calling relion and `cryosieve-core` to do sieving process.
-
-```
-$ cryosieve -h
-usage: cryosieve [-h] --reconstruct_software RECONSTRUCT_SOFTWARE [--postprocess_software POSTPROCESS_SOFTWARE] --i I --o O --angpix ANGPIX [--sym SYM]
-                 [--num_iters NUM_ITERS] [--frequency_start FREQUENCY_START] [--frequency_end FREQUENCY_END] [--retention_ratio RETENTION_RATIO] --mask MASK
-                 [--balance] [--num_gpus NUM_GPUS]
-
-CryoSieve: a particle sorting and sieving software for single particle analysis in cryo-EM.
-
-options:
-  -h, --help            show this help message and exit
-  --reconstruct_software RECONSTRUCT_SOFTWARE
-                        command for reconstruction.
-  --postprocess_software POSTPROCESS_SOFTWARE
-                        command for postprocessing.
-  --i I                 input star file path.
-  --o O                 output path prefix.
-  --angpix ANGPIX       pixelsize in Angstrom.
-  --sym SYM             molecular symmetry, c1 by default.
-  --num_iters NUM_ITERS
-                        number of iterations for applying CryoSieve, 10 by default.
-  --frequency_start FREQUENCY_START
-                        starting threshold frquency, in Angstrom, 50A by default.
-  --frequency_end FREQUENCY_END
-                        ending threshold frquency, in Angstrom, 3A by default.
-  --retention_ratio RETENTION_RATIO
-                        fraction of retained particles in each iteration, 0.8 by default.
-  --mask MASK           mask file path.
-  --balance             make remaining particles in different subsets in same size.
-  --num_gpus NUM_GPUS   number of gpus to execute CryoSieve core program, 1 by default.
-```
-
-There are several useful remarks:
-
-- CryoSieve utilizes the `RECONSTRUCT_SOFTWARE` in its reconstruction command. This enables you to enhance the speed of the reconstruction step through multiprocessing by using the option `--reconstruct_software "mpirun -n 5 relion_reconstruct_mpi"`. Additionally, you can further boost the reconstruction speed by using the option `--reconstruct_software "mpirun -n 5 relion_reconstruct_mpi --j 20"`, leveraging multi-threading.
-- If POSTPROCESS_SOFTWARE is not given, CryoSieve will skip the postprocessing step. Notice that postprocessing is not necessary for the sieving procedure.
-- Since `relion_reconstruct` use current directory as its default working directory, user should ensure that `relion_reconstruct` can correctly access the particles.
-
-<a name="cryosieve_auto_cryosparc"></a>
-## Options/Arguments of `cryosieve_auto_cryosparc.py`
-
-The `cryosieve_auto_cryosparc.py` is a Python script designed to automatically and sequentially execute a series of operations in CryoSPARC, namely `import particle stack`, `ab-initio`, `homogenous refinement`, and `non-uniform refinement` jobs.
-
-```
-usage: cryosieve_auto_cryosparc.py [-h] [--particles_sheet PARTICLES_SHEET] [--cryosparc_user_id CRYOSPARC_USER_ID]
-                                   [--cryosparc_project_uid CRYOSPARC_PROJECT_UID] [--cryosparc_workspace_uid CRYOSPARC_WORKSPACE_UID]
-                                   [--cryosparc_lane CRYOSPARC_LANE] [--molecular_symmetry MOLECULAR_SYMMETRY]
-
-The cryosieve_auto_cryosparc.py is a Python script designed to automate CryoSPARC operations via the command line. Its purpose is to
-bypass the labor-intensive manual processes.
-
-options:
-  -h, --help            show this help message and exit
-  --particles_sheet PARTICLES_SHEET
-                        a file containing a list of starfiles; each starfile corresponds to a single-particle dataset; NOTE, absolute
-                        directory is mandatory
-  --cryosparc_user_id CRYOSPARC_USER_ID
-                        the E-mail address of the user of CryoSPARC
-  --cryosparc_project_uid CRYOSPARC_PROJECT_UID
-                        the project UID in cryoSPARC
-  --cryosparc_workspace_uid CRYOSPARC_WORKSPACE_UID
-                        the workspace UID in cryoSPARC
-  --cryosparc_lane CRYOSPARC_LANE
-                        the lane for computing resource in cryoSPARC
-  --molecular_symmetry MOLECULAR_SYMMETRY
-                        molecular symmetry
-```
-
-# Release Note
-
-* Version 1.2.4:
-  - Fix the bug occurring with starfile >=0.5. CryoSieve now requires starfile >=0.4, <0.5.
-  - Support gloo backend for multi-GPU version of cryosieve-core.
-  - Fix the bug of SequentialSampler occurring with pytorch >=2.
-* Version 1.2.3: Add new video tutorial.
-* Version 1.2.1: fix the bug occurring when multiple optic groups are present in a star file.
-* Version 1.2: Initial stable release.
+Metadata-Version: 2.1
+Name: cryosieve
+Version: 1.2.5
+Summary: CryoSieve: a particle sorting and sieving algorithm for single particle analysis in cryo-EM
+Author-email: Jianying Zhu <zhu-jy20@mails.tsinghua.edu.cn>, Qi Zhang <q-zhang20@mails.tsinghua.edu.cn>, Hui Zhang <zhanghui198@mails.ucas.ac.cn>, Zuoqiang Shi <zqshi@tsinghua.edu.cn>, Mingxu Hu <humingxu@mail.tsinghua.edu.cn>, Chenglong Bao <clbao@tsinghua.edu.cn>
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
+Project-URL: Homepage, https://github.com/mxhulab/cryosieve
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Environment :: GPU :: NVIDIA CUDA
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS
+Requires-Dist: numpy>=1.18
+Requires-Dist: mrcfile>=1.2
+Requires-Dist: starfile<0.5,>=0.4
+Requires-Dist: pandas<2.2
+Requires-Dist: cupy>=10
+Requires-Dist: torch>=1.10
+
+![featured image](featured_image.jpg)
+
+# CryoSieve Overview
+
+CryoSieve is an advanced software solution designed for particle sorting/sieving in single particle analysis (SPA) for Cryogenic Electron Microscopy (cryo-EM). Supported by extensive experimental results, CryoSieve has demonstrated superior performance and efficiency compared to other cryo-EM particle sorting algorithms.
+
+Its unique ability to eliminate unnecessary particles from final stacks significantly optimizes the data analysis process. The refined selection of particles that remain contribute to a notably higher resolution output in reconstructed density maps.
+
+For certain datasets, the precision of CryoSieve's particle subset selection is so refined that it approaches the theoretical limit, delivering unprecedented detail and accuracy.
+
+## Video Tutorial
+
+A video tutorial is available within this repository. You can directly download it [here](cryosieve_video_tutorial.mp4).
+
+## Publications
+
+For more details, please refer to the paper ["A minority of final stacks yields superior amplitude in single-particle cryo-EM"](https://www.nature.com/articles/s41467-023-43555-x). If you find that CryoSieve contributes to your work, we kindly request you to cite this paper.
+
+## The List of Available Demo Cases
+
+| dataset | number of particles | molecular weight (kDa) | EMPIAR link | expected result link
+| ------- | ------------------- | --------------------- | ----------- | --------------- |
+| TRPA1 | 43,585 | 688 | [EMPIAR-10024](https://www.ebi.ac.uk/empiar/EMPIAR-10024/) | [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-10024) |
+| hemagglutinin | 130,000 | 150 | [EMPIAR-10097](https://www.ebi.ac.uk/empiar/EMPIAR-10097/) | [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-10097) |
+| LAT1 | 250,712 | 172 | [EMPIAR-10264](https://www.ebi.ac.uk/empiar/EMPIAR-10264/) | [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-10264) |
+| pfCRT | 16,905 | 102 | [EMPIAR-10330](https://www.ebi.ac.uk/empiar/EMPIAR-10330/) | [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-10330) |
+| TSHR-Gs | 41,054 | 125 | [EMPIAR-11120](https://www.ebi.ac.uk/empiar/EMPIAR-11120/) | [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-11120) |
+| TRPM8 | 42,040 | 513 | [EMPIAR-11233](https://www.ebi.ac.uk/empiar/EMPIAR-11233/) | [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-11233) |
+| apoferritin | 382,391 | 440 | [EMPIAR-10200](https://www.ebi.ac.uk/empiar/EMPIAR-10200/) | [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-10200) |
+| streptavidin | 23,991 | 52 | [EMPIAR-10269](https://www.ebi.ac.uk/empiar/EMPIAR-10269/)  | [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-10269) |
+
+![main figure](main_figure.png)
+
+# Installation
+
+CryoSieve is an open-source software, developed using Python, and is available as a Python package. Please access our source code [on GitHub](https://github.com/mxhulab/cryosieve).
+
+## Prerequisites
+
+- Python version 3.7 or later.
+- NVIDIA CUDA library 10.2 or later installed in the user's environment.
+
+## Dependencies
+
+The CryoSieve package depends on the following libraries:
+
+```
+numpy>=1.18
+mrcfile>=1.2
+starfile>=0.4,<0.5
+pandans<2.2
+cupy>=10
+torch>=1.10
+```
+
+## Preparation of CUDA Environment
+
+We recommend installing CuPy and PyTorch initially, as their installation largely depends on the CUDA environment. Please note, PyTorch should be CUDA-capable. To streamline this process, we suggest preparing a conda environment with the following commands.
+
+For CUDA version <= 11.7:
+```
+conda create -n CRYOSIEVE_ENV python=3.8 cudatoolkit=10.2 cupy=10.0 pytorch=1.10 -c pytorch -c conda-forge
+```
+Please note that this command is tailored for CUDA version 10.2. To accommodate a different CUDA version, adjust the `cudatoolkit` version accordingly. Modify the versions of Python, CuPy, and PyTorch based on requirements, ensuring compatibility with the minimal requirements of CryoSieve.
+
+For CUDA version >= 11.8:
+```
+conda create -n CRYOSIEVE_ENV python=3.10 cupy=12.0 pytorch pytorch-cuda=12.1 -c pytorch -c nvidia -c conda-forge
+```
+Please note that This command is tailored for CUDA environment version 12.1. For a different CUDA version, adjust `pytorch-cuda` version accordingly.
+
+## Installing CryoSieve
+
+After preparing CuPy and PyTorch, it is crucial to activate it before proceeding with the CryoSieve installation.
+```
+conda activate CRYOSIEVE_ENV
+```
+
+Then, we turn to the step of installing CryoSieve. CryoSieve can be installed either via `pip` or `conda`.
+
+To install CryoSieve using `pip`, execute the following command:
+```
+pip install cryosieve
+```
+Alternatively, to install CryoSieve using `conda`, execute the following command:
+```
+conda install -c mxhulab cryosieve
+```
+
+## Verifying Installation
+
+You can verify whether CryoSieve has been installed successfully by running the following command:
+```
+cryosieve -h
+```
+This should display the help information for CryoSieve, indicating a successful installation.
+
+# Tutorial
+
+## Quickstart: A Toy Example
+
+To validate your successful installation of CryoSieve and familiarize yourself with its functionalities, we highly recommend trying CryoSieve on this [toy example](https://github.com/mxhulab/cryosieve-demos/tree/master/toy). Please follow the steps below:
+
+1. Download the dataset and place it into any directory of your choice, e.g., `~/toy/`.
+2. Navigate to this directory by executing the following command:
+```
+cd ~/toy/
+```
+3. Initiate CryoSieve with the following command:
+```
+cryosieve-core --i CNG.star --o my_CNG_1.star --angpix 1.32 --volume CNG_A.mrc --volume CNG_B.mrc --mask CNG_mask.mrc --retention_ratio 0.8 --frequency 40
+```
+You may find explanation for each option of `cryosieve-core` [in the following section](#cryosieve-core).
+
+When the `--num_gpus` parameter is used with a value larger than 1, CryoSieve's core program will leverage multiple GPUs to expedite the sieving process. It accomplishes this by using PyTorch's [elastic launch](https://pytorch.org/docs/1.10/elastic/run.html?highlight=torchrun) feature to initiate multiple processes. Each of these processes will use exactly one GPU.
+
+For instance, on a machine equipped with 4 GPUs, you can use the following command to run the toy example:
+```
+cryosieve-core --i CNG.star --o my_CNG_1.star --angpix 1.32 --volume CNG_A.mrc --volume CNG_B.mrc --mask CNG_mask.mrc --retention_ratio 0.8 --frequency 40 --num_gpus 4
+```
+
+Upon successful execution, the command will generate two star files, `my_CNG_1.star` and `my_CNG_1_sieved.star`. These files contain the information of the remaining particles and the sieved particles, respectively. You can compare them with the provided `CNG_1.star` and `CNG_1_sieved.star` files. If executed correctly, they should contain the same particles.
+
+## Processing Real-World Dataset
+
+In this section, we provide a hands-on example of how to utilize CryoSieve for processing the final stack in a real-world experimental dataset.
+
+### Download the Dataset
+
+For this tutorial, we'll be using the final particle stack from the [EMPIAR-11233](https://www.ebi.ac.uk/empiar/EMPIAR-11233/) dataset. This dataset includes a final particle stack of TRPM8 bound to calcium, collected on a 300 kV FEI Titan Krios microscope.
+
+To download the final particle stack, navigate to your desired working directory and execute the following command:
+
+```
+wget -nH -m ftp://ftp.ebi.ac.uk/empiar/world_availability/11233/data/Final_Particle_Stack/
+```
+
+Upon completion, you'll find a new directory named `XXX/data/Final_Particle_Stack` in your working directory. This directory contains a star file with all particle information and an mrcs file representing the final stack.
+
+Additionally, you'll need a mask file. You can generate a mask file using any cryo-EM software, based on the reconstructed volume. If you prefer not to generate a mask file, we've provided one used in our experiments which you can download from this [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-11233). Once you have the mask file, move it into the `Final_Particle_Stack` directory.
+
+You can find additional demonstration data, along with expected results, in [this repository](https://github.com/mxhulab/cryosieve-demos/tree/master).
+
+### Iterative Reconstruction and Sieving
+
+To achieve optimal results with real-world datasets, the sieving process generally involves several iterations. In each iteration, we perform 3D reconstruction (and perhaps postprocessing to derive the Fourier Shell Correlation (FSC) curve and resolution). We then apply CryoSieve to sieve a fraction of the particles based on the reconstructed map. The highpass cut-off frequency typically increases with each round.
+
+For your convenience, we've developed an automatic command `cryosieve` which performs all these steps in a single run. To use it, please follow these steps:
+
+1. Change the working directory to `XXX/data/Final_Particle_Stack`:
+```
+cd XXX/data/Final_Particle_Stack
+```
+2. Our automatic program currently uses Relion for 3D reconstruction and postprocessing. Therefore, make sure that `relion_reconstruct` or `relion_reconstruct_mpi` and `relion_postprocess` are accessible. Once confirmed, run the following command:
+```
+cryosieve --reconstruct_software relion_reconstruct --postprocess_software relion_postprocess --i diver2019_pmTRPM8_calcium_Krios_6Feb18_finalParticleStack_EMPIAR_composite.star --o output/ --mask mask.mrc --angpix 1.059 --num_iters 10 --frequency_start 40 --frequency_end 3 --retention_ratio 0.8 --sym C4
+```
+
+For a detailed explanation of each `cryosieve` option, please refer to the following section [Options/Arguments of `cryosieve`](#cryosieve).
+
+The entire process may take over an hour, depending on your system resources. Multiple result files will be generated and saved in the `output/` directory. For instance, the `_iter{n}.star` file contains particles that remain after the n-th sieving iteration, and the `_postprocess_iter{n}` folder houses the postprocessing result after the n-th iteration.
+
+### [Recommended] Re-estimate poses
+
+The objective of re-estimating poses is to prevent the unintentional transfer of information from the discarded particles to those that are retained. This process of re-estimating poses with CryoSPARC can be performed manually or automated using a Python module. We provide a Python script named `cryosieve-csrefine` in this repository for this purpose.
+
+For manually re-estimating poses with CryoSPARC, particles must be imported using CryoSPARC’s `import particle stack` job. This importation is from the `_iter{n}.star` file, which contains particles remaining after the n-th sieving iteration. Subsequently, the process involves conducting sequential `ab-initio` jobs, followed by either `homogeneous refinement` or `non-uniform refinement` jobs.
+
+Alternatively, users can utilize the `cryosieve-csrefine` command, available in this repository, to streamline the labor-intensive manual operations in CryoSPARC. This script automates the sequential execution of `import particle stack`, `ab-initio`, `homogenous refinement` or `non-uniform refinement` jobs for each input particle stack. Additionally, it generates a summary of resolutions and B-factors. For a detailed explanation of each option available in `cryosieve-csrefine`, please refer to the following section [Options/Arguments of `cryosieve-csrefine`](#cryosieve-csrefine).
+
+### [Optional] Calculate the Rosenthal-Henderson B-factor
+
+The gold standard for assessing the quality of a set of single particle images involves determining its Rosenthal-Henderson B-factor. A lower B-factor indicates better quality. Utilizing CryoSieve to filter out ineffective particles can reduce the B-factor, suggesting improved quality among the remaining particles. Users can leverage the `cryosieve-csrhbfactor` command to automatically calculate the Rosenthal-Henderson B-factor by CryoSPARC. The script's arguments/options are similar to those in `cryosieve-csrhbfactor`. For a detailed explanation of each `cryosieve-csrhbfactor` option, please refer to the following section [Options/Arguments of `cryosieve-csrhbfactor`](#cryosieve-csrhbfactor).
+
+# Options/Arguments
+
+<a name="cryosieve-core"></a>
+## Options/Arguments of `cryosieve-core`
+
+The program `cryosieve-core` is the core particle sieving module.
+
+```
+$ cryosieve-core -h
+usage: cryosieve-core [-h] --i I --o O [--directory DIRECTORY] --angpix ANGPIX --volume VOLUME [--mask MASK] [--retention_ratio RETENTION_RATIO] --frequency
+                      FREQUENCY [--balance] [--num_gpus NUM_GPUS]
+
+CryoSieve core.
+
+options:
+  -h, --help            show this help message and exit
+  --i I                 input star file path.
+  --o O                 output star file path.
+  --directory DIRECTORY
+                        directory of particles, empty (current directory) by default.
+  --angpix ANGPIX       pixelsize in Angstrom.
+  --volume VOLUME       list of volume file paths.
+  --mask MASK           mask file path.
+  --retention_ratio RETENTION_RATIO
+                        fraction of retained particles, 0.8 by default.
+  --frequency FREQUENCY
+                        cut-off highpass frequency.
+  --balance             make retained particles in different subsets in same size.
+  --num_gpus NUM_GPUS   number of GPUs to execute the cryosieve program, 1 by default.
+```
+
+<a name="cryosieve"></a>
+## Options/Arguments of `cryosieve`
+
+The program `cryosieve` is an integreted program iteratively calling RELION and `cryosieve-core` to do sieving process.
+
+```
+$ cryosieve -h
+usage: cryosieve [-h] --reconstruct_software RECONSTRUCT_SOFTWARE [--postprocess_software POSTPROCESS_SOFTWARE] --i I --o O --angpix ANGPIX [--sym SYM]
+                 [--num_iters NUM_ITERS] [--frequency_start FREQUENCY_START] [--frequency_end FREQUENCY_END] [--retention_ratio RETENTION_RATIO] --mask MASK
+                 [--balance] [--num_gpus NUM_GPUS]
+
+CryoSieve: a particle sorting and sieving software for single particle analysis in cryo-EM.
+
+options:
+  -h, --help            show this help message and exit
+  --reconstruct_software RECONSTRUCT_SOFTWARE
+                        command for reconstruction.
+  --postprocess_software POSTPROCESS_SOFTWARE
+                        command for postprocessing.
+  --i I                 input star file path.
+  --o O                 output path prefix.
+  --angpix ANGPIX       pixelsize in Angstrom.
+  --sym SYM             molecular symmetry, C1 by default.
+  --num_iters NUM_ITERS
+                        number of iterations for applying CryoSieve, 10 by default.
+  --frequency_start FREQUENCY_START
+                        starting threshold frquency, in Angstrom, 50A by default.
+  --frequency_end FREQUENCY_END
+                        ending threshold frquency, in Angstrom, 3A by default.
+  --retention_ratio RETENTION_RATIO
+                        fraction of retained particles in each iteration, 0.8 by default.
+  --mask MASK           mask file path.
+  --balance             make remaining particles in different subsets in same size.
+  --num_gpus NUM_GPUS   number of gpus to execute CryoSieve core program, 1 by default.
+```
+
+There are several useful remarks:
+
+- CryoSieve utilizes the `RECONSTRUCT_SOFTWARE` in its reconstruction command. This enables you to enhance the speed of the reconstruction step through multiprocessing by using the option `--reconstruct_software "mpirun -n 5 relion_reconstruct_mpi"`. Additionally, you can further boost the reconstruction speed by using the option `--reconstruct_software "mpirun -n 5 relion_reconstruct_mpi --j 20"`, leveraging multi-threading.
+- If `POSTPROCESS_SOFTWARE` is not given, CryoSieve will skip the postprocessing step. Notice that postprocessing is not necessary for the sieving procedure.
+- Since `relion_reconstruct` use current directory as its default working directory, user should ensure that `relion_reconstruct` can correctly access the particles.
+
+<a name="cryosieve-csrefine"></a>
+## Options/Arguments of `cryosieve-csrefine`
+
+The program `cryosieve-csrefine` is designed to automatically and sequentially execute a series of operations in CryoSPARC, namely `import particle stack`, `ab-initio`, `homogenous refinement` or `non-uniform refinement` jobs.
+
+```
+$ cryosieve-csrefine -h
+usage: cryosieve-csrefine [-h] [--i I [I ...]] [--directory DIRECTORY] [--o O] [--sym SYM] [--ref REF] [--repeat REPEAT] --user USER
+                          --project PROJECT --workspace WORKSPACE --lane LANE [--nu] [--resplit] [--workers WORKERS]
+
+cryosieve-csrefine: automatic SPA 3D-refinement by calling CryoSPARC.
+
+options:
+  -h, --help            show this help message and exit
+  --i I [I ...]         input star file(s) or txt file(s) containing a list of star files.
+  --directory DIRECTORY
+                        directory of particles, empty (current directory) by default.
+  --o O                 output summary csv file path. If not provided, no summary is written.
+  --sym SYM             molecular symmetry, C1 by default.
+  --ref REF             initial reference model. If not provided, CryoSPARC's ab-initio job will be used.
+  --repeat REPEAT       number of trials, 1 by default.
+  --user USER           e-mail address of the user of CryoSPARC.
+  --project PROJECT     project UID in CryoSPARC.
+  --workspace WORKSPACE
+                        workspace UID in CryoSPARC.
+  --lane LANE           lane selected for computing in CryoSPARC.
+  --nu                  use non-uniform refinement.
+  --resplit             force re-do GS split.
+  --workers WORKERS     number of workers to run CryoSPARC job, unlimited by default.
+```
+
+There are several useful remarks:
+
+- The input parameter `--i` supports multiple star files, such as `--i a.star b.star c.star`. Wildcards can also be used, for example, `--i output/_iter?.star` will include `output/_iter0.star`, `output/_iter1.star` up to `output/_iter9.star` in the previous example. Additionally, the input file can be a `.txt` file containing star files, with each file listed on a separate line.
+- When the `--o` parameter is provided, a summary report including resolutions and B-factors estimated by CryoSPARC will be written to a file in CSV format.
+- This program submits a series of jobs within a designated project and workspace. The compute resources are determined by the lane parameter. By default, the program refines all star files in parallel, but the option `--workers` allows you to limit the number of jobs executing simultaneously.
+
+For example, in the previous EMPAIR-11233 case, you can re-estimated all its output star files with a single command:
+```
+cryosieve-csrefine --i output/_iter?.star --o summary.csv --sym C4 --user XXX_YOUR_USER_EMAIL_XXX --project P1 --workspace W1 --lane XXX_YOUR_LANE_XXX
+```
+
+<a name="cryosieve-csrhbfactor"></a>
+## Options/Arguments of `cryosieve-csrhbfactor`
+
+The program `cryosieve-csrhbfactor` is designed to automatically determine Rosenthal-Henderson B-factor by calling `cryosieve-csrefine`.
+
+```
+$ cryosieve-csrhbfactor -h
+usage: cryosieve-csrhbfactor [-h] [--i I [I ...]] [--directory DIRECTORY] --o O [--sym SYM] [--ref REF] [--voltage VOLTAGE]
+                             [--repeat REPEAT] [--halves HALVES] --user USER --project PROJECT --workspace WORKSPACE --lane LANE [--nu]
+                             [--resplit] [--workers WORKERS]
+
+cryosieve-csrhbfactor: automatic Rosenthal-Henderson B-factor estimation by calling CryoSPARC.
+
+options:
+  -h, --help            show this help message and exit
+  --i I [I ...]         input star file(s) or txt file(s) containing a list of star files.
+  --directory DIRECTORY
+                        directory of particles, empty (current directory) by default.
+  --o O                 output summary csv file path.
+  --sym SYM             molecular symmetry, C1 by default.
+  --ref REF             initial reference model. If not provided, CryoSPARC's ab-initio job will be used.
+  --voltage VOLTAGE     acceleration voltage (kV), 300 by default. Only 200 and 300 supported!
+  --repeat REPEAT       number of trials, 1 by default.
+  --halves HALVES       number of times executing halvings, 4 by default.
+  --user USER           e-mail address of the user of CryoSPARC.
+  --project PROJECT     project UID in CryoSPARC.
+  --workspace WORKSPACE
+                        workspace UID in CryoSPARC.
+  --lane LANE           lane selected for computing in CryoSPARC.
+  --nu                  use non-uniform refinement.
+  --resplit             force re-do GS split.
+  --workers WORKERS     number of workers to run CryoSPARC job, unlimited by default.
+```
+
+There are several useful remarks:
+
+- The `cryosieve-csrhbfactor` program shares most parameters with `cryosieve-csrefine`, and their usage is similar.
+- Estimating the Rosenthal-Henderson B-factor involves a computationally intensive process. It requires iteratively halving the particle dataset and estimating the resolutions for each subset. For example, if you want to estimate the Rosenthal-Henderson B-factors for all 10 output stacks from the previous demo, and you choose to perform 3 trials with each stack using up to 4th halves, it would involve a total of 10 * 3 * (4 + 1) = 150 rounds of 3D-refinement.
+
+# Release Note
+
+* Version 1.2.5:
+  - Add two new programs: `cryosieve-csrefine` and `cryosieve-csrhbfactor`.
+  - Introduce a simplified command for preparing the Conda environment.
+  - Add support for CUDA >=11.8.
+* Version 1.2.4:
+  - Fix the bug occurring with starfile >=0.5. CryoSieve now requires starfile >=0.4, <0.5.
+  - Support gloo backend for multi-GPU version of cryosieve-core.
+  - Fix the bug of SequentialSampler occurring with pytorch >=2.
+* Version 1.2.3: Add new video tutorial.
+* Version 1.2.1: fix the bug occurring when multiple optic groups are present in a star file.
+* Version 1.2: Initial stable release.
```

### Comparing `cryosieve-1.2.4/README.md` & `cryosieve-1.2.5/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -29,76 +29,74 @@
 | apoferritin | 382,391 | 440 | [EMPIAR-10200](https://www.ebi.ac.uk/empiar/EMPIAR-10200/) | [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-10200) |
 | streptavidin | 23,991 | 52 | [EMPIAR-10269](https://www.ebi.ac.uk/empiar/EMPIAR-10269/)  | [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-10269) |
 
 ![main figure](main_figure.png)
 
 # Installation
 
-CryoSieve is an open-source software, developed using Python, and is available as a Python package. You can access our source code [on GitHub](https://github.com/mxhulab/cryosieve).
+CryoSieve is an open-source software, developed using Python, and is available as a Python package. Please access our source code [on GitHub](https://github.com/mxhulab/cryosieve).
 
 ## Prerequisites
 
 - Python version 3.7 or later.
-- NVIDIA CUDA library installed in the user's environment.
+- NVIDIA CUDA library 10.2 or later installed in the user's environment.
 
 ## Dependencies
 
 The CryoSieve package depends on the following libraries:
 
 ```
 numpy>=1.18
 mrcfile>=1.2
 starfile>=0.4,<0.5
+pandans<2.2
 cupy>=10
 torch>=1.10
 ```
 
 ## Preparation of CUDA Environment
 
-We recommend you install CuPy and PyTorch initially, as their installation largely depends on your CUDA environment. Please note, your PyTorch package should be CUDA-capable.
+We recommend installing CuPy and PyTorch initially, as their installation largely depends on the CUDA environment. Please note, PyTorch should be CUDA-capable. To streamline this process, we suggest preparing a conda environment with the following commands.
 
-To streamline this process, we suggest preparing a conda environment with the following command:
+For CUDA version <= 11.7:
 ```
-conda create -n CRYOSIEVE_ENV python=3.10 cupy=10.2 cudatoolkit=10.2 pytorch=1.12.1=py3.10_cuda10.2_cudnn7.6.5_0 -c conda-forge -c pytorch
+conda create -n CRYOSIEVE_ENV python=3.8 cudatoolkit=10.2 cupy=10.0 pytorch=1.10 -c pytorch -c conda-forge
 ```
+Please note that this command is tailored for CUDA version 10.2. To accommodate a different CUDA version, adjust the `cudatoolkit` version accordingly. Modify the versions of Python, CuPy, and PyTorch based on requirements, ensuring compatibility with the minimal requirements of CryoSieve.
 
-This command is specifically for a CUDA environment version 10.2. If your CUDA environment is higher than 10.2, adjust the command based on the suitable variants and versions recommended by the [CuPy](https://cupy.dev) and [PyTorch](https://pytorch.org) developers for your specific CUDA environment.
+For CUDA version >= 11.8:
+```
+conda create -n CRYOSIEVE_ENV python=3.10 cupy=12.0 pytorch pytorch-cuda=12.1 -c pytorch -c nvidia -c conda-forge
+```
+Please note that This command is tailored for CUDA environment version 12.1. For a different CUDA version, adjust `pytorch-cuda` version accordingly.
 
 ## Installing CryoSieve
 
-After preparing CuPy and PyTorch according to your CUDA environment, it is crucial to activate it before proceeding with the CryoSieve installation.
-
-We recommend using the following command to activate it directly. (replace CRYOSIEVE_ENV with the name of your custom environment).
-
+After preparing CuPy and PyTorch, it is crucial to activate it before proceeding with the CryoSieve installation.
 ```
 conda activate CRYOSIEVE_ENV
 ```
 
 Then, we turn to the step of installing CryoSieve. CryoSieve can be installed either via `pip` or `conda`.
 
 To install CryoSieve using `pip`, execute the following command:
-
 ```
 pip install cryosieve
 ```
-
 Alternatively, to install CryoSieve using `conda`, execute the following command:
-
 ```
 conda install -c mxhulab cryosieve
 ```
 
 ## Verifying Installation
 
 You can verify whether CryoSieve has been installed successfully by running the following command:
-
 ```
 cryosieve -h
 ```
-
 This should display the help information for CryoSieve, indicating a successful installation.
 
 # Tutorial
 
 ## Quickstart: A Toy Example
 
 To validate your successful installation of CryoSieve and familiarize yourself with its functionalities, we highly recommend trying CryoSieve on this [toy example](https://github.com/mxhulab/cryosieve-demos/tree/master/toy). Please follow the steps below:
@@ -158,23 +156,27 @@
 cryosieve --reconstruct_software relion_reconstruct --postprocess_software relion_postprocess --i diver2019_pmTRPM8_calcium_Krios_6Feb18_finalParticleStack_EMPIAR_composite.star --o output/ --mask mask.mrc --angpix 1.059 --num_iters 10 --frequency_start 40 --frequency_end 3 --retention_ratio 0.8 --sym C4
 ```
 
 For a detailed explanation of each `cryosieve` option, please refer to the following section [Options/Arguments of `cryosieve`](#cryosieve).
 
 The entire process may take over an hour, depending on your system resources. Multiple result files will be generated and saved in the `output/` directory. For instance, the `_iter{n}.star` file contains particles that remain after the n-th sieving iteration, and the `_postprocess_iter{n}` folder houses the postprocessing result after the n-th iteration.
 
-### [Recommended] Re-estimate poses by CryoSPARC
+### [Recommended] Re-estimate poses
 
-The objective of re-estimating poses using CryoSPARC is to prevent the unintentional transfer of information from the discarded particles to those that are retained. This process of re-estimating poses with CryoSPARC can be conducted either manually or through automation using a Python script. The script, named `cryosieve_auto_cryosparc.py`, is provided by us in this repository.
+The objective of re-estimating poses is to prevent the unintentional transfer of information from the discarded particles to those that are retained. This process of re-estimating poses with CryoSPARC can be performed manually or automated using a Python module. We provide a Python script named `cryosieve-csrefine` in this repository for this purpose.
 
 For manually re-estimating poses with CryoSPARC, particles must be imported using CryoSPARC’s `import particle stack` job. This importation is from the `_iter{n}.star` file, which contains particles remaining after the n-th sieving iteration. Subsequently, the process involves conducting sequential `ab-initio` jobs, followed by either `homogeneous refinement` or `non-uniform refinement` jobs.
 
-Alternatively, users can utilize the `cryosieve_auto_cryosparc.py` script, available in this repository, to circumvent the labor-intensive manual operations in CryoSPARC. The prerequisite for executing the `cryosieve_auto_cryosparc.py` script is the loading of CryoSPARC’s environment variables. This can be accomplished by executing the command `eval $(cryosparcm env)` in the shell. The successful loading of this environment can be verified by using the `which python` command. Upon successful execution, this command should point to a Python interpreter located within CryoSPARC’s installation path. Utilizing this Python interpreter, users can execute the `cryosieve_auto_cryosparc.py` script to automatically and sequentially carry out `import particle stack`, `ab-initio`, `homogenous refinement`, and `non-uniform refinement` jobs. These operations are performed for each particle stack listed in a sheet, which is provided as an argument to the `cryosieve_auto_cryosparc.py` script. For a detailed explanation of each `cryosieve_auto_cryosparc.py` option, please refer to the following section [Options/Arguments of `cryosieve_auto_cryosparc.py`](#cryosieve_auto_cryosparc).
+Alternatively, users can utilize the `cryosieve-csrefine` command, available in this repository, to streamline the labor-intensive manual operations in CryoSPARC. This script automates the sequential execution of `import particle stack`, `ab-initio`, `homogenous refinement` or `non-uniform refinement` jobs for each input particle stack. Additionally, it generates a summary of resolutions and B-factors. For a detailed explanation of each option available in `cryosieve-csrefine`, please refer to the following section [Options/Arguments of `cryosieve-csrefine`](#cryosieve-csrefine).
 
-# Options/Arguments of `cryosive-core`, `cryosieve` and `cryosieve_auto_cryosparc.py`
+### [Optional] Calculate the Rosenthal-Henderson B-factor
+
+The gold standard for assessing the quality of a set of single particle images involves determining its Rosenthal-Henderson B-factor. A lower B-factor indicates better quality. Utilizing CryoSieve to filter out ineffective particles can reduce the B-factor, suggesting improved quality among the remaining particles. Users can leverage the `cryosieve-csrhbfactor` command to automatically calculate the Rosenthal-Henderson B-factor by CryoSPARC. The script's arguments/options are similar to those in `cryosieve-csrhbfactor`. For a detailed explanation of each `cryosieve-csrhbfactor` option, please refer to the following section [Options/Arguments of `cryosieve-csrhbfactor`](#cryosieve-csrhbfactor).
+
+# Options/Arguments
 
 <a name="cryosieve-core"></a>
 ## Options/Arguments of `cryosieve-core`
 
 The program `cryosieve-core` is the core particle sieving module.
 
 ```
@@ -200,15 +202,15 @@
   --balance             make retained particles in different subsets in same size.
   --num_gpus NUM_GPUS   number of GPUs to execute the cryosieve program, 1 by default.
 ```
 
 <a name="cryosieve"></a>
 ## Options/Arguments of `cryosieve`
 
-The program `cryosieve` is an integreted program iteratively calling relion and `cryosieve-core` to do sieving process.
+The program `cryosieve` is an integreted program iteratively calling RELION and `cryosieve-core` to do sieving process.
 
 ```
 $ cryosieve -h
 usage: cryosieve [-h] --reconstruct_software RECONSTRUCT_SOFTWARE [--postprocess_software POSTPROCESS_SOFTWARE] --i I --o O --angpix ANGPIX [--sym SYM]
                  [--num_iters NUM_ITERS] [--frequency_start FREQUENCY_START] [--frequency_end FREQUENCY_END] [--retention_ratio RETENTION_RATIO] --mask MASK
                  [--balance] [--num_gpus NUM_GPUS]
 
@@ -219,15 +221,15 @@
   --reconstruct_software RECONSTRUCT_SOFTWARE
                         command for reconstruction.
   --postprocess_software POSTPROCESS_SOFTWARE
                         command for postprocessing.
   --i I                 input star file path.
   --o O                 output path prefix.
   --angpix ANGPIX       pixelsize in Angstrom.
-  --sym SYM             molecular symmetry, c1 by default.
+  --sym SYM             molecular symmetry, C1 by default.
   --num_iters NUM_ITERS
                         number of iterations for applying CryoSieve, 10 by default.
   --frequency_start FREQUENCY_START
                         starting threshold frquency, in Angstrom, 50A by default.
   --frequency_end FREQUENCY_END
                         ending threshold frquency, in Angstrom, 3A by default.
   --retention_ratio RETENTION_RATIO
@@ -236,49 +238,104 @@
   --balance             make remaining particles in different subsets in same size.
   --num_gpus NUM_GPUS   number of gpus to execute CryoSieve core program, 1 by default.
 ```
 
 There are several useful remarks:
 
 - CryoSieve utilizes the `RECONSTRUCT_SOFTWARE` in its reconstruction command. This enables you to enhance the speed of the reconstruction step through multiprocessing by using the option `--reconstruct_software "mpirun -n 5 relion_reconstruct_mpi"`. Additionally, you can further boost the reconstruction speed by using the option `--reconstruct_software "mpirun -n 5 relion_reconstruct_mpi --j 20"`, leveraging multi-threading.
-- If POSTPROCESS_SOFTWARE is not given, CryoSieve will skip the postprocessing step. Notice that postprocessing is not necessary for the sieving procedure.
+- If `POSTPROCESS_SOFTWARE` is not given, CryoSieve will skip the postprocessing step. Notice that postprocessing is not necessary for the sieving procedure.
 - Since `relion_reconstruct` use current directory as its default working directory, user should ensure that `relion_reconstruct` can correctly access the particles.
 
-<a name="cryosieve_auto_cryosparc"></a>
-## Options/Arguments of `cryosieve_auto_cryosparc.py`
+<a name="cryosieve-csrefine"></a>
+## Options/Arguments of `cryosieve-csrefine`
 
-The `cryosieve_auto_cryosparc.py` is a Python script designed to automatically and sequentially execute a series of operations in CryoSPARC, namely `import particle stack`, `ab-initio`, `homogenous refinement`, and `non-uniform refinement` jobs.
+The program `cryosieve-csrefine` is designed to automatically and sequentially execute a series of operations in CryoSPARC, namely `import particle stack`, `ab-initio`, `homogenous refinement` or `non-uniform refinement` jobs.
 
 ```
-usage: cryosieve_auto_cryosparc.py [-h] [--particles_sheet PARTICLES_SHEET] [--cryosparc_user_id CRYOSPARC_USER_ID]
-                                   [--cryosparc_project_uid CRYOSPARC_PROJECT_UID] [--cryosparc_workspace_uid CRYOSPARC_WORKSPACE_UID]
-                                   [--cryosparc_lane CRYOSPARC_LANE] [--molecular_symmetry MOLECULAR_SYMMETRY]
+$ cryosieve-csrefine -h
+usage: cryosieve-csrefine [-h] [--i I [I ...]] [--directory DIRECTORY] [--o O] [--sym SYM] [--ref REF] [--repeat REPEAT] --user USER
+                          --project PROJECT --workspace WORKSPACE --lane LANE [--nu] [--resplit] [--workers WORKERS]
 
-The cryosieve_auto_cryosparc.py is a Python script designed to automate CryoSPARC operations via the command line. Its purpose is to
-bypass the labor-intensive manual processes.
+cryosieve-csrefine: automatic SPA 3D-refinement by calling CryoSPARC.
 
 options:
   -h, --help            show this help message and exit
-  --particles_sheet PARTICLES_SHEET
-                        a file containing a list of starfiles; each starfile corresponds to a single-particle dataset; NOTE, absolute
-                        directory is mandatory
-  --cryosparc_user_id CRYOSPARC_USER_ID
-                        the E-mail address of the user of CryoSPARC
-  --cryosparc_project_uid CRYOSPARC_PROJECT_UID
-                        the project UID in cryoSPARC
-  --cryosparc_workspace_uid CRYOSPARC_WORKSPACE_UID
-                        the workspace UID in cryoSPARC
-  --cryosparc_lane CRYOSPARC_LANE
-                        the lane for computing resource in cryoSPARC
-  --molecular_symmetry MOLECULAR_SYMMETRY
-                        molecular symmetry
+  --i I [I ...]         input star file(s) or txt file(s) containing a list of star files.
+  --directory DIRECTORY
+                        directory of particles, empty (current directory) by default.
+  --o O                 output summary csv file path. If not provided, no summary is written.
+  --sym SYM             molecular symmetry, C1 by default.
+  --ref REF             initial reference model. If not provided, CryoSPARC's ab-initio job will be used.
+  --repeat REPEAT       number of trials, 1 by default.
+  --user USER           e-mail address of the user of CryoSPARC.
+  --project PROJECT     project UID in CryoSPARC.
+  --workspace WORKSPACE
+                        workspace UID in CryoSPARC.
+  --lane LANE           lane selected for computing in CryoSPARC.
+  --nu                  use non-uniform refinement.
+  --resplit             force re-do GS split.
+  --workers WORKERS     number of workers to run CryoSPARC job, unlimited by default.
 ```
 
+There are several useful remarks:
+
+- The input parameter `--i` supports multiple star files, such as `--i a.star b.star c.star`. Wildcards can also be used, for example, `--i output/_iter?.star` will include `output/_iter0.star`, `output/_iter1.star` up to `output/_iter9.star` in the previous example. Additionally, the input file can be a `.txt` file containing star files, with each file listed on a separate line.
+- When the `--o` parameter is provided, a summary report including resolutions and B-factors estimated by CryoSPARC will be written to a file in CSV format.
+- This program submits a series of jobs within a designated project and workspace. The compute resources are determined by the lane parameter. By default, the program refines all star files in parallel, but the option `--workers` allows you to limit the number of jobs executing simultaneously.
+
+For example, in the previous EMPAIR-11233 case, you can re-estimated all its output star files with a single command:
+```
+cryosieve-csrefine --i output/_iter?.star --o summary.csv --sym C4 --user XXX_YOUR_USER_EMAIL_XXX --project P1 --workspace W1 --lane XXX_YOUR_LANE_XXX
+```
+
+<a name="cryosieve-csrhbfactor"></a>
+## Options/Arguments of `cryosieve-csrhbfactor`
+
+The program `cryosieve-csrhbfactor` is designed to automatically determine Rosenthal-Henderson B-factor by calling `cryosieve-csrefine`.
+
+```
+$ cryosieve-csrhbfactor -h
+usage: cryosieve-csrhbfactor [-h] [--i I [I ...]] [--directory DIRECTORY] --o O [--sym SYM] [--ref REF] [--voltage VOLTAGE]
+                             [--repeat REPEAT] [--halves HALVES] --user USER --project PROJECT --workspace WORKSPACE --lane LANE [--nu]
+                             [--resplit] [--workers WORKERS]
+
+cryosieve-csrhbfactor: automatic Rosenthal-Henderson B-factor estimation by calling CryoSPARC.
+
+options:
+  -h, --help            show this help message and exit
+  --i I [I ...]         input star file(s) or txt file(s) containing a list of star files.
+  --directory DIRECTORY
+                        directory of particles, empty (current directory) by default.
+  --o O                 output summary csv file path.
+  --sym SYM             molecular symmetry, C1 by default.
+  --ref REF             initial reference model. If not provided, CryoSPARC's ab-initio job will be used.
+  --voltage VOLTAGE     acceleration voltage (kV), 300 by default. Only 200 and 300 supported!
+  --repeat REPEAT       number of trials, 1 by default.
+  --halves HALVES       number of times executing halvings, 4 by default.
+  --user USER           e-mail address of the user of CryoSPARC.
+  --project PROJECT     project UID in CryoSPARC.
+  --workspace WORKSPACE
+                        workspace UID in CryoSPARC.
+  --lane LANE           lane selected for computing in CryoSPARC.
+  --nu                  use non-uniform refinement.
+  --resplit             force re-do GS split.
+  --workers WORKERS     number of workers to run CryoSPARC job, unlimited by default.
+```
+
+There are several useful remarks:
+
+- The `cryosieve-csrhbfactor` program shares most parameters with `cryosieve-csrefine`, and their usage is similar.
+- Estimating the Rosenthal-Henderson B-factor involves a computationally intensive process. It requires iteratively halving the particle dataset and estimating the resolutions for each subset. For example, if you want to estimate the Rosenthal-Henderson B-factors for all 10 output stacks from the previous demo, and you choose to perform 3 trials with each stack using up to 4th halves, it would involve a total of 10 * 3 * (4 + 1) = 150 rounds of 3D-refinement.
+
 # Release Note
 
+* Version 1.2.5:
+  - Add two new programs: `cryosieve-csrefine` and `cryosieve-csrhbfactor`.
+  - Introduce a simplified command for preparing the Conda environment.
+  - Add support for CUDA >=11.8.
 * Version 1.2.4:
   - Fix the bug occurring with starfile >=0.5. CryoSieve now requires starfile >=0.4, <0.5.
   - Support gloo backend for multi-GPU version of cryosieve-core.
   - Fix the bug of SequentialSampler occurring with pytorch >=2.
 * Version 1.2.3: Add new video tutorial.
 * Version 1.2.1: fix the bug occurring when multiple optic groups are present in a star file.
 * Version 1.2: Initial stable release.
```

### Comparing `cryosieve-1.2.4/pyproject.toml` & `cryosieve-1.2.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cryosieve"
-version = "1.2.4"
+version = "1.2.5"
 authors = [
     { name="Jianying Zhu", email="zhu-jy20@mails.tsinghua.edu.cn" },
     { name="Qi Zhang", email="q-zhang20@mails.tsinghua.edu.cn" },
     { name="Hui Zhang", email="zhanghui198@mails.ucas.ac.cn" },
     { name="Zuoqiang Shi", email="zqshi@tsinghua.edu.cn" },
     { name="Mingxu Hu", email="humingxu@mail.tsinghua.edu.cn" },
     { name="Chenglong Bao", email="clbao@tsinghua.edu.cn" },
@@ -17,14 +17,15 @@
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
 dependencies = [
     "numpy>=1.18",
     "mrcfile>=1.2",
     "starfile>=0.4,<0.5",
+    "pandas<2.2",
     "cupy>=10",
     "torch>=1.10"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
@@ -34,7 +35,9 @@
 
 [project.urls]
 "Homepage" = "https://github.com/mxhulab/cryosieve"
 
 [project.scripts]
 "cryosieve" = "cryosieve.__main__:main"
 "cryosieve-core" = "cryosieve.core:core"
+"cryosieve-csrefine" = "cryosieve.cs_refine:main"
+"cryosieve-csrhbfactor" = "cryosieve.cs_rhbfactor:main"
```

### Comparing `cryosieve-1.2.4/src/cryosieve/ParticleDataset.py` & `cryosieve-1.2.5/src/cryosieve/ParticleDataset.py`

 * *Files identical despite different names*

### Comparing `cryosieve-1.2.4/src/cryosieve/__main__.py` & `cryosieve-1.2.5/src/cryosieve/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 import argparse
 import shutil
+import sys
 import numpy as np
 from pathlib import Path
 
-from .utility import run_commands
-
 def parse_argument():
     parser = argparse.ArgumentParser(description = 'CryoSieve: a particle sorting and sieving software for single particle analysis in cryo-EM.')
     parser.add_argument('--reconstruct_software', type = str,   required = True,  help = 'command for reconstruction.')
     parser.add_argument('--postprocess_software', type = str,   required = False, help = 'command for postprocessing.')
     parser.add_argument('--i',                    type = str,   required = True,  help = 'input star file path.')
     parser.add_argument('--o',                    type = str,   required = True,  help = 'output path prefix.')
     parser.add_argument('--angpix',               type = float, required = True,  help = 'pixelsize in Angstrom.')
-    parser.add_argument('--sym',                  type = str,   default  = 'c1',  help = 'molecular symmetry, c1 by default.')
+    parser.add_argument('--sym',                  type = str,   default  = 'C1',  help = 'molecular symmetry, C1 by default.')
     parser.add_argument('--num_iters',            type = int,   default  = 10,    help = 'number of iterations for applying CryoSieve, 10 by default.')
     parser.add_argument('--frequency_start',      type = float, default  = 50.,   help = 'starting threshold frquency, in Angstrom, 50A by default.')
     parser.add_argument('--frequency_end',        type = float, default  = 3.,    help = 'ending threshold frquency, in Angstrom, 3A by default.')
     parser.add_argument('--retention_ratio',      type = float, default  = 0.8,   help = 'fraction of retained particles in each iteration, 0.8 by default.')
     parser.add_argument('--mask',                 type = str,   required = True,  help = 'mask file path.')
     parser.add_argument('--balance',              action = 'store_true',          help = 'make remaining particles in different subsets in same size.')
     parser.add_argument('--num_gpus',             type = int,   default  = 1,     help = 'number of gpus to execute CryoSieve core program, 1 by default.')
+    if len(sys.argv) == 1:
+        parser.print_help()
+        exit()
     return parser.parse_args()
 
 def main():
     args = parse_argument()
+    from .utility import check_cupy
+    check_cupy()
 
     # copy the star file to output directory as iteration 0.
     src = Path(f'{args.i}')
     dst = Path(f'{args.o}_iter0.star')
     if not src.exists():
         raise FileNotFoundError(f'{args.i} not found.')
     elif src.suffix != '.star':
@@ -35,14 +39,15 @@
     dst.absolute().parent.mkdir(parents = True, exist_ok = True)
     try:
         shutil.copyfile(src, dst)
     except shutil.SameFileError:
         pass
 
     # go.
+    from .utility import run_commands
     frequences = 1 / np.linspace(1.0 / args.frequency_start, 1.0 / args.frequency_end, args.num_iters)
     overall_retention_ratio = 1.0
     for i in range(args.num_iters):
         print(f'[ITER {i}][Overall Retaining ratio: {overall_retention_ratio * 100:.2f}%][Threshold frequency : {frequences[i]:.2f}A]')
 
         # reconstruct.
         commands = [f'{args.reconstruct_software} --i {args.o}_iter{i}.star --o {args.o}_iter{i}_half1.mrc --angpix {args.angpix} --sym {args.sym} --ctf true --subset 1 >{args.o}_iter{i}_reconstruct_half1.txt',
```

### Comparing `cryosieve-1.2.4/src/cryosieve/core.py` & `cryosieve-1.2.5/src/cryosieve/core.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import argparse
 import os
+import sys
 import torch
 import torch.distributed
-import cupy as cp
 import numpy as np
 from time import time
-
-from .ParticleDataset import ParticleDataset
-from .utility import mrcread, run_commands
-from .sieve import sieve
+try:
+    import cupy as cp
+    from .ParticleDataset import ParticleDataset
+    from .utility import mrcread, run_commands
+    from .sieve import sieve
+except:
+    pass
 
 def core_parser():
     parser = argparse.ArgumentParser(description = 'CryoSieve core.')
     parser.add_argument('--i',               type = str,   required = True,  help = 'input star file path.')
     parser.add_argument('--o',               type = str,   required = True,  help = 'output star file path.')
     parser.add_argument('--directory',       type = str,   default  = '',    help = 'directory of particles, empty (current directory) by default.')
     parser.add_argument('--angpix',          type = float, required = True,  help = 'pixelsize in Angstrom.')
@@ -78,15 +81,20 @@
         root, ext = os.path.splitext(output_path)
         dataset_rem.save(output_path)
         dataset_sie.save(root + "_sieved" + ext)
 
 def core():
     parser = core_parser()
     parser.add_argument('--num_gpus',        type = int,   default  = 1,     help = 'number of GPUs to execute the cryosieve program, 1 by default.')
+    if len(sys.argv) == 1:
+        parser.print_help()
+        exit()
     args = parser.parse_args()
+    from .utility import check_cupy
+    check_cupy()
 
     if args.num_gpus == 1:
         time0 = time()
         main(args)
         time1 = time()
         print(f'[Processes completed successfully in {time1 - time0:.2f}s.][SINGLE-GPU CRYOSIEVE-CORE DONE.]')
     else:
```

### Comparing `cryosieve-1.2.4/src/cryosieve/kernels.py` & `cryosieve-1.2.5/src/cryosieve/kernels.py`

 * *Files identical despite different names*

### Comparing `cryosieve-1.2.4/src/cryosieve/sieve.py` & `cryosieve-1.2.5/src/cryosieve/sieve.py`

 * *Files identical despite different names*

### Comparing `cryosieve-1.2.4/src/cryosieve/utility.py` & `cryosieve-1.2.5/src/cryosieve/utility.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,27 @@
-import cupy as cp
-import numpy as np
 import mrcfile
 import subprocess
+import numpy as np
+try:
+    import cupy as cp
+except:
+    pass
 from time import time
 from torch.utils.dlpack import to_dlpack, from_dlpack
 
+def check_cupy():
+    try:
+        import cupy
+    except ModuleNotFoundError:
+        print('[ERROR] CuPy module not found.')
+        exit(1)
+    except ImportError:
+        print('[ERROR] Error occured when importing CuPy. Please check your CUDA environment or GPU card.')
+        exit(1)
+
 def cupy_to_torch(x):
     return from_dlpack(x.toDlpack())
 
 def torch_to_cupy(x):
     return cp.fromDlpack(to_dlpack(x))
 
 def mrcread(fpath : str, iSlc = None):
```

### Comparing `cryosieve-1.2.4/src/cryosieve.egg-info/PKG-INFO` & `cryosieve-1.2.5/src/cryosieve.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,980 +1,1038 @@
-Metadata-Version: 2.1
-Name: cryosieve
-Version: 1.2.4
-Summary: CryoSieve: a particle sorting and sieving algorithm for single particle analysis in cryo-EM
-Author-email: Jianying Zhu <zhu-jy20@mails.tsinghua.edu.cn>, Qi Zhang <q-zhang20@mails.tsinghua.edu.cn>, Hui Zhang <zhanghui198@mails.ucas.ac.cn>, Zuoqiang Shi <zqshi@tsinghua.edu.cn>, Mingxu Hu <humingxu@mail.tsinghua.edu.cn>, Chenglong Bao <clbao@tsinghua.edu.cn>
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
-Project-URL: Homepage, https://github.com/mxhulab/cryosieve
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Environment :: GPU :: NVIDIA CUDA
-Classifier: Topic :: Scientific/Engineering :: Image Processing
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS
-Requires-Dist: numpy>=1.18
-Requires-Dist: mrcfile>=1.2
-Requires-Dist: starfile<0.5,>=0.4
-Requires-Dist: cupy>=10
-Requires-Dist: torch>=1.10
-
-![featured image](featured_image.jpg)
-
-# CryoSieve Overview
-
-CryoSieve is an advanced software solution designed for particle sorting/sieving in single particle analysis (SPA) for Cryogenic Electron Microscopy (cryo-EM). Supported by extensive experimental results, CryoSieve has demonstrated superior performance and efficiency compared to other cryo-EM particle sorting algorithms.
-
-Its unique ability to eliminate unnecessary particles from final stacks significantly optimizes the data analysis process. The refined selection of particles that remain contribute to a notably higher resolution output in reconstructed density maps.
-
-For certain datasets, the precision of CryoSieve's particle subset selection is so refined that it approaches the theoretical limit, delivering unprecedented detail and accuracy.
-
-## Video Tutorial
-
-A video tutorial is available within this repository. You can directly download it [here](cryosieve_video_tutorial.mp4).
-
-## Publications
-
-For more details, please refer to the paper ["A minority of final stacks yields superior amplitude in single-particle cryo-EM"](https://www.nature.com/articles/s41467-023-43555-x). If you find that CryoSieve contributes to your work, we kindly request you to cite this paper.
-
-## The List of Available Demo Cases
-
-| dataset | number of particles | molecular weight (kDa) | EMPIAR link | expected result link
-| ------- | ------------------- | --------------------- | ----------- | --------------- |
-| TRPA1 | 43,585 | 688 | [EMPIAR-10024](https://www.ebi.ac.uk/empiar/EMPIAR-10024/) | [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-10024) |
-| hemagglutinin | 130,000 | 150 | [EMPIAR-10097](https://www.ebi.ac.uk/empiar/EMPIAR-10097/) | [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-10097) |
-| LAT1 | 250,712 | 172 | [EMPIAR-10264](https://www.ebi.ac.uk/empiar/EMPIAR-10264/) | [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-10264) |
-| pfCRT | 16,905 | 102 | [EMPIAR-10330](https://www.ebi.ac.uk/empiar/EMPIAR-10330/) | [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-10330) |
-| TSHR-Gs | 41,054 | 125 | [EMPIAR-11120](https://www.ebi.ac.uk/empiar/EMPIAR-11120/) | [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-11120) |
-| TRPM8 | 42,040 | 513 | [EMPIAR-11233](https://www.ebi.ac.uk/empiar/EMPIAR-11233/) | [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-11233) |
-| apoferritin | 382,391 | 440 | [EMPIAR-10200](https://www.ebi.ac.uk/empiar/EMPIAR-10200/) | [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-10200) |
-| streptavidin | 23,991 | 52 | [EMPIAR-10269](https://www.ebi.ac.uk/empiar/EMPIAR-10269/)  | [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-10269) |
-
-![main figure](main_figure.png)
-
-# Installation
-
-CryoSieve is an open-source software, developed using Python, and is available as a Python package. You can access our source code [on GitHub](https://github.com/mxhulab/cryosieve).
-
-## Prerequisites
-
-- Python version 3.7 or later.
-- NVIDIA CUDA library installed in the user's environment.
-
-## Dependencies
-
-The CryoSieve package depends on the following libraries:
-
-```
-numpy>=1.18
-mrcfile>=1.2
-starfile>=0.4,<0.5
-cupy>=10
-torch>=1.10
-```
-
-## Preparation of CUDA Environment
-
-We recommend you install CuPy and PyTorch initially, as their installation largely depends on your CUDA environment. Please note, your PyTorch package should be CUDA-capable.
-
-To streamline this process, we suggest preparing a conda environment with the following command:
-```
-conda create -n CRYOSIEVE_ENV python=3.10 cupy=10.2 cudatoolkit=10.2 pytorch=1.12.1=py3.10_cuda10.2_cudnn7.6.5_0 -c conda-forge -c pytorch
-```
-
-This command is specifically for a CUDA environment version 10.2. If your CUDA environment is higher than 10.2, adjust the command based on the suitable variants and versions recommended by the [CuPy](https://cupy.dev) and [PyTorch](https://pytorch.org) developers for your specific CUDA environment.
-
-## Installing CryoSieve
-
-After preparing CuPy and PyTorch according to your CUDA environment, it is crucial to activate it before proceeding with the CryoSieve installation.
-
-We recommend using the following command to activate it directly. (replace CRYOSIEVE_ENV with the name of your custom environment).
-
-```
-conda activate CRYOSIEVE_ENV
-```
-
-Then, we turn to the step of installing CryoSieve. CryoSieve can be installed either via `pip` or `conda`.
-
-To install CryoSieve using `pip`, execute the following command:
-
-```
-pip install cryosieve
-```
-
-Alternatively, to install CryoSieve using `conda`, execute the following command:
-
-```
-conda install -c mxhulab cryosieve
-```
-
-## Verifying Installation
-
-You can verify whether CryoSieve has been installed successfully by running the following command:
-
-```
-cryosieve -h
-```
-
-This should display the help information for CryoSieve, indicating a successful installation.
-
-# Tutorial
-
-## Quickstart: A Toy Example
-
-To validate your successful installation of CryoSieve and familiarize yourself with its functionalities, we highly recommend trying CryoSieve on this [toy example](https://github.com/mxhulab/cryosieve-demos/tree/master/toy). Please follow the steps below:
-
-1. Download the dataset and place it into any directory of your choice, e.g., `~/toy/`.
-2. Navigate to this directory by executing the following command:
-```
-cd ~/toy/
-```
-3. Initiate CryoSieve with the following command:
-```
-cryosieve-core --i CNG.star --o my_CNG_1.star --angpix 1.32 --volume CNG_A.mrc --volume CNG_B.mrc --mask CNG_mask.mrc --retention_ratio 0.8 --frequency 40
-```
-You may find explanation for each option of `cryosieve-core` [in the following section](#cryosieve-core).
-
-When the `--num_gpus` parameter is used with a value larger than 1, CryoSieve's core program will leverage multiple GPUs to expedite the sieving process. It accomplishes this by using PyTorch's [elastic launch](https://pytorch.org/docs/1.10/elastic/run.html?highlight=torchrun) feature to initiate multiple processes. Each of these processes will use exactly one GPU.
-
-For instance, on a machine equipped with 4 GPUs, you can use the following command to run the toy example:
-```
-cryosieve-core --i CNG.star --o my_CNG_1.star --angpix 1.32 --volume CNG_A.mrc --volume CNG_B.mrc --mask CNG_mask.mrc --retention_ratio 0.8 --frequency 40 --num_gpus 4
-```
-
-Upon successful execution, the command will generate two star files, `my_CNG_1.star` and `my_CNG_1_sieved.star`. These files contain the information of the remaining particles and the sieved particles, respectively. You can compare them with the provided `CNG_1.star` and `CNG_1_sieved.star` files. If executed correctly, they should contain the same particles.
-
-## Processing Real-World Dataset
-
-In this section, we provide a hands-on example of how to utilize CryoSieve for processing the final stack in a real-world experimental dataset.
-
-### Download the Dataset
-
-For this tutorial, we'll be using the final particle stack from the [EMPIAR-11233](https://www.ebi.ac.uk/empiar/EMPIAR-11233/) dataset. This dataset includes a final particle stack of TRPM8 bound to calcium, collected on a 300 kV FEI Titan Krios microscope.
-
-To download the final particle stack, navigate to your desired working directory and execute the following command:
-
-```
-wget -nH -m ftp://ftp.ebi.ac.uk/empiar/world_availability/11233/data/Final_Particle_Stack/
-```
-
-Upon completion, you'll find a new directory named `XXX/data/Final_Particle_Stack` in your working directory. This directory contains a star file with all particle information and an mrcs file representing the final stack.
-
-Additionally, you'll need a mask file. You can generate a mask file using any cryo-EM software, based on the reconstructed volume. If you prefer not to generate a mask file, we've provided one used in our experiments which you can download from this [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-11233). Once you have the mask file, move it into the `Final_Particle_Stack` directory.
-
-You can find additional demonstration data, along with expected results, in [this repository](https://github.com/mxhulab/cryosieve-demos/tree/master).
-
-### Iterative Reconstruction and Sieving
-
-To achieve optimal results with real-world datasets, the sieving process generally involves several iterations. In each iteration, we perform 3D reconstruction (and perhaps postprocessing to derive the Fourier Shell Correlation (FSC) curve and resolution). We then apply CryoSieve to sieve a fraction of the particles based on the reconstructed map. The highpass cut-off frequency typically increases with each round.
-
-For your convenience, we've developed an automatic command `cryosieve` which performs all these steps in a single run. To use it, please follow these steps:
-
-1. Change the working directory to `XXX/data/Final_Particle_Stack`:
-```
-cd XXX/data/Final_Particle_Stack
-```
-2. Our automatic program currently uses Relion for 3D reconstruction and postprocessing. Therefore, make sure that `relion_reconstruct` or `relion_reconstruct_mpi` and `relion_postprocess` are accessible. Once confirmed, run the following command:
-```
-cryosieve --reconstruct_software relion_reconstruct --postprocess_software relion_postprocess --i diver2019_pmTRPM8_calcium_Krios_6Feb18_finalParticleStack_EMPIAR_composite.star --o output/ --mask mask.mrc --angpix 1.059 --num_iters 10 --frequency_start 40 --frequency_end 3 --retention_ratio 0.8 --sym C4
-```
-
-For a detailed explanation of each `cryosieve` option, please refer to the following section [Options/Arguments of `cryosieve`](#cryosieve).
-
-The entire process may take over an hour, depending on your system resources. Multiple result files will be generated and saved in the `output/` directory. For instance, the `_iter{n}.star` file contains particles that remain after the n-th sieving iteration, and the `_postprocess_iter{n}` folder houses the postprocessing result after the n-th iteration.
-
-### [Recommended] Re-estimate poses by CryoSPARC
-
-The objective of re-estimating poses using CryoSPARC is to prevent the unintentional transfer of information from the discarded particles to those that are retained. This process of re-estimating poses with CryoSPARC can be conducted either manually or through automation using a Python script. The script, named `cryosieve_auto_cryosparc.py`, is provided by us in this repository.
-
-For manually re-estimating poses with CryoSPARC, particles must be imported using CryoSPARC’s `import particle stack` job. This importation is from the `_iter{n}.star` file, which contains particles remaining after the n-th sieving iteration. Subsequently, the process involves conducting sequential `ab-initio` jobs, followed by either `homogeneous refinement` or `non-uniform refinement` jobs.
-
-Alternatively, users can utilize the `cryosieve_auto_cryosparc.py` script, available in this repository, to circumvent the labor-intensive manual operations in CryoSPARC. The prerequisite for executing the `cryosieve_auto_cryosparc.py` script is the loading of CryoSPARC’s environment variables. This can be accomplished by executing the command `eval $(cryosparcm env)` in the shell. The successful loading of this environment can be verified by using the `which python` command. Upon successful execution, this command should point to a Python interpreter located within CryoSPARC’s installation path. Utilizing this Python interpreter, users can execute the `cryosieve_auto_cryosparc.py` script to automatically and sequentially carry out `import particle stack`, `ab-initio`, `homogenous refinement`, and `non-uniform refinement` jobs. These operations are performed for each particle stack listed in a sheet, which is provided as an argument to the `cryosieve_auto_cryosparc.py` script. For a detailed explanation of each `cryosieve_auto_cryosparc.py` option, please refer to the following section [Options/Arguments of `cryosieve_auto_cryosparc.py`](#cryosieve_auto_cryosparc).
-
-# Options/Arguments of `cryosive-core`, `cryosieve` and `cryosieve_auto_cryosparc.py`
-
-<a name="cryosieve-core"></a>
-## Options/Arguments of `cryosieve-core`
-
-The program `cryosieve-core` is the core particle sieving module.
-
-```
-$ cryosieve-core -h
-usage: cryosieve-core [-h] --i I --o O [--directory DIRECTORY] --angpix ANGPIX --volume VOLUME [--mask MASK] [--retention_ratio RETENTION_RATIO] --frequency
-                      FREQUENCY [--balance] [--num_gpus NUM_GPUS]
-
-CryoSieve core.
-
-options:
-  -h, --help            show this help message and exit
-  --i I                 input star file path.
-  --o O                 output star file path.
-  --directory DIRECTORY
-                        directory of particles, empty (current directory) by default.
-  --angpix ANGPIX       pixelsize in Angstrom.
-  --volume VOLUME       list of volume file paths.
-  --mask MASK           mask file path.
-  --retention_ratio RETENTION_RATIO
-                        fraction of retained particles, 0.8 by default.
-  --frequency FREQUENCY
-                        cut-off highpass frequency.
-  --balance             make retained particles in different subsets in same size.
-  --num_gpus NUM_GPUS   number of GPUs to execute the cryosieve program, 1 by default.
-```
-
-<a name="cryosieve"></a>
-## Options/Arguments of `cryosieve`
-
-The program `cryosieve` is an integreted program iteratively calling relion and `cryosieve-core` to do sieving process.
-
-```
-$ cryosieve -h
-usage: cryosieve [-h] --reconstruct_software RECONSTRUCT_SOFTWARE [--postprocess_software POSTPROCESS_SOFTWARE] --i I --o O --angpix ANGPIX [--sym SYM]
-                 [--num_iters NUM_ITERS] [--frequency_start FREQUENCY_START] [--frequency_end FREQUENCY_END] [--retention_ratio RETENTION_RATIO] --mask MASK
-                 [--balance] [--num_gpus NUM_GPUS]
-
-CryoSieve: a particle sorting and sieving software for single particle analysis in cryo-EM.
-
-options:
-  -h, --help            show this help message and exit
-  --reconstruct_software RECONSTRUCT_SOFTWARE
-                        command for reconstruction.
-  --postprocess_software POSTPROCESS_SOFTWARE
-                        command for postprocessing.
-  --i I                 input star file path.
-  --o O                 output path prefix.
-  --angpix ANGPIX       pixelsize in Angstrom.
-  --sym SYM             molecular symmetry, c1 by default.
-  --num_iters NUM_ITERS
-                        number of iterations for applying CryoSieve, 10 by default.
-  --frequency_start FREQUENCY_START
-                        starting threshold frquency, in Angstrom, 50A by default.
-  --frequency_end FREQUENCY_END
-                        ending threshold frquency, in Angstrom, 3A by default.
-  --retention_ratio RETENTION_RATIO
-                        fraction of retained particles in each iteration, 0.8 by default.
-  --mask MASK           mask file path.
-  --balance             make remaining particles in different subsets in same size.
-  --num_gpus NUM_GPUS   number of gpus to execute CryoSieve core program, 1 by default.
-```
-
-There are several useful remarks:
-
-- CryoSieve utilizes the `RECONSTRUCT_SOFTWARE` in its reconstruction command. This enables you to enhance the speed of the reconstruction step through multiprocessing by using the option `--reconstruct_software "mpirun -n 5 relion_reconstruct_mpi"`. Additionally, you can further boost the reconstruction speed by using the option `--reconstruct_software "mpirun -n 5 relion_reconstruct_mpi --j 20"`, leveraging multi-threading.
-- If POSTPROCESS_SOFTWARE is not given, CryoSieve will skip the postprocessing step. Notice that postprocessing is not necessary for the sieving procedure.
-- Since `relion_reconstruct` use current directory as its default working directory, user should ensure that `relion_reconstruct` can correctly access the particles.
-
-<a name="cryosieve_auto_cryosparc"></a>
-## Options/Arguments of `cryosieve_auto_cryosparc.py`
-
-The `cryosieve_auto_cryosparc.py` is a Python script designed to automatically and sequentially execute a series of operations in CryoSPARC, namely `import particle stack`, `ab-initio`, `homogenous refinement`, and `non-uniform refinement` jobs.
-
-```
-usage: cryosieve_auto_cryosparc.py [-h] [--particles_sheet PARTICLES_SHEET] [--cryosparc_user_id CRYOSPARC_USER_ID]
-                                   [--cryosparc_project_uid CRYOSPARC_PROJECT_UID] [--cryosparc_workspace_uid CRYOSPARC_WORKSPACE_UID]
-                                   [--cryosparc_lane CRYOSPARC_LANE] [--molecular_symmetry MOLECULAR_SYMMETRY]
-
-The cryosieve_auto_cryosparc.py is a Python script designed to automate CryoSPARC operations via the command line. Its purpose is to
-bypass the labor-intensive manual processes.
-
-options:
-  -h, --help            show this help message and exit
-  --particles_sheet PARTICLES_SHEET
-                        a file containing a list of starfiles; each starfile corresponds to a single-particle dataset; NOTE, absolute
-                        directory is mandatory
-  --cryosparc_user_id CRYOSPARC_USER_ID
-                        the E-mail address of the user of CryoSPARC
-  --cryosparc_project_uid CRYOSPARC_PROJECT_UID
-                        the project UID in cryoSPARC
-  --cryosparc_workspace_uid CRYOSPARC_WORKSPACE_UID
-                        the workspace UID in cryoSPARC
-  --cryosparc_lane CRYOSPARC_LANE
-                        the lane for computing resource in cryoSPARC
-  --molecular_symmetry MOLECULAR_SYMMETRY
-                        molecular symmetry
-```
-
-# Release Note
-
-* Version 1.2.4:
-  - Fix the bug occurring with starfile >=0.5. CryoSieve now requires starfile >=0.4, <0.5.
-  - Support gloo backend for multi-GPU version of cryosieve-core.
-  - Fix the bug of SequentialSampler occurring with pytorch >=2.
-* Version 1.2.3: Add new video tutorial.
-* Version 1.2.1: fix the bug occurring when multiple optic groups are present in a star file.
-* Version 1.2: Initial stable release.
+Metadata-Version: 2.1
+Name: cryosieve
+Version: 1.2.5
+Summary: CryoSieve: a particle sorting and sieving algorithm for single particle analysis in cryo-EM
+Author-email: Jianying Zhu <zhu-jy20@mails.tsinghua.edu.cn>, Qi Zhang <q-zhang20@mails.tsinghua.edu.cn>, Hui Zhang <zhanghui198@mails.ucas.ac.cn>, Zuoqiang Shi <zqshi@tsinghua.edu.cn>, Mingxu Hu <humingxu@mail.tsinghua.edu.cn>, Chenglong Bao <clbao@tsinghua.edu.cn>
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
+Project-URL: Homepage, https://github.com/mxhulab/cryosieve
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Environment :: GPU :: NVIDIA CUDA
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS
+Requires-Dist: numpy>=1.18
+Requires-Dist: mrcfile>=1.2
+Requires-Dist: starfile<0.5,>=0.4
+Requires-Dist: pandas<2.2
+Requires-Dist: cupy>=10
+Requires-Dist: torch>=1.10
+
+![featured image](featured_image.jpg)
+
+# CryoSieve Overview
+
+CryoSieve is an advanced software solution designed for particle sorting/sieving in single particle analysis (SPA) for Cryogenic Electron Microscopy (cryo-EM). Supported by extensive experimental results, CryoSieve has demonstrated superior performance and efficiency compared to other cryo-EM particle sorting algorithms.
+
+Its unique ability to eliminate unnecessary particles from final stacks significantly optimizes the data analysis process. The refined selection of particles that remain contribute to a notably higher resolution output in reconstructed density maps.
+
+For certain datasets, the precision of CryoSieve's particle subset selection is so refined that it approaches the theoretical limit, delivering unprecedented detail and accuracy.
+
+## Video Tutorial
+
+A video tutorial is available within this repository. You can directly download it [here](cryosieve_video_tutorial.mp4).
+
+## Publications
+
+For more details, please refer to the paper ["A minority of final stacks yields superior amplitude in single-particle cryo-EM"](https://www.nature.com/articles/s41467-023-43555-x). If you find that CryoSieve contributes to your work, we kindly request you to cite this paper.
+
+## The List of Available Demo Cases
+
+| dataset | number of particles | molecular weight (kDa) | EMPIAR link | expected result link
+| ------- | ------------------- | --------------------- | ----------- | --------------- |
+| TRPA1 | 43,585 | 688 | [EMPIAR-10024](https://www.ebi.ac.uk/empiar/EMPIAR-10024/) | [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-10024) |
+| hemagglutinin | 130,000 | 150 | [EMPIAR-10097](https://www.ebi.ac.uk/empiar/EMPIAR-10097/) | [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-10097) |
+| LAT1 | 250,712 | 172 | [EMPIAR-10264](https://www.ebi.ac.uk/empiar/EMPIAR-10264/) | [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-10264) |
+| pfCRT | 16,905 | 102 | [EMPIAR-10330](https://www.ebi.ac.uk/empiar/EMPIAR-10330/) | [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-10330) |
+| TSHR-Gs | 41,054 | 125 | [EMPIAR-11120](https://www.ebi.ac.uk/empiar/EMPIAR-11120/) | [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-11120) |
+| TRPM8 | 42,040 | 513 | [EMPIAR-11233](https://www.ebi.ac.uk/empiar/EMPIAR-11233/) | [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-11233) |
+| apoferritin | 382,391 | 440 | [EMPIAR-10200](https://www.ebi.ac.uk/empiar/EMPIAR-10200/) | [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-10200) |
+| streptavidin | 23,991 | 52 | [EMPIAR-10269](https://www.ebi.ac.uk/empiar/EMPIAR-10269/)  | [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-10269) |
+
+![main figure](main_figure.png)
+
+# Installation
+
+CryoSieve is an open-source software, developed using Python, and is available as a Python package. Please access our source code [on GitHub](https://github.com/mxhulab/cryosieve).
+
+## Prerequisites
+
+- Python version 3.7 or later.
+- NVIDIA CUDA library 10.2 or later installed in the user's environment.
+
+## Dependencies
+
+The CryoSieve package depends on the following libraries:
+
+```
+numpy>=1.18
+mrcfile>=1.2
+starfile>=0.4,<0.5
+pandans<2.2
+cupy>=10
+torch>=1.10
+```
+
+## Preparation of CUDA Environment
+
+We recommend installing CuPy and PyTorch initially, as their installation largely depends on the CUDA environment. Please note, PyTorch should be CUDA-capable. To streamline this process, we suggest preparing a conda environment with the following commands.
+
+For CUDA version <= 11.7:
+```
+conda create -n CRYOSIEVE_ENV python=3.8 cudatoolkit=10.2 cupy=10.0 pytorch=1.10 -c pytorch -c conda-forge
+```
+Please note that this command is tailored for CUDA version 10.2. To accommodate a different CUDA version, adjust the `cudatoolkit` version accordingly. Modify the versions of Python, CuPy, and PyTorch based on requirements, ensuring compatibility with the minimal requirements of CryoSieve.
+
+For CUDA version >= 11.8:
+```
+conda create -n CRYOSIEVE_ENV python=3.10 cupy=12.0 pytorch pytorch-cuda=12.1 -c pytorch -c nvidia -c conda-forge
+```
+Please note that This command is tailored for CUDA environment version 12.1. For a different CUDA version, adjust `pytorch-cuda` version accordingly.
+
+## Installing CryoSieve
+
+After preparing CuPy and PyTorch, it is crucial to activate it before proceeding with the CryoSieve installation.
+```
+conda activate CRYOSIEVE_ENV
+```
+
+Then, we turn to the step of installing CryoSieve. CryoSieve can be installed either via `pip` or `conda`.
+
+To install CryoSieve using `pip`, execute the following command:
+```
+pip install cryosieve
+```
+Alternatively, to install CryoSieve using `conda`, execute the following command:
+```
+conda install -c mxhulab cryosieve
+```
+
+## Verifying Installation
+
+You can verify whether CryoSieve has been installed successfully by running the following command:
+```
+cryosieve -h
+```
+This should display the help information for CryoSieve, indicating a successful installation.
+
+# Tutorial
+
+## Quickstart: A Toy Example
+
+To validate your successful installation of CryoSieve and familiarize yourself with its functionalities, we highly recommend trying CryoSieve on this [toy example](https://github.com/mxhulab/cryosieve-demos/tree/master/toy). Please follow the steps below:
+
+1. Download the dataset and place it into any directory of your choice, e.g., `~/toy/`.
+2. Navigate to this directory by executing the following command:
+```
+cd ~/toy/
+```
+3. Initiate CryoSieve with the following command:
+```
+cryosieve-core --i CNG.star --o my_CNG_1.star --angpix 1.32 --volume CNG_A.mrc --volume CNG_B.mrc --mask CNG_mask.mrc --retention_ratio 0.8 --frequency 40
+```
+You may find explanation for each option of `cryosieve-core` [in the following section](#cryosieve-core).
+
+When the `--num_gpus` parameter is used with a value larger than 1, CryoSieve's core program will leverage multiple GPUs to expedite the sieving process. It accomplishes this by using PyTorch's [elastic launch](https://pytorch.org/docs/1.10/elastic/run.html?highlight=torchrun) feature to initiate multiple processes. Each of these processes will use exactly one GPU.
+
+For instance, on a machine equipped with 4 GPUs, you can use the following command to run the toy example:
+```
+cryosieve-core --i CNG.star --o my_CNG_1.star --angpix 1.32 --volume CNG_A.mrc --volume CNG_B.mrc --mask CNG_mask.mrc --retention_ratio 0.8 --frequency 40 --num_gpus 4
+```
+
+Upon successful execution, the command will generate two star files, `my_CNG_1.star` and `my_CNG_1_sieved.star`. These files contain the information of the remaining particles and the sieved particles, respectively. You can compare them with the provided `CNG_1.star` and `CNG_1_sieved.star` files. If executed correctly, they should contain the same particles.
+
+## Processing Real-World Dataset
+
+In this section, we provide a hands-on example of how to utilize CryoSieve for processing the final stack in a real-world experimental dataset.
+
+### Download the Dataset
+
+For this tutorial, we'll be using the final particle stack from the [EMPIAR-11233](https://www.ebi.ac.uk/empiar/EMPIAR-11233/) dataset. This dataset includes a final particle stack of TRPM8 bound to calcium, collected on a 300 kV FEI Titan Krios microscope.
+
+To download the final particle stack, navigate to your desired working directory and execute the following command:
+
+```
+wget -nH -m ftp://ftp.ebi.ac.uk/empiar/world_availability/11233/data/Final_Particle_Stack/
+```
+
+Upon completion, you'll find a new directory named `XXX/data/Final_Particle_Stack` in your working directory. This directory contains a star file with all particle information and an mrcs file representing the final stack.
+
+Additionally, you'll need a mask file. You can generate a mask file using any cryo-EM software, based on the reconstructed volume. If you prefer not to generate a mask file, we've provided one used in our experiments which you can download from this [link](https://github.com/mxhulab/cryosieve-demos/tree/master/EMPIAR-11233). Once you have the mask file, move it into the `Final_Particle_Stack` directory.
+
+You can find additional demonstration data, along with expected results, in [this repository](https://github.com/mxhulab/cryosieve-demos/tree/master).
+
+### Iterative Reconstruction and Sieving
+
+To achieve optimal results with real-world datasets, the sieving process generally involves several iterations. In each iteration, we perform 3D reconstruction (and perhaps postprocessing to derive the Fourier Shell Correlation (FSC) curve and resolution). We then apply CryoSieve to sieve a fraction of the particles based on the reconstructed map. The highpass cut-off frequency typically increases with each round.
+
+For your convenience, we've developed an automatic command `cryosieve` which performs all these steps in a single run. To use it, please follow these steps:
+
+1. Change the working directory to `XXX/data/Final_Particle_Stack`:
+```
+cd XXX/data/Final_Particle_Stack
+```
+2. Our automatic program currently uses Relion for 3D reconstruction and postprocessing. Therefore, make sure that `relion_reconstruct` or `relion_reconstruct_mpi` and `relion_postprocess` are accessible. Once confirmed, run the following command:
+```
+cryosieve --reconstruct_software relion_reconstruct --postprocess_software relion_postprocess --i diver2019_pmTRPM8_calcium_Krios_6Feb18_finalParticleStack_EMPIAR_composite.star --o output/ --mask mask.mrc --angpix 1.059 --num_iters 10 --frequency_start 40 --frequency_end 3 --retention_ratio 0.8 --sym C4
+```
+
+For a detailed explanation of each `cryosieve` option, please refer to the following section [Options/Arguments of `cryosieve`](#cryosieve).
+
+The entire process may take over an hour, depending on your system resources. Multiple result files will be generated and saved in the `output/` directory. For instance, the `_iter{n}.star` file contains particles that remain after the n-th sieving iteration, and the `_postprocess_iter{n}` folder houses the postprocessing result after the n-th iteration.
+
+### [Recommended] Re-estimate poses
+
+The objective of re-estimating poses is to prevent the unintentional transfer of information from the discarded particles to those that are retained. This process of re-estimating poses with CryoSPARC can be performed manually or automated using a Python module. We provide a Python script named `cryosieve-csrefine` in this repository for this purpose.
+
+For manually re-estimating poses with CryoSPARC, particles must be imported using CryoSPARC’s `import particle stack` job. This importation is from the `_iter{n}.star` file, which contains particles remaining after the n-th sieving iteration. Subsequently, the process involves conducting sequential `ab-initio` jobs, followed by either `homogeneous refinement` or `non-uniform refinement` jobs.
+
+Alternatively, users can utilize the `cryosieve-csrefine` command, available in this repository, to streamline the labor-intensive manual operations in CryoSPARC. This script automates the sequential execution of `import particle stack`, `ab-initio`, `homogenous refinement` or `non-uniform refinement` jobs for each input particle stack. Additionally, it generates a summary of resolutions and B-factors. For a detailed explanation of each option available in `cryosieve-csrefine`, please refer to the following section [Options/Arguments of `cryosieve-csrefine`](#cryosieve-csrefine).
+
+### [Optional] Calculate the Rosenthal-Henderson B-factor
+
+The gold standard for assessing the quality of a set of single particle images involves determining its Rosenthal-Henderson B-factor. A lower B-factor indicates better quality. Utilizing CryoSieve to filter out ineffective particles can reduce the B-factor, suggesting improved quality among the remaining particles. Users can leverage the `cryosieve-csrhbfactor` command to automatically calculate the Rosenthal-Henderson B-factor by CryoSPARC. The script's arguments/options are similar to those in `cryosieve-csrhbfactor`. For a detailed explanation of each `cryosieve-csrhbfactor` option, please refer to the following section [Options/Arguments of `cryosieve-csrhbfactor`](#cryosieve-csrhbfactor).
+
+# Options/Arguments
+
+<a name="cryosieve-core"></a>
+## Options/Arguments of `cryosieve-core`
+
+The program `cryosieve-core` is the core particle sieving module.
+
+```
+$ cryosieve-core -h
+usage: cryosieve-core [-h] --i I --o O [--directory DIRECTORY] --angpix ANGPIX --volume VOLUME [--mask MASK] [--retention_ratio RETENTION_RATIO] --frequency
+                      FREQUENCY [--balance] [--num_gpus NUM_GPUS]
+
+CryoSieve core.
+
+options:
+  -h, --help            show this help message and exit
+  --i I                 input star file path.
+  --o O                 output star file path.
+  --directory DIRECTORY
+                        directory of particles, empty (current directory) by default.
+  --angpix ANGPIX       pixelsize in Angstrom.
+  --volume VOLUME       list of volume file paths.
+  --mask MASK           mask file path.
+  --retention_ratio RETENTION_RATIO
+                        fraction of retained particles, 0.8 by default.
+  --frequency FREQUENCY
+                        cut-off highpass frequency.
+  --balance             make retained particles in different subsets in same size.
+  --num_gpus NUM_GPUS   number of GPUs to execute the cryosieve program, 1 by default.
+```
+
+<a name="cryosieve"></a>
+## Options/Arguments of `cryosieve`
+
+The program `cryosieve` is an integreted program iteratively calling RELION and `cryosieve-core` to do sieving process.
+
+```
+$ cryosieve -h
+usage: cryosieve [-h] --reconstruct_software RECONSTRUCT_SOFTWARE [--postprocess_software POSTPROCESS_SOFTWARE] --i I --o O --angpix ANGPIX [--sym SYM]
+                 [--num_iters NUM_ITERS] [--frequency_start FREQUENCY_START] [--frequency_end FREQUENCY_END] [--retention_ratio RETENTION_RATIO] --mask MASK
+                 [--balance] [--num_gpus NUM_GPUS]
+
+CryoSieve: a particle sorting and sieving software for single particle analysis in cryo-EM.
+
+options:
+  -h, --help            show this help message and exit
+  --reconstruct_software RECONSTRUCT_SOFTWARE
+                        command for reconstruction.
+  --postprocess_software POSTPROCESS_SOFTWARE
+                        command for postprocessing.
+  --i I                 input star file path.
+  --o O                 output path prefix.
+  --angpix ANGPIX       pixelsize in Angstrom.
+  --sym SYM             molecular symmetry, C1 by default.
+  --num_iters NUM_ITERS
+                        number of iterations for applying CryoSieve, 10 by default.
+  --frequency_start FREQUENCY_START
+                        starting threshold frquency, in Angstrom, 50A by default.
+  --frequency_end FREQUENCY_END
+                        ending threshold frquency, in Angstrom, 3A by default.
+  --retention_ratio RETENTION_RATIO
+                        fraction of retained particles in each iteration, 0.8 by default.
+  --mask MASK           mask file path.
+  --balance             make remaining particles in different subsets in same size.
+  --num_gpus NUM_GPUS   number of gpus to execute CryoSieve core program, 1 by default.
+```
+
+There are several useful remarks:
+
+- CryoSieve utilizes the `RECONSTRUCT_SOFTWARE` in its reconstruction command. This enables you to enhance the speed of the reconstruction step through multiprocessing by using the option `--reconstruct_software "mpirun -n 5 relion_reconstruct_mpi"`. Additionally, you can further boost the reconstruction speed by using the option `--reconstruct_software "mpirun -n 5 relion_reconstruct_mpi --j 20"`, leveraging multi-threading.
+- If `POSTPROCESS_SOFTWARE` is not given, CryoSieve will skip the postprocessing step. Notice that postprocessing is not necessary for the sieving procedure.
+- Since `relion_reconstruct` use current directory as its default working directory, user should ensure that `relion_reconstruct` can correctly access the particles.
+
+<a name="cryosieve-csrefine"></a>
+## Options/Arguments of `cryosieve-csrefine`
+
+The program `cryosieve-csrefine` is designed to automatically and sequentially execute a series of operations in CryoSPARC, namely `import particle stack`, `ab-initio`, `homogenous refinement` or `non-uniform refinement` jobs.
+
+```
+$ cryosieve-csrefine -h
+usage: cryosieve-csrefine [-h] [--i I [I ...]] [--directory DIRECTORY] [--o O] [--sym SYM] [--ref REF] [--repeat REPEAT] --user USER
+                          --project PROJECT --workspace WORKSPACE --lane LANE [--nu] [--resplit] [--workers WORKERS]
+
+cryosieve-csrefine: automatic SPA 3D-refinement by calling CryoSPARC.
+
+options:
+  -h, --help            show this help message and exit
+  --i I [I ...]         input star file(s) or txt file(s) containing a list of star files.
+  --directory DIRECTORY
+                        directory of particles, empty (current directory) by default.
+  --o O                 output summary csv file path. If not provided, no summary is written.
+  --sym SYM             molecular symmetry, C1 by default.
+  --ref REF             initial reference model. If not provided, CryoSPARC's ab-initio job will be used.
+  --repeat REPEAT       number of trials, 1 by default.
+  --user USER           e-mail address of the user of CryoSPARC.
+  --project PROJECT     project UID in CryoSPARC.
+  --workspace WORKSPACE
+                        workspace UID in CryoSPARC.
+  --lane LANE           lane selected for computing in CryoSPARC.
+  --nu                  use non-uniform refinement.
+  --resplit             force re-do GS split.
+  --workers WORKERS     number of workers to run CryoSPARC job, unlimited by default.
+```
+
+There are several useful remarks:
+
+- The input parameter `--i` supports multiple star files, such as `--i a.star b.star c.star`. Wildcards can also be used, for example, `--i output/_iter?.star` will include `output/_iter0.star`, `output/_iter1.star` up to `output/_iter9.star` in the previous example. Additionally, the input file can be a `.txt` file containing star files, with each file listed on a separate line.
+- When the `--o` parameter is provided, a summary report including resolutions and B-factors estimated by CryoSPARC will be written to a file in CSV format.
+- This program submits a series of jobs within a designated project and workspace. The compute resources are determined by the lane parameter. By default, the program refines all star files in parallel, but the option `--workers` allows you to limit the number of jobs executing simultaneously.
+
+For example, in the previous EMPAIR-11233 case, you can re-estimated all its output star files with a single command:
+```
+cryosieve-csrefine --i output/_iter?.star --o summary.csv --sym C4 --user XXX_YOUR_USER_EMAIL_XXX --project P1 --workspace W1 --lane XXX_YOUR_LANE_XXX
+```
+
+<a name="cryosieve-csrhbfactor"></a>
+## Options/Arguments of `cryosieve-csrhbfactor`
+
+The program `cryosieve-csrhbfactor` is designed to automatically determine Rosenthal-Henderson B-factor by calling `cryosieve-csrefine`.
+
+```
+$ cryosieve-csrhbfactor -h
+usage: cryosieve-csrhbfactor [-h] [--i I [I ...]] [--directory DIRECTORY] --o O [--sym SYM] [--ref REF] [--voltage VOLTAGE]
+                             [--repeat REPEAT] [--halves HALVES] --user USER --project PROJECT --workspace WORKSPACE --lane LANE [--nu]
+                             [--resplit] [--workers WORKERS]
+
+cryosieve-csrhbfactor: automatic Rosenthal-Henderson B-factor estimation by calling CryoSPARC.
+
+options:
+  -h, --help            show this help message and exit
+  --i I [I ...]         input star file(s) or txt file(s) containing a list of star files.
+  --directory DIRECTORY
+                        directory of particles, empty (current directory) by default.
+  --o O                 output summary csv file path.
+  --sym SYM             molecular symmetry, C1 by default.
+  --ref REF             initial reference model. If not provided, CryoSPARC's ab-initio job will be used.
+  --voltage VOLTAGE     acceleration voltage (kV), 300 by default. Only 200 and 300 supported!
+  --repeat REPEAT       number of trials, 1 by default.
+  --halves HALVES       number of times executing halvings, 4 by default.
+  --user USER           e-mail address of the user of CryoSPARC.
+  --project PROJECT     project UID in CryoSPARC.
+  --workspace WORKSPACE
+                        workspace UID in CryoSPARC.
+  --lane LANE           lane selected for computing in CryoSPARC.
+  --nu                  use non-uniform refinement.
+  --resplit             force re-do GS split.
+  --workers WORKERS     number of workers to run CryoSPARC job, unlimited by default.
+```
+
+There are several useful remarks:
+
+- The `cryosieve-csrhbfactor` program shares most parameters with `cryosieve-csrefine`, and their usage is similar.
+- Estimating the Rosenthal-Henderson B-factor involves a computationally intensive process. It requires iteratively halving the particle dataset and estimating the resolutions for each subset. For example, if you want to estimate the Rosenthal-Henderson B-factors for all 10 output stacks from the previous demo, and you choose to perform 3 trials with each stack using up to 4th halves, it would involve a total of 10 * 3 * (4 + 1) = 150 rounds of 3D-refinement.
+
+# Release Note
+
+* Version 1.2.5:
+  - Add two new programs: `cryosieve-csrefine` and `cryosieve-csrhbfactor`.
+  - Introduce a simplified command for preparing the Conda environment.
+  - Add support for CUDA >=11.8.
+* Version 1.2.4:
+  - Fix the bug occurring with starfile >=0.5. CryoSieve now requires starfile >=0.4, <0.5.
+  - Support gloo backend for multi-GPU version of cryosieve-core.
+  - Fix the bug of SequentialSampler occurring with pytorch >=2.
+* Version 1.2.3: Add new video tutorial.
+* Version 1.2.1: fix the bug occurring when multiple optic groups are present in a star file.
+* Version 1.2: Initial stable release.
```

