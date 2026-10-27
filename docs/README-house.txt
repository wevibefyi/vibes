House Book, House Sans and House Typewriter
===========================================

These three fonts are modified versions of New Computer Modern 8.1.1, by Antonis
Tsolomitis, itself based on Donald Knuth's Computer Modern.

  House Book        from NewCM10-Book.otf      -> house-book.woff2
  House Sans        from NewCMSans10-Book.otf  -> house-sans.woff2
  House Typewriter  from NewCMMono10-Book.otf  -> house-typewriter.woff2

The original
------------

New Computer Modern is distributed on CTAN at

  https://ctan.org/pkg/newcomputermodern

under the GNU General Public License version 3 or later with the font exception,
or the GUST Font License (the LaTeX Project Public License 1.3c, with a request
that derived works be renamed). These modified versions are distributed under the
GUST Font License. The complete, unmodified originals are always obtainable from the
address above.

What was changed
----------------

1. Subset to 280 characters: printable ASCII, Latin-1, general punctuation
   (U+2010-2027, U+2030-203A), four arrows (U+2190-2193), the Greek alphabet with
   accented lower case, and the Middle English letters thorn, eth, yogh and wynn.
2. OpenType layout features kept: kern, liga, locl, smcp, c2sc, onum, lnum, pnum,
   tnum, frac, hist, mark, mkmk (those the original carries). All others removed.
3. The FontForge metadata tables FFTM and PfEd removed.
4. Renamed, at the GUST Font License's request: family "House Book", "House Sans"
   and "House Typewriter", PostScript names HouseBook-Regular, HouseSans-Regular
   and HouseTypewriter-Regular. The name table's description field carries a short
   form of this notice.
5. Converted to WOFF2.

They were made with the fontTools subsetter from the three original files named above.

Support
-------

Neither Antonis Tsolomitis nor Donald Knuth, nor anyone else involved with the
originals, provides any support for these modified versions. Questions about them
belong here, not upstream.
