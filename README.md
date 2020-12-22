# Fortune Files

Quote databases have a line or lines containing a quote, then a line that only contains a '%' (percent sign) to separate it from the others.  ex:

    Let's just pretend Quote 1 is very
    ...very...
    ...very...
    long.
    %
    and quote 2 is short
    %

after adding or altering a new file recreate the index files for

    strfile <filename>

you can compile every fortune file in this directory with `make`

use these with `fortune` like:

    fortune ~/path/to/this/repo/named/fortunes

or you can combine these with the fortune files already on your system by asking fortune where it's databases are like so:

    fortune ~/path/to/this/repo/named/fortunes $(fortune -f 2>&1 | head -n1 | cut -d' ' -f2)


* [Makefile](Makefile):
  make & update new fortune files with `make`
* [handey](handey):
  Jack Handey quotes, because you're good enough, you're smart enough, and
  gosh-darnit people like you.
* [chuckfacts](chuckfacts):
  Facts about Chuck Norris (because 2005 should never end)
* [memebomb](memebomb):
  [Discordian memebombs][1] scraped with [kwotes.py][2]
* [yow](yow):
  The file consists of Zippy the Pinhead quotations (from various comic books and
  strips by Bill Griffith) notable accesible using the the m-x yow command in GNU Emacs.
* [Oblique Strategies](ObliqueStrategies): Brian Eno's Oblique Strategies cards
  to help you get out of a creative rut.
* [Real Facts](realfacts) as real as Snapple makes 'em!
* [English As She Is Spoke](EnglishAsSheIsSpoke) Familiar Phrases, Idiotisms\[sic\] and Proverbs, and Anecdotes as found in [English As She Is Spoke, or A Jest in Somber Earnest](http://www.gutenberg.org/cache/epub/30411/pg30411-images.html)
* [rfc1925](rfc1925) is taken from [IETF Network Working Group RFC 1925: The Twelve Networking Truths](https://www.ietf.org/rfc/rfc1925.txt)
* [The Seventy Maxims of Maximally Effective Mercenaries](SeventyMaximsOfMaximallyEffectiveMercenaries) is taken from the [Schlock Mercenary][3] webcomic.
* [Enkiv2's Glossary of Tech Industry Terms](enkiv2s-glossary-of-tech-industry-terms) taken from [A short glossary of tech industry terms][7]
* [The Holy Bible: Abridged beyond the point of usefulness](BibleAbridged) by Zach Weinersmith, 2015. Some Rights Reserved.  [Attribution-Noncommercial 3.0 Unported](http://creativecommons.org/licenses/by-nc/3.0/)
* [Anathem Glossary](anathem-glossary) from [Anathem by Neal Stephenson][8], as compiled by [David Blume][9]
* [Infinite States](infinitestates) from [Fortunate by Mr Led][10] (P.S. check out this link for a neat "twitter to fortune file" script)
* Many other quotes manualy collected, scraped from [goodreads][4] or [brainyquotes][5], or from random sites with my [page-scraping bookmarklet, found here.][6]

[1]: http://principiadiscordia.com/memebombs/
[2]: https://gist.github.com/JKirchartz/5383142
[3]: http://SchlockMercenary.com
[4]: https://gist.github.com/JKirchartz/80ad6ec90d44b58486db89058d2fdb37
[5]: https://gist.github.com/JKirchartz/05b1132a1151bb497bb408fdf4d0cc56
[6]: http://jkirchartz.com/demos/bookmarklets.html
[7]: https://medium.com/@enkiv2/a-short-glossary-of-tech-industry-terms-4b5f9fef8db3
[8]: https://en.wikipedia.org/wiki/Anathem
[9]: http://anathem.dlma.com/
[10]: https://github.com/mrled/fortunate
