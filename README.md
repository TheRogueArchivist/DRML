# DRML
Welcome to DRML, the DRM Library! Here you'll find my various research, notes, and random information about various kinds of DRM, and DRM tangential information.

This library is made in tandem with my work on [BurnOutSharp](https://github.com/mnadareski/BurnOutSharp), which is where the more exact details of how these DRM schemes can be detected will continue to be found.

DRML itself is licensed under [CC0](https://creativecommons.org/share-your-work/public-domain/cc0/), which of course does *not* extend to anything linked in this library. Anything linked is referenced for further research or as a citation only. Also of note, ANY AND ALL LINKED RESOURCES, ESPECIALLY (BUT NOT ONLY) EXECUTABLES, ARE NOT GUARANTEED TO BE SAFE. Although I'll do my best to specifically warn if anything seems especially dodgy, any and all external resources should be treated with care and not be explicitly trusted.


# Guides
* "How to detect PC DRM in optical media." (TODO)


# Library
## Anti-Cheat
### TODO
## Copy Protection
### TODO
## Packers
### TODO


# Addenda
## Additional DRM resources
* ["CD Cracking Uncovered: Protection Against Unsanctioned CD Copying" by Kris Kaspersky](https://archive.org/details/CDCrackingUncoveredProtectionAgainstUnsanctionedCDCopyingKrisKaspersky)
* [CD Media World's "CD/DVD/Media Protections"](https://www.cdmediaworld.com/hardware/cdrom/cd_protections.shtml) (WARNING: Site contains *many* ads, some of which are suggestive and possibly NSFW, and aren't blocked by all ad-blockers)
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
