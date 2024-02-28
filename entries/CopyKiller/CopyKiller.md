### Names:

CopyKiller[^CopyKiller_Website_2003], CK[^CopyKiller_English_Website_2003]

[^CopyKiller_Website_2003]: [CopyKiller website landing page. (Archived 2003-03-12)](https://web.archive.org/web/20030312200712/http://www.webstylerzone.com/CopyKiller/index.htm)

[^CopyKiller_English_Website_2003]: [CopyKiller English website. (Archived 2003-03-13)](https://web.archive.org/web/20030313040938/http://www.webstylerzone.com/CopyKiller/En/index.htm)

***

### Developers:

WebStylerZone / Tom Commander[^CopyKiller_Website_2003]

***

### Years Active: 

2001(?)[^CopyKiller_Website_2003] - 2006/2007(?)[^WebStylerZone_Website_English_2007]

[^WebStylerZone_Website_English_2007]: [WebStylerZone English website.(Archived 2007-07-21)](https://web.archive.org/web/20070721070430/http://www.webstylerzone.com/en/index.htm)

***

### Known Versions & Differences: 

[TODO: Add more information about what each version changes, preferably from an official changelog, if available.]

* 3.62: First documented release. An installer for this version is available.[^CK_Install_3.62]
* 3.64: An installer for this version is available.[^CK_Install_3.64]
* 4.00 alpha build 20: Seemingly the only known public build of 4.X. It appears to have only been available through the not well-preserved WebStylerZone forum[^WebStylerZone_Website_English_2007], and so is currently lost.
* 3.99: This version is based on the 4.00 alpha[^WebStylerZone_Website_English_2007], and even still refers to itself as "CopyKillerV4" internally. An installer for this version is available.[^CK_Install_3.99]
* 3.99a: Final version. Released shortly after 3.99, and may be a big fix update. An installer[^CK_Install_3.99a] (and portable zip[^CK_Zip_3.99a]) for this version is available.

[^CK_Install_3.62]: [CopyKiller 3.62 Installer. (Archived 2003-11-30)]( https://web.archive.org/web/20031130192048/http://www.webstylerzone.com/Downloads/Brennertools/CopyKiller-Setup.exe)

[^CK_Install_3.64]: [CopyKiller 3.64 Installer. (Archived 2006-05-24)](https://web.archive.org/web/20060524220845/http://download.webstylerzone.com:80/exe/CopyKiller-Setup.exe)

[^CK_Install_3.99]: [CopyKiller 3.99 Installer. (2007-01-02)](https://web.archive.org/web/20070102080031/http://download.webstylerzone.com:80/exe/CopyKiller-Setup.exe)

[^CK_Install_3.99a]: [CopyKiller 3.99a Installer. (Archived 2007-07-21)](https://web.archive.org/web/20070721070138/http://www.webstylerzone.com/Downloads/exe/CopyKiller-Setup.exe)

[^CK_Zip_3.99a]: [CopyKiller 3.99a Portable zip. (Archived 2007-07-21)](https://web.archive.org/web/20070721070214/http://www.webstylerzone.com/Downloads/zip/CopyKiller.zip)

***

### Known Samples: 

#### Confirmed: 

* Only the original software used to add this DRM to discs is known, no actual distributed discs using it are currently known.

#### Unconfirmed:

* N/A

***

### Categories: 

DRM Builder, Optical Copy Protection, Audio CD Protection[^WebStylerZone_Burning_Programs]

[^WebStylerZone_Burning_Programs]: [WebStylerZone English "Downloads (Burning)" page. (Archived 2007-08-11)](https://web.archive.org/web/20070811202419/http://www.webstylerzone.com/en/download_brenner_copykiller_safedisc_safediscscanner_whatspeed_copyprotection_copy_protection_protect_cd_cds_audiocd_datacd_against_copying.htm)

***

### Supported Platforms:

* Windows[^WebStylerZone_English_Downloads]

[^WebStylerZone_English_Downloads]: [WebStylerZone English "Downloads" page. (Archived 2007-08-11)](https://web.archive.org/web/20070811202511/http://www.webstylerzone.com/en/downloads_freeware_shareware_copykiller_exeshield_deluxe_pictureviewer_xl_whatspeed_safediscscanner_asciicommander_audiocommander_mathcheater_lol_.htm)

***

### Protection Features:

Copy Prevention(?), Weak Sectors(?)[^WebStylerZone_Burning_Programs]

***

### Software Known to Detect:

A-Ray Scanner[^ARay_GBATemp], BinaryObjectScanner[^CK_BOS], BurnOut[^BurnOut_Changelog]

[^ARay_GBATemp]: [GBATemp page for A-Ray Scanner. (Archived 2023-05-28)](http://web.archive.org/web/20230528222019/https://gbatemp.net/download/a-ray-scanner.37818/)

[^CK_BOS]: [BinaryObjectScanner source code for CopyKiller detection.](https://github.com/SabreTools/BinaryObjectScanner/blob/master/BinaryObjectScanner/Protection/CopyKiller.cs)

[^BurnOut_Changelog]: [BurnOut changelog, which shows detection for CopyKiller being added (and eventually removed). (Archived 2023-10-02)](https://web.archive.org/web/20231002225132/https://www.softpedia.com/progChangelog/BurnOut-Changelog-103960.html)

***

### Preservation Instructions:

N/A

***

### Overall Description:

CopyKiller was a DRM by WebStylerZone / Tom Commander that allowed users to protect their burned discs[^WebStylerZone_Burning_Programs]. It did this by having users add the CopyKiller files to their disc before burning it, including an option AutoRun that presumably checks for the presence/integrity of those files. As far as I can tell, there's no ability to integrate this into an executable or have it do anything but show a pop-up if the check fails.

Because of this, the program itself appears to be mostly useless aside from providing a tutorial for how to add the DRM, as it doesn't appear to automatically add anything itself. It does offer Audio CD protection as well, but the section of the program for that requires you to have the registered version. This means that I have no idea how adding this to an Audio CD would work, or if program actually directly does this rather than just giving a tutorial. It may be intended that you add a data track with CopyKiller to an Audio CD, or that you somehow add the raw data as audio track, but this is speculation.

How this DRM works exactly is currently unknown, as unlike similar DRM (such as [Freelock](../Freelock/Freelock.md)), it doesn't require you to intentionally delete or corrupt files, or otherwise tamper with the burning process. What is known is that it "makes damaged sectors on cd" and it "does not work with every writer, because it uses a firmware error to make the cd copy protected".[^WebStylerZone_Burning_Programs] 

Because of this, I speculate that it contains specific patterns of data within the files that when burned, contain weak sectors. This would then cause susceptible drives with a specific firmware bug to burn the original copies of discs with intentional errors, meaning that anybody who attempts to copy the disc will be met with these errors. The optional autorun likely checks for these files on launch, and either expects these files to be not present on a burned copy at all, or does further checks to see if these files are intact and not simply blank. This needs further testing to verify.

CopyKiller appears to have been created in 2001, but no copies of the program or website have been found from before 2003. And due to the 2003 website having a slightly dynamic layout, most relevant content from it appears to be unarchived. There are also little to no archives of the site between 2003-2007, but there also appear to have been few, if any, significant updates to CopyKiller within this time anyway.

Interestingly, WebStylerZone has had some form of connection with WebToolMaster since at least 2003, as they had a banner for the site up on their main page.[^CopyKiller_English_Website_2003] WebToolMaster has also hosted CopyKiller since 2006.[^WTM_CK_3.64] WebStylerZone hosted WTM CD Protect[^WebStylerZone_Burning_Programs] and had WebToolMaster listed as a partner[^WSZ_Partners_English] since at least 2007. By 2012, WebToolMaster had bought the WebStylerZone domain, making it redirect to their own site, and announced that the project had been cancelled by the original developer.[^WTM_CK_2011] This site is still up to this day, as of 2024-02-27.

[^WTM_CK_3.64]: [WebToolMaster page for CopyKiller 3.64. (Archived 2006-11-09)](https://web.archive.org/web/20061109151642/http://www.webtoolmaster.com/copykiller.htm)

[^WTM_CK_2011]: [WebToolMaster page for CopyKiller, which announces that CopyKiller has been cancelled by the original developer. (Archived 2011-12-16)](https://web.archive.org/web/20111216035125/http://www.webtoolmaster.com:80/copykiller.htm)

[^WSZ_Partners_English]: [WebStylerZone English "Partners" page. (Archived 2007-08-11)](https://web.archive.org/web/20070811202517/http://www.webstylerzone.com/en/partner_banner_partnes_friends_of_webstylerzone_dot_com.htm)

***

#### Known Associated Executable Sections:

N/A

***

#### Known Associated Extensions:

[TODO]

***

#### Known Associated Files:

[TODO]

***

#### Known Associated Magic Numbers:

N/A

***

### Media:

[TODO]

***

### Additional Resources:

#### WebStylerZone/CopyKiller main website:
* [CopyKiller website landing page. (Archived 2003-03-12)](https://web.archive.org/web/20030312200712/http://www.webstylerzone.com/CopyKiller/index.htm)
* [CopyKiller English website. (Archived 2003-03-13)](https://web.archive.org/web/20030313040938/http://www.webstylerzone.com/CopyKiller/En/index.htm)
* [CopyKiller German website. (Archived 2003-03-13)](https://web.archive.org/web/20030313040850/http://www.webstylerzone.com/CopyKiller/De/index.htm)
* [WebStylerZone website landing page. (Archived 2003-04-27)](https://web.archive.org/web/20030427110218/http://www.webstylerzone.com:80/index.htm)
* [WebStylerZone English website. (Archived 2003-03-12)](https://web.archive.org/web/20030312195210/http://www.webstylerzone.com/English/index.htm)
* [WebStylerZone English website. (Archived 2007-07-21)](https://web.archive.org/web/20070721070430/http://www.webstylerzone.com/en/index.htm)
* [WebStylerZone German website. (Archived 2003-03-12)](https://web.archive.org/web/20030312185503/http://www.webstylerzone.com/German/index.htm)
* [WebStylerZone German website. (Archived 2007-07-21)](https://web.archive.org/web/20070721070544/http://www.webstylerzone.com/de/index.htm)
* [WebStylerZone English website changelog. (Archived 2007-08-11)](https://web.archive.org/web/20070811202454/http://www.webstylerzone.com/en/news/change_history_changelog_log_evolution.htm)
* [WebStylerZone German website changelog. (Archived 2007-08-11)](https://web.archive.org/web/20070811202638/http://www.webstylerzone.com/de/news/change_changelog_history_version_information_versionen.htm)
* [WebStylerZone English "Downloads" page. (Archived 2007-08-11)](https://web.archive.org/web/20070811202511/http://www.webstylerzone.com/en/downloads_freeware_shareware_copykiller_exeshield_deluxe_pictureviewer_xl_whatspeed_safediscscanner_asciicommander_audiocommander_mathcheater_lol_.htm)
* [WebStylerZone German "Downloads" page. (Archived 2007-08-11)](https://web.archive.org/web/20070811202728/http://www.webstylerzone.com/de/downloads_freeware_shareware_copykiller_exeshield_deluxe_pictureviewer_xl_whatspeed_safediscscanner_asciicommander_audiocommander_mathcheater_lol_text_crypter.htm)
* [WebStylerZone English "Downloads (Burning)" page. (Archived 2007-08-11)](https://web.archive.org/web/20070811202419/http://www.webstylerzone.com/en/download_brenner_copykiller_safedisc_safediscscanner_whatspeed_copyprotection_copy_protection_protect_cd_cds_audiocd_datacd_against_copying.htm)
* [WebStylerZone German "Downloads (Brenner)" page. (Archived 2007-08-11)](https://web.archive.org/web/20070811202626/http://www.webstylerzone.com/de/download_brenner_download_copykiller_download_safediscscanner_download_whatspeed_kopierschutz_fuer_cds_einfach_und_guenstig.htm)
* [WebStylerZone English "about" page. (Archived 2007-08-11)](https://web.archive.org/web/20070811202429/http://www.webstylerzone.com/en/impressum_about_webstylerzone_about_tom_commander_who_is_responsible_of_webstylerzone.com.htm)
* [WebStylerZone German "Impressum" page. (Archived 2007-08-11)](https://web.archive.org/web/20070811202755/http://www.webstylerzone.com/de/impressum_ueber_tom_commander_commander_tom_verzeichniss_about_verantwortlich_ist_tom_commander_fuer_webstylerzone_com.htm)
* [WebStylerZone English "Partners" page. (Archived 2007-08-11)](https://web.archive.org/web/20070811202517/http://www.webstylerzone.com/en/partner_banner_partnes_friends_of_webstylerzone_dot_com.htm)
* [WebStylerZone German "Partners" page. (Archived 2007-08-11)](https://web.archive.org/web/20070811202743/http://www.webstylerzone.com/de/partner_kollege_banner_tausch_partner_seiten_fans_kollegen_.htm)

#### WebStylerZone forums:
Unfortunately, the forums are very poorly preserved.
* [WebStylerZone English forum page. (Archived 2007-07-21)](https://web.archive.org/web/20070721071134/http://www.webstylerzone.com/en/forum/)
* [WebStylerZone German forum page. (Archived 2007-07-21)](https://web.archive.org/web/20070721070851/http://www.webstylerzone.com/de/forum/)
* [WebStylerZone German forum post detailing their lineup of products. (Posted 2006-10-22) (Archived 2007-08-11)](https://web.archive.org/web/20070811202901/http://www.webstylerzone.com/de/forum/viewtopic.php?f=13&p=133&sid=d67eda2fe83b7e8035a6e5120fae4cae)
* [List of German WebStylerZone forum posts that weren't responded to. (Archived 2007-08-12](https://web.archive.org/web/20070811202913/http://www.webstylerzone.com/de/forum/search.php?search_id=unanswered&sid=d67eda2fe83b7e8035a6e5120fae4cae)

#### WebToolMaster:
* [WebToolMaster page for CopyKiller 3.64. (Archived 2006-11-09)](https://web.archive.org/web/20061109151642/http://www.webtoolmaster.com/copykiller.htm)
* [WebToolMaster page for CopyKiller 3.99. (Archived 2006-11-23)](https://web.archive.org/web/20061123234046/http://www.webtoolmaster.com:80/copykiller.htm)
* [WebToolMaster page for CopyKiller. Doesn't appear to actually contain CopyKiller, only links to WTM's own DRM. (Archived 2009-09-08)](https://web.archive.org/web/20090908151003/http://www.webtoolmaster.com:80/copykiller.htm)
* [WebToolMaster page for CopyKiller, which announces that CopyKiller has been cancelled by the original developer. (Archived 2011-12-16)](https://web.archive.org/web/20111216035125/http://www.webtoolmaster.com:80/copykiller.htm)

#### CopyKiller downloads:
* [CopyKiller 3.62 Installer. (Archived 2003-11-30)]( https://web.archive.org/web/20031130192048/http://www.webstylerzone.com/Downloads/Brennertools/CopyKiller-Setup.exe)
* [CopyKiller 3.64 Installer. (Archived 2006-05-24)](https://web.archive.org/web/20060524220845/http://download.webstylerzone.com:80/exe/CopyKiller-Setup.exe)
* [CopyKiller 3.99 Installer. (2007-01-02)](https://web.archive.org/web/20070102080031/http://download.webstylerzone.com:80/exe/CopyKiller-Setup.exe)
* [CopyKiller 3.99a Installer. (Archived 2007-07-21)](https://web.archive.org/web/20070721070138/http://www.webstylerzone.com/Downloads/exe/CopyKiller-Setup.exe)
* [CopyKiller 3.99a Portable zip. (Archived 2007-07-21)](https://web.archive.org/web/20070721070214/http://www.webstylerzone.com/Downloads/zip/CopyKiller.zip)

#### Misc.: 
* [GBATemp page for A-Ray Scanner. (Archived 2023-05-28)](http://web.archive.org/web/20230528222019/https://gbatemp.net/download/a-ray-scanner.37818/)
* [BinaryObjectScanner source code for CopyKiller detection.](https://github.com/SabreTools/BinaryObjectScanner/blob/master/BinaryObjectScanner/Protection/CopyKiller.cs)
* [BurnOut changelog, which shows detection for CopyKiller being added (and eventually removed). (Archived 2023-10-02)](https://web.archive.org/web/20231002225132/https://www.softpedia.com/progChangelog/BurnOut-Changelog-103960.html)

***

### Authors/Contributors:

* TheRogueArchivist - Entry author.

***

### Footnotes:

