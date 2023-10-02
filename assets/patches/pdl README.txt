
19970505  shc@cfg.com

These changes correct printing of dates on or after 2000/01/01.  They are
applied to the ada, design, man2167, text, manual, and letter styles.

After these changes are applied, the year portion of a date should be
displayed as four digits.

The file 'patch.19970505' is a context diff showing the additions.

To install the changes, change to the pdl/81 style library directory
(usually /usr/lib/pdl81) and execute

	patch <patch.19970505

which will save the old files with a ".orig" suffix and create modified
versions of the files.

Note that the above assumes that you have a copy of Larry Wall's patch
utility.  If you don't, and don't want to get one, these patches can
be applied by hand.

Steve Caine // shc@cfg.com