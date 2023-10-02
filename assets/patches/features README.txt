960514  shc

These changes introduce a %asis / %noasis command pair for use in
flow segments.  All formatting is turned off between them.

The new commands are implemented by adding them to the end of the 'design'
style file.  The file 'patch.960514' is a context diff showing the additions.

To install the changes, change to the pdl/81 style library directory
(usually /usr/lib/pdl81) and execute

	patch design patch.960514

which will save the old design file as design.orig and make a new 'design'
with the patch applied.

Note that the above assumes that you have a copy of Larry Wall's patch
utility.  If you don't, and don't want to get one, this patch can easily
be applied by hand since all changes are at the end of the file.

The new commands are effective only within a flow segment (%s).  The command

	%asis

turns off all formatting and data item definition and referencing.  The
command

	%noasis

retuns things to the normal mode.


Steve Caine // shc@cfg.com
