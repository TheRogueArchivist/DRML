### Names:

phenoProtect[^1], PhenoProtect[^2], Phenoprotect[^3], Pheno Protect[^4]

### Developers:

Codecult Software Research & Development GmbH[^8] (AKA Codecult[^8], codecult[^8], and CodeCult[^5]), Phenomedia AG[^5]

### Years Active: 

~2001[^9]-~2002[^5]

### Known Versions & Differences: 

Version 1.0:[^3] The initial version, very few sources mention this version specifically existing but is presumably the version present on "Carrera Grand Prix".

Version 2.0:[^5] No games are known to use this version, though one forum post indicates that it used a serial number check.[^6]

### Known Samples: 

#### Confirmed: 

* Carrera Grand Prix.[^9]

#### Unconfirmed:

* Another War.[^3] [^7] [^8]

* Mega Race 3.[^3] [^7]

* RollerCoaster Factory.[^3]

* Simon the Sorcerer 3D.[^7]

* ZanZarah.[^5] [^7]

### Categories: 

Optical Copy Protection

### Protection Features:

Bad sectors [TODO: Verify what kind], Disc check [TODO: Confirm this is part of phenoProtect itself], Serial[^6] (Unconfirmed)

### Minimum Required Image Format to Run:

CUE[^12]

### Software Known to Detect:

BurnOutSharp[^10], ClonyXXL[^11]


### Preservation Instructions:

[TODO]

### Overall Description:

The DRM phenoProtect was a copy protection created by Codecult,[^5] whose parent company at the time was Phenomedia AG.[^8] In 2002, Phenomedia AG became insolvent,[^12] and Codecult would become part of "H2Labs Creative Research GmbH" as of 2002-08-28.[^14] It seems that phenoProtect, both in branding and technology, was abandoned as of this point.

It was seemingly used in several games during this time period, but the only one currently confirmed is "Carrera Grand Prix"[^9]. PhenoProtect itself seems to make use of a "signature" using bad sectors on the disc to validate the authenticity of the media. The exact type of errors aren't currently known, but don't appear to be C2 errors. 

The main protection check is triggered during installation, and appears to be implemented entirely within the InstallShield compiled script. There's a secondary disc check present when attempting to launch the game itself, though this appears to only check for the presence of the disc, no signature check is apparently performed. It's currently unknown if this disc check is part of phenoProtect itself, or if this was an extra check added by the game developers. Further testing is required, as I haven't been personally able to run the game whatsoever. This, however, appears to be a game crash and not a failed protection check.

#### Known Associated Files:

N/A.

#### Game Specific Files:

N/A.

#### Known Associated Executable Sections:

N/A.

### Media:

1. [^15] !["Warning" - "phenoProtect not found on CD-ROM!](./phenoProtect_Error_English.png "English phenoProtect Error Message")
2. [^15] !["Avertissement" - "PhenoProtect introuvable sur le disque!](./phenoProtect_Error_French.png "French phenoProtect Error Message")
3. [^15] !["Warnung" - "phenoProtect wurde nicht auf der CD-ROM gefunden!](./phenoProtect_Error_German.png "German phenoProtect Error Message")

### Additional Resources:

1. [CD Media World page for phenoProtect.](https://www.cdmediaworld.com/hardware/cdrom/cd_protections_phenoprotect.shtml)
2. [German manual that briefly describes phenoProtect.](https://www.manualslib.de/manual/174345/I-Tv-Group-Smart.html?page=28#manual)
3. [Entry in German DRM list for "Carrera Grand Prix".](http://dl.seite.net/cgi-bin/baseportal.pl?htx=/clonecd/main&cmd=list&range=0,20&Titel~=C&cmd=all&Id=1003)
4. [World of Gothic forum post that mentions CodeCult and phenoProtect.](https://forum.worldofplayers.de/forum/threads/1551291-PB-Project-Zerberus/page3)
5. [Slideshow about DRM that lists phenoProtect.](https://slideplayer.com/slide/3863342/)
6. [Information about and timeline for Codecult.](https://www.northdata.com/codecult+software+research+%26+development+GmbH,+Bochum/HRB+6572)
7. [Website that lists "Another War" as containing phenoProtect.](https://www.uvlist.net/groups/info/phenoprotect)
8. [World of Gothic forum post that gives backstory about CodeCult and CodeCreature.](https://forum.worldofplayers.de/forum/threads/1553764-CC-PB-Relations-of-PB-s-very-own-Genome-Engine-to-the-CodeCult-CodeCreatures-engine)
9. [FileForums forum post that briefly explains phenoProtect 2.](https://fileforums.com/archive/index.php/t-62914.html)
10. [BurnOutSharp source code for phenoProtect.](https://github.com/mnadareski/BurnOutSharp/blob/master/BurnOutSharp/ProtectionType/Phenoprotect.cs)
11. [Official Codecult website. (Mostly Broken) (2001-03-02)](https://web.archive.org/web/20010302232209/http://www.codecult.com/)
12. [Official Codecult website. (Post-Phenomedia) (2003-02-01)](https://web.archive.org/web/20030201231731if_/http://www.codecult.com:80/)
13. [List of DRM protected games from Daemon Tools that contains several phenoProtect games. (2017-02-22)](https://web.archive.org/web/20170222085203/http://forum.daemon-tools.cc/gamedb.php?letter=all)
14. [Redump entry for "Carrera Grand Prix", a game that contains phenoProtect.](http://redump.org/disc/84082)
15. [All Redump entries listed as having phenoProtect as a protection.](http://redump.org/discs/quicksearch/phenoProtect/protection/only)
16. [DIC GitHub Readme that mentions phenoProtect.](https://github.com/saramibreak/DiscImageCreator)
17. [BurnOutSharp source code for detecting phenoProtect.](https://github.com/mnadareski/BurnOutSharp/blob/master/BurnOutSharp/ProtectionType/Phenoprotect.cs)
18. [GBATemp page for ClonnyXXL.](https://gbatemp.net/download/clonyxxl.37819/)
19. [German Wikipedia article for Phenomedia (The English version simply redirects to the page for their most well-known game series, Moorhuhn).](https://de.wikipedia.org/wiki/Phenomedia)
20. [Official Phenomedia AG website with news headlines regarding the company. (Mostly broken, the news links on the page are completely broken) (2002-06-06)](https://web.archive.org/web/20020606172205/http://www.phenomedia.com/neu/index.html)
21. [Mobygames page that gives a timeline for the history of "phenomedia publishing gmbh".](https://www.mobygames.com/company/phenomedia-publishing-gmbh/history)
22. [Archive of news reports regarding Phenomedia AG.](https://www.eqs-news.com/company/phenomedia-ag/news/5b6d2b45-ea7c-11e8-902f-2c44fd856d8c)
23. [News report regarding Phenomedia AG's insolvency.](https://www.eqs-news.com/news/adhoc/phenomedia-ag-english/32173)
24. [Official Codecult press release regarding CodeCreatures' continued development post Phenomedia AG. (2003-02-28)](https://web.archive.org/web/20030228062718fw_/http://www.codecult.com/main.asp?page=Press_News_Show&id=20)

### Footnotes:

[^1]: Media #1.

[^2]: Media #2.

[^3]: Additional Resource #1.

[^4]: Additional Resource #3.

[^5]: Additional Resource #4.

[^6]: Additional Resource #9.

[^7]: Additional Resource #13.

[^8]: Additional Resource #7.

[^9]: Additional Resource #14.

[^10]: Additional Resource #17.

[^11]: Additional Resource #18.

[^12]: This has been confirmed personally, and is because phenoProtect checks for the bad sectors that aren't present in an ISO image.

[^13]: Additional Resource #23.

[^14]: Additional Resource #24.

[^15]: [Found in Redump entry 84082.](http://redump.org/disc/84082)