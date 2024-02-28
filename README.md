# DRML
Welcome to DRML, the DRM Library! Here you'll find my various research, notes, and random information about various kinds of DRM, and DRM-tangential information.

This library is made in tandem with my work on [BinaryObjectScanner](https://github.com/SabreTools/BinaryObjectScanner), which is where the more exact details of how these DRM schemes can be detected will continue to be found.
There is a heavy skew toward optical media DRM due to its prevalence, (relative) ease to catalogue, and the importance of knowing which DRM is being used in order to be properly archived.
That being said, any form of DRM that can be consistently detected is within the scope of the library, though some protections may not be fully covered for several reasons, such as CSS/AACS, which is documented in depth in a multitude of other places.

DRML itself is licensed under [CC0](https://creativecommons.org/share-your-work/public-domain/cc0/), which of course does *not* extend to anything linked in this library. Anything linked is referenced for further research or as a citation only. Also of note, ANY AND ALL LINKED RESOURCES, ESPECIALLY (BUT NOT ONLY) EXECUTABLES, ARE NOT GUARANTEED TO BE SAFE. Although I'll do my best to specifically warn if anything seems especially dodgy, any and all external resources should be treated with care and not be explicitly trusted.

## Disclaimer
All information contained in this project is published for general information purposes only and in good faith.
Any trademarks mentioned here are registered or copyrighted by their respective owners.
I make no warranties about the completeness, correctness, accuracy and reliability of the information contained in this project.
This project is provided "AS IS" without warranty of any kind.
Any action you take upon the information you find on this document is strictly at your own risk. Under no circumstances will I be held responsible or liable in any way for any damages, losses, costs, or liabilities whatsoever resulting or arising directly or indirectly from your use of this project. You alone are fully responsible for your actions.

# Guides

* [What’s the Most Convenient Optical Image Format for Daily Use?](./Guides/Image_Formats.md)
* "How to detect PC DRM in optical media." (TODO)


# Library
## Anti-Cheat
### [Denuvo Anti-Cheat](./entries/Denuvo_Anti-Cheat/Denuvo_Anti-Cheat.md)
## Audio CD Protection
### [CopyKiller](./entries/CopyKiller/CopyKiller.md)
### [MediaCloQ](./entries/MediaCloQ/MediaCloQ.md)
## DRM Builder
### [CopyKiller](./entries/CopyKiller/CopyKiller.md)
### [Freelock](./entries/Freelock/Freelock.md)
## Multimedia DRM
### [PlayJ](./entries/PlayJ/PlayJ.md)
## Optical Copy Protection
### [Bitpool](./entries/Bitpool/Bitpool.md)
### [Cenega ProtectDVD](./entries/Cenega_ProtectDVD/Cenega_ProtectDVD.md)
### [CopyKiller](./entries/CopyKiller/CopyKiller.md)
### [DigiGuard](./entries/DigiGuard/DigiGuard.md)
### [engine32](./entries/engine32/engine32.md)
### [Freelock](./entries/Freelock/Freelock.md)
### [MediaCloQ](./entries/MediaCloQ/MediaCloQ.md)
### [phenoProtect](./entries/phenoProtect/phenoProtect.md)
## Packers
### TODO
## Unknown / No Samples
### [Alcatraz](./entries/Alcatraz/Alcatraz.md)
### [Roxxe](./entries/Roxxe/Roxxe.md)


# Addenda
## Additional DRM resources
* ["CD Cracking Uncovered: Protection Against Unsanctioned CD Copying" by Kris Kaspersky](https://archive.org/details/CDCrackingUncoveredProtectionAgainstUnsanctionedCDCopyingKrisKaspersky)
* [CD Media World's "CD/DVD/Media Protections"](https://www.cdmediaworld.com/hardware/cdrom/cd_protections.shtml) (WARNING: Site contains *many* ads, some of which are suggestive and possibly NSFW, and aren't blocked by all ad-blockers)
* [Collection of Copy Protected MDS Files](https://archive.org/details/collection-of-copy-protected-mds-files)
* [Website that includes various technical papers, including several about reverse engineering DRM.](https://www.lucadamico.dev/)
## DRM Detection Tools
### Please note that all the software below is linked with absolutely no guarantees whatsoever. Although they are noted here, they have not all been investigated for malware, catasrophic bugs, and so on. Use with caution.
* [A-Ray Scanner](https://web.archive.org/web/20050528202640/http://www.aray-software.com/index.php?showtopic=55) - Development long since halted, closed-source, but can detect a fair number of protections. Can also perform sector scanning.
* [BurnOut](http://burnout.sourceforge.net/) - Development halted, open-source. Fully superseded by its C# fork, BurnOutSharp.
* [BurnOutSharp](https://github.com/mnadareski/BurnOutSharp) - Actively developed, open-source, and can detect a majority of the DRM that all other scanners can. Currently limited to filesystem checks.
* [ClonyXXL](https://web.archive.org/web/20030209022858/http://clony.smokers-board.de:80/) - Development halted, closed-source, has a few oddball detections missed by other software. Also includes a few novel features, such as checking for the presence of bad sectors on a disc, or monitoring the system for when specific protected games are launched. [Download](https://web.archive.org/web/20200507185551/cmw.mobiletarget.net/?f=ClonyXXL.zip).
* [Detect It Easy](https://github.com/horsicq/Detect-It-Easy) - Actively developed, open-source, but not exactly a DRM scanner per se, more of a general file-type scanner. However, it can detect some forms of DRM.
* [ProtectionID](https://web.archive.org/web/20210331144912/https://protectionid.net/) - Development currently stopped, closed-source, but generally considered the most complete option at the moment. Includes the ability to scan for the presence of DRM via sector scanning, and not just filesystem checks. [Download](https://web.archive.org/web/20180909104700/https://pid.wiretarget.com/?f=ProtectionId.690.December.2017.rar).
## Glossaries
* "Glossary of protection features used by DRM." (TODO)
## Lists of copy protected optical media
* http://cpdb.kemuri-net.com/ 
* [Official list of music CDs with the XCP copy protection.](https://web.archive.org/web/20071012024250/http://cp.sonybmg.com/xcp/english/titles.html)
* ["List of compact discs sold with MediaMax CD-3" (From Wikipedia)](https://en.m.wikipedia.org/wiki/List_of_compact_discs_sold_with_MediaMax_CD-3)
* [List of copy-protected games from the devs of Daemon Tools.](https://web.archive.org/web/20170222085203/http://forum.daemon-tools.cc/gamedb.php?letter=all)
* [German forum post linking to and explaining the "Copybase" database, an XML database containing numberous discs and their copy protections. (2004-08-16)](https://web.archive.org/web/20040816080838/http://forum.copybase.ch/de/index.php?showtopic=1624)
* [The XML file containing the previously mentioned Copybase database. (2004-07-14)](https://web.archive.org/web/20040714135732/http://copybase.ch/XML/Database/index.xml)
* https://web.archive.org/web/20191230172450/http://nocccd.noihjp.com/Problems.php
* https://web.archive.org/web/20050407205157/http://www.cdlogo.nl/cd-beveiliging/pagina.asp?pagkey=23577&formposted=yes&formname=docsearch23577&templateid=10&fullsearchtemplate=10&fullsearchvalue=%25 (List of copy protected music CDs from the Netherlands.)
* [Changelog for Protection ID, which includes specific details about multiple types of DRM.](https://web.archive.org/web/20210331144912/https://protectionid.net/)
* http://www12.plala.or.jp/t2-bun/
* http://redump.org/discs/quicksearch/EXAMPLE/protection/only (NOTE: Replace "EXAMPLE" in the URL with what you want to search for.)
* http://fileforums.com/forumdisplay.php?f=37
* [Australian website that has a list of copy-protected games.](https://web.archive.org/web/20030226122451/http://www.users.bigpond.net.au/portmac/index.htm)
* http://www.projectkaigo.org/grprotected.html
* [German copy protection database software. (Possibly not final DB version)](https://web.archive.org/web/20020221142949/http://www.isis.de:80/members/~awenderh/tccd/TCCD26BDE.exe)
* [German list of copy protected games and what versions of CloneCD can dump them.](http://dl.seite.net/cgi-bin/baseportal.pl?htx=/clonecd/main&range=0,737)
## Lists of copy protected digital media
* [Steam collection of games that have been protected with Denuvo Anti-Tamper.](https://store.steampowered.com/curator/26095454-Denuvo-Games/)
* [List of games that have been protected with Denuvo Anti-Tamper.](https://www.game-debate.com/games/gamesWithDenuvo)
* http://green.ribbon.to/~erog/GIGA/Acti.html (Japanese, focused on online activation DRM)
