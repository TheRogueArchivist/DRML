### Names:

engine32[^engine32_product_name], engine32.dll[^engine32_file_name]

[^engine32_product_name]: Product name of most copies of "engine32.dll".

[^engine32_file_name]: File name for the only known file specific to this DRM.

***

### Developers:

Nival/Atomy/"Buka Entertainment"[^Nival_Atomy_Buka_Connection]

[^Nival_Atomy_Buka_Connection]: It seems that Nival may have developed this DRM internally, and that Atomy may have picked up on it later. It also appears that Buka also used the DRM, presumably due to ties to Atomy. This is speculation, and is elaborated on further in the "Overall Description" section.

***

### Years Active: 

~2003[^Lionheart_Rutracker] - ~2008[^Da_Vinci_Code_Rutracker]

[^Da_Vinci_Code_Rutracker]: [Forum post and torrent for "The Da Vinci Code". (Archived 2024-03-02)](https://web.archive.org/web/20240302021638/https://rutracker.org/forum/viewtopic.php?t=5198858)

[^Lionheart_Rutracker]: [Forum post and torrent for "Lionheart: Legacy of The Crusader". (Archived 2024-03-02)](https://web.archive.org/web/20240302023029/https://rutracker.org/forum/viewtopic.php?t=5188207)

***

### Known Versions & Differences: 

2.0.0.0: Only known version based on file version of multiple copies of the file "engine32.dll". "One Must Fall: Battlegrounds"[^One_Must_Fall_Redump] and "Lionheart: Legacy of The Crusader[^Lionheart_Rutracker]" both have "engine32.dll" without file properties, so the version field is blank.

[^One_Must_Fall_Redump]: [Forum post and torrent for "One Must Fall: Battlegrounds". (Archived 2024-03-02)](https://web.archive.org/web/20240302023831/https://rutracker.org/forum/viewtopic.php?t=5495752)

***

### Known Samples: 

#### Confirmed: 

The RU localized versions of the following games:

* Rayman Raving Rabbids 2[^Rayman_Raving_Rabbids_Redump].
* Colin McRae Rally 2005[^Colin_McRae_Rally_Redump].
* TOCA Race Driver 2[^TOCA_Redump].
* One Must Fall: Battlegrounds[^One_Must_Fall_Redump].
* The Da Vinci Code[^Da_Vinci_Code_Rutracker].
* Lionheart: Legacy of The Crusader[^Lionheart_Rutracker].
* CivCity Rome[^CivCity_Rome_Rutracker].

[^Colin_McRae_Rally_Redump]: Redump entry 103413.
[^TOCA_Redump]: Redump entries 104593-104596.
[^CivCity_Rome_Rutracker]: [Forum post and torrent for "CivCity Rome". (Archived 2024-03-02)](https://web.archive.org/web/20240302034812/https://rutracker.org/forum/viewtopic.php?t=5319308)

#### Unconfirmed:

Possibly other games localized/developed by Nival, Atomy and/or Buka Entertainment.

***

### Categories: 

Optical Copy Protection

***

### Protection Features:

Disc Check

***

### Minimum Required Image Format to Run:

ISO

***

### Software Known to Detect:

BinaryObjectScanner[^engine32_BOS]

[^engine32_BOS]: [BinaryObjectScanner's engine32 detection code.](https://github.com/SabreTools/BinaryObjectScanner/blob/master/BinaryObjectScanner/Protection/Engine32.cs)

***

### Preservation Instructions:

Only a basic disc image is needed.

***

### Overall Description:

Engine32 is the tentative name given to a generic disc check DRM used across several games localized/developed by Nival and Atomy. Starting in 2003, Nival released a few games with engine32 present, including "Lionheart: Legacy of The Crusader"[^Lionheart_Rutracker] and "One Must Fall: Battlegrounds"[^One_Must_Fall_Redump]. Some later games from around 2006 that include engine32 include "CivCity: Rome"[^CivCity_Rome_Rutracker] and "The Da Vinci Code"[^Da_Vinci_Code_Rutracker], both of which were localized by Atomy[^Atomy_Localization_MobyGames]. Funnily enough, the file description for "engine32.dll" present within "CivCity: Rome" is "The Da Vinci Code DLL-helper", despite having different hashes and being last modified on different days. Finally, one of (if not the) latest examples of engine32 being used is "Rayman Raving Rabbids 2"[^Rayman_Raving_Rabbids_Redump], by Buka Entertainment.

It appears that engine32 originated in Nival, most likely as an exceedingly simple, easy to add DRM to add to their projects. It then appears to stopped being used by Nival, and instead began being used by Atomy. Atomy had also apparently hired several people who were originally from Nival around this time ("In 2006, he founded and headed the Atomy company, which included former employees of the Nival localization department.")[^Ilya_Mamontoc_Kanobu]. Curiously, the final currently known game to use "engine32.dll" was "Rayman Raving Rabbids 2", in which the protection still has a copyright of "Atomy games" despite the game being officially published in Russia by Buka Entertainment, suggesting a connection between the two. It's also important to note that the founder of Atomy also got an executive localization-related role at Buka Entertainment not long after (the same year as) founding Atomy[^Ilya_Mamontoc_Kanobu]. This leads me to believe that engine32 was originally developed by or for Nival initially, and was brought along to Atomy later by the ex-Nival team. Finally, it seems that it was brought to Buka Entertainment, either by the founder of Atomy when he took on an executive role there, or possibly by the same ex-Nival team, as some may have once again followed along to the new company.

Due to the unfortunately generic file name, there are a few cases of what are assumed to be unrelated files that also happen to be named "engine32.dll". This includes a file associated with "Ultima Online Sphere Server"[^Ultima_Online_Sphere_Server_uokit][^Ultima_Online_Sphere_Server_uokit_Download], FritzChess 17[^FritzChess_17_SteamDB], Houdini 5 Pro[^Houdini_5_Pro_Should_I_Remove_It], and ChessBase 14[^ChessBase_14_HerdProtect].

The DRM itself is a simple disc check that appears to simply check for a generic file name on the disc. This means that it's completely bypassed by having a disc image mounted. It's also possible to easily modify a copy of "engine32.dll" to always pass the disc check, and this modified copy can be used on most, if not all, other games with engine32. The "engine32.dll" file that was modified to crack "One Must Fall: Battlegrounds"[^One_Must_Fall_Redump] has been confirmed to work for every known sample so far.


[^Atomy_Localization_MobyGames]: [MobyGames list of games localized by Atomy. (Archived 2024-03-02)](https://web.archive.org/web/20240302035550/https://www.mobygames.com/company/10503/atomy/games/title:11/)

[^Ilya_Mamontoc_Kanobu]: [A news article about Ilya Mamontov, founder of Atomy. (Archived 2024-03-02)](https://web.archive.org/web/20240302040129/https://kanobu.ru/news/glava-evropejskogo-ofisa-mailru-games-pereshel-v-crytek-371932/)

[^Ultima_Online_Sphere_Server_uokit]: [Ultima Online Sphere Server forum post that mentions an "engine32.dll". (Archived 2024-03-02)](https://web.archive.org/web/20240302041228/https://forum.uokit.com/index.php?showtopic=27645)

[^Ultima_Online_Sphere_Server_uokit_Download]: [Utlima Online Sphere Server forum post that includes a (now defunct) link to download an "engine32.dll". (Archived 2024-03-02)](https://web.archive.org/web/20240302041622/https://forum.uokit.com/smart/index.php?t23568-20.html)

[^FritzChess_17_SteamDB]: [SteamDB page for a FritzChess 17 depot.](https://steamdb.info/depot/1279592/)

[^Houdini_5_Pro_Should_I_Remove_It]: ["Should I Remove It?" page for Houdini 5 Pro. (Archived 2024-03-02)](https://web.archive.org/web/20240302042445/https://www.shouldiremoveit.com/Houdini-5-Pro-64-bit-201918-program.aspx)

[^ChessBase_14_HerdProtect]: [HerdProtect page for "engine32.dll" from ChessBase 14. (Archived 2024-03-02)](https://web.archive.org/web/20240302042953/https://www.herdprotect.com/engine32.dll-48f4ed3ffa234e454164e4f87803f1fe6924d345.aspx)

***

#### Known Associated Files:

##### "engine32.dll":

Found in every known sample of this DRM, as it's the defining file that indicates the DRM's presence.

#### Game Specific Files:

N/A.

***

#### Known Associated Executable Sections:

N/A.

***

### Media:

1. Error message when disc check fails for "Rayman Raving Rabbids 2"[^Rayman_Raving_Rabbids_Redump]:

![Windows warning window with the title"Rayman Бешеные кролики 2: диск не найден!"; the main window text "Пожалуйста, поместите диск с игрой Rayman Бешеные кролики 2 в CD/DVD-привод."; and the option buttons "Retry" and "Cancel"](./engine32-rayman-error.png "Engine32 Error Message")

[^Rayman_Raving_Rabbids_Redump]: Redump entry 106031.

***

### Additional Resources:

#### Rutracker posts:
 
* [Forum post and torrent for "One Must Fall: Battlegrounds". (Archived 2024-03-02)](https://web.archive.org/web/20240302023831/https://rutracker.org/forum/viewtopic.php?t=5495752)
* [Forum post and torrent for "The Da Vinci Code". (Archived 2024-03-02)](https://web.archive.org/web/20240302021638/https://rutracker.org/forum/viewtopic.php?t=5198858)
* [Forum post and torrent for "Lionheart: Legacy of The Crusader". (Archived 2024-03-02)](https://web.archive.org/web/20240302023029/https://rutracker.org/forum/viewtopic.php?t=5188207)
* [Forum post and torrent for "CivCity Rome". (Archived 2024-03-02)](https://web.archive.org/web/20240302034812/https://rutracker.org/forum/viewtopic.php?t=5319308)
* [Forum post and torrent for "Rayman Raving Rabbids 2". (Archived 2024-03-02)](https://web.archive.org/web/20240302044211/https://rutracker.org/forum/viewtopic.php?t=6362358)

#### Internet Archive backups:

* [Internet Archive backup of the torrent for "One Must Fall: Battlegrounds".](https://archive.org/details/one-must-fall-battlegrounds-l-rus-eng-rus-eng-2003-1-rutracker)
* [Internet Archive backup of the torrent for "The Da Vinci Code".](https://archive.org/details/the-da-vinci-code-l-rus-rus-2006-1-rutracker)
* [Internet Archive backup of the torrent for "Lionheart: Legacy of The Crusader".](https://archive.org/details/lionheart-legacy-of-the-crusader-l-rus-rus-2003-1-rutracker)
* [Internet Archive backup of the torrent for "CivCity Rome".](https://archive.org/details/civcity-rome-l-rus-rus-2006-1-rutracker)
* [Internet Archive backup of the torrent for "Rayman Raving Rabbids 2".](https://archive.org/details/rayman-raving-rabbids-2-2-l-rus-2007-rutracker)

#### MobyGames: 

* [MobyGames page for Atomy. (Archived 2024-03-02)](https://web.archive.org/web/20240302035628/https://www.mobygames.com/company/10503/atomy/)
* [MobyGames page for Nival. (Archived 2024-03-02)](https://web.archive.org/web/20240302045321/https://www.mobygames.com/company/925/nival-inc/)
* [MobyGames page for ESDigital Games, formerly Buka Entertainment. (Archived 2024-03-02)](https://web.archive.org/web/20240302045726/https://www.mobygames.com/company/1392/esdigital-games/)
* [MobyGames list of games localized by Atomy. (Archived 2024-03-02)](https://web.archive.org/web/20240302035550/https://www.mobygames.com/company/10503/atomy/games/title:11/)

#### Misc.:

[TODO: Make sure files from GameCopyWorld are properly archived.]

* [Crack for "Lionheart: Legacy of The Crusader" from GameCopyWorld. (Archived 2024-03-02)](https://web.archive.org/web/20240302050136/https://gamecopyworld.com/games/pc_lionheart.shtml)
* [Torrent for "Colin McRae Rally 2005", including a crack (Untested. (Archived 2023-08-29)](https://web.archive.org/web/20230829003900/https://top.lafa.site/igry/Gonki/colin-mcrae-rally-2005.htm)
* [Ultima Online Sphere Server forum post that mentions an "engine32.dll". (Archived 2024-03-02)](https://web.archive.org/web/20240302041228/https://forum.uokit.com/index.php?showtopic=27645)
* [Utlima Online Sphere Server forum post that includes a (now defunct) link to download an "engine32.dll". (Archived 2024-03-02)](https://web.archive.org/web/20240302041622/https://forum.uokit.com/smart/index.php?t23568-20.html)
* [SteamDB page for a FritzChess 17 depot.](https://steamdb.info/depot/1279592/)
* ["Should I Remove It?" page for Houdini 5 Pro. (Archived 2024-03-02)](https://web.archive.org/web/20240302042445/https://www.shouldiremoveit.com/Houdini-5-Pro-64-bit-201918-program.aspx)
* [HerdProtect page for "engine32.dll" from ChessBase 14. (Archived 2024-03-02)](https://web.archive.org/web/20240302042953/https://www.herdprotect.com/engine32.dll-48f4ed3ffa234e454164e4f87803f1fe6924d345.aspx)
* [A news article about Ilya Mamontov, founder of Atomy. (Archived 2024-03-02)](https://web.archive.org/web/20240302040129/https://kanobu.ru/news/glava-evropejskogo-ofisa-mailru-games-pereshel-v-crytek-371932/)
* [A news article that briefly lists the career history of Ilya Mamontov. (Archived 2024-03-02)](https://web.archive.org/web/20240302043630/https://www.gamesindustry.biz/crytek-hires-mail-ru-exec)

***

### Authors/Contributors:

* TheRogueArchivist - Entry author.

***

### Footnotes:









