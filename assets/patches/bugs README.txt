19980303  shc@cfg.com

This change corrects a problem which is evidenced by special characters
being taken as data special characters in data items.  To date, it
has appeared only under Digital UNIX on Alphas.

The file 'patch.19980303' is a context diff showing the additions.

To install the changes, change to the pdl/81 style library directory
(usually /usr/lib/pdl81) and execute

	patch <patch.19980303

You will then need to rebuild the PDL/81 processor.

Note that the above assumes that you have a copy of Larry Wall's patch
utility.  If you don't, and don't want to get one, these patches can
be applied by hand.

Steve Caine // shc@cfg.com