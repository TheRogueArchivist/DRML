# DRML
Welcome to DRML, the DRM Library! Here you'll find my various research, notes, and random information about various kinds of DRM, and DRM tangential information.

This library is made in tandem with my work on [BurnOutSharp](https://github.com/mnadareski/BurnOutSharp), which is where the more exact details of how these DRM schemes can be detected will continue to be found.
There is a heavy skew toward optical media DRM due it's prevalence, (relative) ease to catalogue, and the importance of knowing what DRM is being used in order to be properly archived.
That being said, any form of DRM that can be consistently detected is considered to be in-scope, though some protections may not be fully covered for several reasons, such as CSS/AACS, which is documented in depth in a multitude of other places. 

DRML itself is licensed under [CC0](https://creativecommons.org/share-your-work/public-domain/cc0/), which of course does *not* extend to anything linked in this library. Anything linked is referenced for further research or as a citation only. Also of note, ANY AND ALL LINKED RESOURCES, ESPECIALLY (BUT NOT ONLY) EXECUTABLES, ARE NOT GUARANTEED TO BE SAFE. Although I'll do my best to specifically warn if anything seems especially dodgy, any and all external resources should be treated with care and not be explicitly trusted.

## Disclaimer
All information contained in this project is published for general information purposes only and in good faith.
Any trademarks mentioned here are registered or copyrighted by their respective owners.
I make no warranties about the completeness, correctness, accuracy and reliability of the information contained in this project.
This project is provided "AS IS" without warranty of any kind.
Any action you take upon the information you find on this document is strictly at your own risk. Under no circumstances will I be held responsible or liable in any way for any damages, losses, costs, or liabilities whatsoever resulting or arising directly or indirectly from your use of this project. You alone are fully responsible for your actions.

# Guides
* "How to detect PC DRM in optical media." (TODO)


# Library
## Anti-Cheat
### TODO
## Optical Copy Protection
### [Bitpool](./entries/Bitpool.md)
### [Cenega ProtectDVD](./entries/Cenega_ProtectDVD.md)
## Packers
### TODO
## Unknown / No Samples
### [Alcatraz](./entries/Alcatraz.md)
### [Roxxe](./entries/Roxxe.md)


# Addenda
## Additional DRM resources
* ["CD Cracking Uncovered: Protection Against Unsanctioned CD Copying" by Kris Kaspersky](https://archive.org/details/CDCrackingUncoveredProtectionAgainstUnsanctionedCDCopyingKrisKaspersky)
* [CD Media World's "CD/DVD/Media Protections"](https://www.cdmediaworld.com/hardware/cdrom/cd_protections.shtml) (WARNING: Site contains *many* ads, some of which are suggestive and possibly NSFW, and aren't blocked by all ad-blockers)
* [Collection of Copy Protected MDS Files](https://archive.org/details/collection-of-copy-protected-mds-files)
## DRM Detection Tools
### Please note that all the software below is linked with absolutely no guarantees whatsoever. Although they are noted here, they have not all been investigated for malware, catasrophic bugs, and so on. Use with caution.
* [A-Ray Scanner](https://web.archive.org/web/20050528202640/http://www.aray-software.com/index.php?showtopic=55) - Development long since halted, closed source, but is able to detect a fair number of protections. Is also able to perform sector scanning.
* [BurnOut](http://burnout.sourceforge.net/) - Development halted, open source. Is completely superseded by BurnOutSharp, which was created based on it's source.
* [BurnOutSharp](https://github.com/mnadareski/BurnOutSharp) - Actively developed, open-source, and able to detect a majority of the DRM that all other scanners are able to. Limited to filesystem only checks as of right now.
* [ClonyXXL](https://web.archive.org/web/20030209022858/http://clony.smokers-board.de:80/) - Development halted, closed-source, has a few odd-ball detections missed by other software. Also includes a few novel features, such as checking for the presence of bad sectors on a disc, or monitoring the system for when specific protected games are launched. [Download](https://cmw.mobiletarget.net/?f=ClonyXXL.zip).
* [Detect It Easy](https://github.com/horsicq/Detect-It-Easy) - Actively developed, open-source, but not exactly a DRM scanner per se. It's a more general file-type scanner, but it is able to detect some forms of DRM.
* [ProtectionID](https://web.archive.org/web/20210331144912/https://protectionid.net/) - Development currently stopped, closed-source, but generally considered the most complete option at the moment. Includes the ability to scan for the presence of DRM via sector scanning, and not just filesystem checks. [Download](https://web.archive.org/web/20180909104700/https://pid.wiretarget.com/?f=ProtectionId.690.December.2017.rar).
## Glossaries
* "Glossary of protection features used by DRM." (TODO)
## Lists of copy protected optical media
* http://cpdb.kemuri-net.com/ 
* [Official list of music CDs with the XCP copy protection](https://web.archive.org/web/20071012024250/http://cp.sonybmg.com/xcp/english/titles.html)
* ["List of compact discs sold with MediaMax CD-3" (From Wikipedia)](https://en.m.wikipedia.org/wiki/List_of_compact_discs_sold_with_MediaMax_CD-3)
* https://web.archive.org/web/20170222085203/http://forum.daemon-tools.cc/gamedb.php?letter=all
* https://web.archive.org/web/20040816080838/http://forum.copybase.ch/de/index.php?showtopic=1624
* https://web.archive.org/web/20191230172450/http://nocccd.noihjp.com/Problems.php
* https://web.archive.org/web/20050407205157/http://www.cdlogo.nl/cd-beveiliging/pagina.asp?pagkey=23577&formposted=yes&formname=docsearch23577&templateid=10&fullsearchtemplate=10&fullsearchvalue=%25 (List of copy protected music CDs from the Netherlands).
* https://web.archive.org/web/20210331144912/https://protectionid.net/
* http://www12.plala.or.jp/t2-bun/
* http://redump.org/discs/quicksearch/EXAMPLE/protection/only (NOTE: You have to manually replace "EXAMPLE" in the URL with what you want to search for).
* http://fileforums.com/forumdisplay.php?f=37
## Lists of copy protected digital media
* http://green.ribbon.to/~erog/GIGA/Acti.html (Japanese, focused on online activation DRM)
