SIMPLY SCHEME INSTALLATION INSTRUCTIONS
=======================================

Written by David Zabel 8/22/93 zabel@cory.eecs.berkeley.edu.
Updated 8/4/97 by bh for Win95.

This disk includes three sets of files:
	* the SCM interpreter for Scheme
	* the Scheme programs for CS 3 and CS 61A
	* the JOVE text editor (a dialect of EMACS) for use with SCM


DOS/WINDOWS INSTALLATION:
-------------------------

0.  If running Windows, open a DOS window.  Trust me, if you just
    run the installer by double-clicking on it, you'll be sorry.

1.  Install the program files on your hard disk:

    If you have the diskette in drive A, type this command:

	a:scmzip -d c:\

    If the diskette is in drive B, then type

	b:scmzip -d c:\

2.  [DOS users only]  Modify autoexec.bat:

	a)  Use your favorite text editor to add the following lines to
	  your autoexec.bat:

		SET SCM_INIT_PATH=C:\SCM\INIT.SCM
		SET SCHEME_LIBRARY_PATH=C:\SCM\SLIB\
		SET EDITOR=JOVE
		SET JOVERC=C:\SCM\JOVE.RC
		SET DESCRIBE=C:\SCM\CMDS.DOC

	b) Add C:\SCM to your PATH statement.

(To edit and then load a Scheme file from inside SCM, say
	(edit "filename")
which will start JOVE, then load the file after you exit JOVE.)

2.  [Windows users]  The SCM directory includes a file named
WSCM.BAT, which will probably appear on your screen as WSCM with
an icon consisting of a gear inside a box.  This is what you
double-click on to run SCM -- *not* the SCM.EXE icon.

You may feel free to make a shortcut to WSCM to put on the
desktop.

3.  The first time you run SCM, it will ask you which textbook
you're using, in order to select the proper initialization file.
Once you've made that choice, it won't ask again.
