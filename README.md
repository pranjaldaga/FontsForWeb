FontsForWeb
===========

FontsForWeb creates fonts for web browsers.

About
-----

FontsForWeb takes a directory containing ttf(TrueType Font) files and generates woff, eot and svg font files for cross-browser web font embedding via CSS.

You may either change to the fonts directory and simply run the command `webfonts` or run the command from anywhere followed by the path to the fonts directory.

By default the web fonts will be generated into the original fonts directory. You may optionally add the -o followed by a path to copy the original ttfs and generate the web fonts into a different directory.

Recommended CSS for Embedding
-----------------------------

	@font-face {
	  font-family: '<Font Name>';
	  src: url('fonts/<fontname>.eot');
	  src: url('fonts/<fontname>.eot?iefix') format('eot'),
	    url('fonts/<fontname>.woff') format('woff'),
	    url('fonts/<fontname>.ttf') format('truetype'),
	    url('fonts/<fontname>.svg#<fontname>') format('svg');
	  font-style: normal;
	  font-weight: normal;
	}
