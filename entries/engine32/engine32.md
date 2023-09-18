### Names:

engine32[^1], engine32.dll[^2]

### Developers:

Nival/Atomy/"Buka Entertainment"[^10]

### Years Active: 

~2003[^8] - ~2008[^7]

### Known Versions & Differences: 

2.0.0.0: Only known version based on file version of multiple copies of the file "engine32.dll". "One Must Fall: Battlegrounds"[^6] and "Lionheart: Legacy of The Crusader[^8]" both have "engine32.dll" without file properties, so the version field is blank.

### Known Samples: 

#### Confirmed: 

The RU localized versions of the following games:

* Rayman Raving Rabbids 2[^3].
* Colin McRae Rally 2005[^4].
* TOCA Race Driver 2[^5].
* One Must Fall: Battlegrounds[^6].
* The Da Vinci Code[^7].
* Lionheart: Legacy of The Crusader[^8].
* CivCity Rome[^9].

#### Unconfirmed:

Possibly other games localized/developed by Nival, Atomy and/or Buka Entertainment.

### Categories: 

Optical Copy Protection

### Protection Features:

Disc Check

### Minimum Required Image Format to Run:

ISO

### Software Known to Detect:

BurnOutSharp[^10]

### Detection Related Information:

https://github.com/mnadareski/BurnOutSharp/blob/master/BinaryObjectScanner.Protection/Engine32.cs

### Preservation Instructions:

Only a basic disc image is needed.

### Overall Description:

Engine32 is the tentative name given to a generic disc check DRM used across several games localized/developed by Nival and Atomy. Starting in 2003, Nival released a few games with engine32 present, including "Lionheart: Legacy of The Crusader"[^8] and "One Must Fall: Battlegrounds"[^6]. Some later games from around 2006 that include engine32 include "CivCity: Rome"[^9] and "The Da Vinci Code"[^7], both of which were localized by Atomy[^18]. Funnily enough, the file description for "engine32.dll" present within "CivCity: Rome" is "The Da Vinci Code DLL-helper", despite having different hashes and being last modified on different days. Finally, one of (if not the) latest examples of engine32 being used is "Rayman Raving Rabbids 2"[^3], by Buka Entertainment.

It appears that engine32 originated in Nival, most likely as an exceedingly simple, easy to add DRM to add to their projects. It then appears to stopped being used by Nival, and instead began being used by Atomy. Atomy had also apparently hired several people who were originally from Nival around this time ("In 2006, he founded and headed the Atomy company, which included former employees of the Nival localization department.")[^16]. Curiously, the final currently known game to use "engine32.dll" was "Rayman Raving Rabbids 2", in which the protection still has a copyright of "Atomy games" despite the game being officially published in Russia by Buka Entertainment, suggesting a connection between the two. It's also important to note that the founder of Atomy also got an executive localization-related role at Buka Entertainment not long after (the same year as) founding Atomy[^16]. This leads me to believe that engine32 was originally developed by or for Nival initially, and was brought along to Atomy later by the ex-Nival team. Finally, it seems that it was brought to Buka Entertainment, either by the founder of Atomy when he took on an executive role there, or possibly by the same ex-Nival team, as some may have once again followed along to the new company.

Due to the unfortunately generic file name, there are a few cases of what are assumed to be unrelated files that also happen to be named "engine32.dll". This includes a file associated with "Ultima Online Sphere Server"[^11][^12], FritzChess 17[^13], Houdini 5 Pro[^14], and ChessBase 14[^15].

The DRM itself is a simple disc check that appears to simply check for a generic file name on the disc. This means that it's completely bypassed by having a disc image mounted. It's also possible to easily modify a copy of "engine32.dll" to always pass the disc check, and this modified copy can be used on most, if not all, other games with engine32. The "engine32.dll" file that was modified to crack "One Must Fall: Battlegrounds"[^6] has been confirmed to work for every known sample so far.

#### Known Associated Files:

##### "engine32.dll":

Found in every known sample of this DRM, as it's the defining file that indicates the DRM's presence.

#### Game Specific Files:

N/A.

#### Known Associated Executable Sections:

N/A.

### Media:

1. Error message when disc check fails for "Rayman Raving Rabbids 2"[^3]:

!["Rayman Бешеные кролики 2: диск не найден!" - "Пожалуйста, поместите диск с игрой Rayman Бешеные кролики 2 в CD/DVD-привод." - "Retry" - "Cancel"](./engine32-rayman-error.png "Engine32 Error Message")

### Additional Resources:
 
1. [Forum post and torrent for "One Must Fall: Battlegrounds".](https://rutracker.org/forum/viewtopic.php?t=5495752)
2. [Internet Archive backup of the torrent for "One Must Fall: Battlegrounds".](https://archive.org/details/one-must-fall-battlegrounds-l-rus-eng-rus-eng-2003-1-rutracker)
3. [Forum post and torrent for "The Da Vinci Code".](https://rutracker.org/forum/viewtopic.php?t=5198858)
4. [Internet Archive backup of the torrent for "The Da Vinci Code".](https://archive.org/details/the-da-vinci-code-l-rus-rus-2006-1-rutracker)
5. [Forum post and torrent for "Lionheart: Legacy of The Crusader".](https://rutracker.org/forum/viewtopic.php?t=5188207)
6. [Internet Archive backup of the torrent for "Lionheart: Legacy of The Crusader".](https://archive.org/details/lionheart-legacy-of-the-crusader-l-rus-rus-2003-1-rutracker)
7. [Crack for "Lionheart: Legacy of The Crusader" from GameCopyWorld.](https://gamecopyworld.com/games/pc_lionheart.shtml)
8. [Torrent for "Colin McRae Rally 2005", including a crack (Untested)](https://top.lafa.site/igry/Gonki/colin-mcrae-rally-2005.htm)
9. [Forum post and torrent for "CivCity Rome".](https://rutracker.org/forum/viewtopic.php?t=5319308)
10. [Internet Archive backup of the torrent for "CivCity Rome".](https://archive.org/details/civcity-rome-l-rus-rus-2006-1-rutracker)
11. [MobyGames page for Atomy.](https://www.mobygames.com/company/10503/atomy/)
12. [MobyGames page for Nival.](https://www.mobygames.com/company/925/nival-inc/)
13. [Ultima Online Sphere Server forum post that mentions an "engine32.dll".](https://forum.uokit.com/index.php?showtopic=27645)
14. [Utlima Online Sphere Server forum post that includes a (now defunct) link to download an "engine32.dll".](https://forum.uokit.com/smart/index.php?t23568-20.html)
15. [SteamDB page for a FritzChess 17 depot.](https://steamdb.info/depot/1279592/)
16. ["Should I Remove It?" page for Houdini 5 Pro.](https://www.shouldiremoveit.com/Houdini-5-Pro-64-bit-201918-program.aspx)
17. [HerdProtect page for "engine32.dll" from ChessBase 14.](https://www.herdprotect.com/engine32.dll-48f4ed3ffa234e454164e4f87803f1fe6924d345.aspx)
18. [A news article about Ilya Mamontov, founder of Atomy.](https://kanobu.ru/news/glava-evropejskogo-ofisa-mailru-games-pereshel-v-crytek-371932/)
19. [A news article that briefly lists the career history of Ilya Mamontov.](https://www.gamesindustry.biz/crytek-hires-mail-ru-exec)
20. [MobyGames page for ESDigital Games, formerly Buka Entertainment.](https://www.mobygames.com/company/1392/esdigital-games/)
21. [Forum post and torrent for "Rayman Raving Rabbids 2".](https://rutracker.org/forum/viewtopic.php?t=6362358)
22. [Internet Archive backup of the torrent for "Rayman Raving Rabbids 2".](https://archive.org/details/rayman-raving-rabbids-2-2-l-rus-2007-rutracker)
23. [MobyGames list of games localized by Atomy.](https://www.mobygames.com/company/10503/atomy/games/title:11/)


### Footnotes:

[^1]: Product name of most copies of "engine32.dll".
[^2]: File name for the only known file specific to this DRM.
[^3]: Redump entry 106031.
[^4]: Redump entry 103413.
[^5]: Redump entries 104593-104596.
[^6]: [Forum post and torrent for "One Must Fall: Battlegrounds". (Additional Resource #1)](https://rutracker.org/forum/viewtopic.php?t=5495752)
[^7]: [Forum post and torrent for "The Da Vinci Code". (Additional Resource #3)](https://rutracker.org/forum/viewtopic.php?t=5198858)
[^8]: [Forum post and torrent for "Lionheart: Legacy of The Crusader". (Additional Resource #5)](https://rutracker.org/forum/viewtopic.php?t=5188207)
[^9]: [Forum post and torrent for "CivCity Rome". (Additional Resource #9)](https://rutracker.org/forum/viewtopic.php?t=5319308)
[^10]: It seems that Nival may have developed this DRM internally, and that Atomy may have picked up on it later. It also appears that Buka also used the DRM, presumably due to ties to Atomy. This is speculation, and is elaborated on further in the "Overall Description" section.
[^11]: [Ultima Online Sphere Server forum post that mentions an "engine32.dll". (Additional Resource #13)](https://forum.uokit.com/index.php?showtopic=27645)
[^12]: [Utlima Online Sphere Server forum post that includes a (now defunct) link to download an "engine32.dll". (Additional Resource #14)](https://forum.uokit.com/smart/index.php?t23568-20.html)
[^13]: [SteamDB page for a FritzChess 17 depot. (Additional Resource #15)](https://steamdb.info/depot/1279592/)
[^14]: ["Should I Remove It?" page for Houdini 5 Pro. (Additional Resource #16)](https://www.shouldiremoveit.com/Houdini-5-Pro-64-bit-201918-program.aspx)
[^15]: [HerdProtect page for "engine32.dll" from ChessBase 14. (Additional Resource #17)](https://www.herdprotect.com/engine32.dll-48f4ed3ffa234e454164e4f87803f1fe6924d345.aspx)
[^16]: [A news article about Ilya Mamontov, founder of Atomy. (Additional Resource #18)](https://kanobu.ru/news/glava-evropejskogo-ofisa-mailru-games-pereshel-v-crytek-371932/)
[^17]: [A news article that briefly lists the career history of Ilya Mamontov. (Additional Resource #19)](https://www.gamesindustry.biz/crytek-hires-mail-ru-exec)
[^18]: [MobyGames list of games localized by Atomy. (Additional Resource #22)](https://www.mobygames.com/company/10503/atomy/games/title:11/)