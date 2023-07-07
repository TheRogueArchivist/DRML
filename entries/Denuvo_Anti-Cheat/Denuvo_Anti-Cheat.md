### Names:

Denuvo Anti-Cheat[^1]

### Developers:

Irdeto[^1]

### Years Active: 

2020-05-14[^2] - Current(?)

### Known Versions & Differences: 

2.7.0.40281: Only known version (found as file and product version in multiple files).

### Known Samples: 

#### Confirmed: 

* Doom Eternal Update 1[^3] (Steam Depot 782332 Manifest 7064393210727378308) (Removed in Update 1.1[^4]).

#### Unconfirmed:

* Some Ubisoft games post 2019[^5].

### Categories: 

Anti-Cheat

### Supported Platforms:

* Windows[^1]
* iOS[^1]
* PS4/5[^1]
* Xbox Series X/S[^1]
* Android[^1]

### Protection Features:

Kernel-Mode Driver[^1]; Real-time Monitoring[^12]

### Software Known to Detect:

BurnOutSharp[^6]


### Preservation Instructions:

N/A

### Overall Description:

Denuvo Anti-Cheat is a form of anti-cheat, though information on what games use(d) it is rather sparse. It's known to have been in development since at least 2017[^8]. In 2018, Irdeto mentioned how Denuvo Anti-Cheat would be "soon to be launched as a full end-to-end solution"[^9]. It also appears that Denuvo started providing anti-cheat services for Ubisoft in 2019, and this appears to still be active as of 2023[^5]. Which game or games are protected is unclear, but due to this information seemingly only being available in this document (as far as I'm able to find), which itself is only available in Chinese, it may be that this service is only being used for China-exclusive games. The document also states:

>由于Ubisoft实施了Denuvo的反作弊解决方案，迄今为止共有112个作弊工具开发者被识别和清除。

Translated to English via Google Translate:

>As a result of Ubisoft's implementation of Denuvo's anti-cheat solution, a total of 112 cheat developers have been identified and removed to date.

Assuming this information is correct, this essentially confirms that Denuvo Anti-Cheat has been around since presumably 2019, with some level of success.
This predates the otherwise only documented game to have used Denuvo Anti-Cheat, which is Doom Eternal. It was added in Update 1[^3] on 2020-05-14, before being completely removed in Update 1.1[^4] on 2020-05-27 (less than 2 weeks later!). It's been explicitly stated that the removal was due to the community's negative response, not any issues with Denuvo Anti-Cheat itself[^10]. Although this has seemingly been the only use of Denuvo Anti-Cheat, there have been several documents released by Irdeto about it since then. This includes a Q&A about the Denuvo Anti-Cheat kernel-mode driver[^11], an updated datasheet[^12], and a case study about Denuvo & Ubisoft regarding anti-cheat[^5]. Further confusing my attempt to find examples of games using Denuvo Anti-Cheat is presumably the fact that it considers itself a "white-label solution"[^1], which would allow itself to be rebranded for customer use.

Interestingly, the Q&A about the driver[^11] says that Denuvo Anti-Cheat is only installed and ran when competitive multiplayer is used. This would indicate an updated version or implementation of Denuvo Anti-Cheat, as the version used in Doom Eternal was known to be installed at launch and was required for singleplayer features[^10]. 

Denuvo Anti-Cheat itself works via a kernel-mode driver[^1] that allows the anti-cheat to monitor the game processes and the Windows kernel to send the information along to the server, where all the actual checks take place[^12]. There, the game company can decide if cheating is actually occurring, and what to do about it.

#### Known Associated Executable Sections:

N/A

#### Known Associated Extensions:

N/A

#### Known Associated Files:

* "denuvo-anti-cheat.sys"[^6]
* "denuvo-anti-cheat-update-service.exe"[^6]
* "denuvo-anti-cheat-runtime.dll"[^6]
* "Denuvo Anti-Cheat Installer.exe"[^6]

#### Known Associated Magic Numbers:

N/A

### Media:

N/A

### Additional Resources:

1. [Official Denuvo Anti-Cheat website (Archived 2023-07-05).](https://web.archive.org/web/20230705034105/https://irdeto.com/denuvo/anti-cheat/)
2. ["Denuvo Anti-Cheat goes LIVE!" announcement. (Archived 2023-07-05)](https://web.archive.org/web/20230705040801/https://store.steampowered.com/news/app/782330/view/2187005925152148469)
3. [Denuvo Anti-Cheat Troubleshooting website (Archived 2023-07-05).](https://web.archive.org/web/20230705040353/https://support.codefusion.technology/anti-cheat/)
4. [DOOM Eternal Update 1 Changelog (Archived 2023-07-05).](https://web.archive.org/web/20230705041156/https://slayersclub.bethesda.net/en/article/2zHgbzsIV8gTzFUZ75ADGx/update-1)
5. [DOOM Eternal Update 1.1 Changelog (Archived 2023-07-05).](https://web.archive.org/web/20230705041659/https://slayersclub.bethesda.net/en/article/7puA2mxWqIyP1beRNl23yB/doom-eternal-update-1-1-pc-only-patch-notes)
6. [Denuvo Anti-Cheat Datasheet (Archived 2019-05-12).](https://web.archive.org/web/20190512082146/https://resources.irdeto.com/video-games/datasheet-anti-cheat)
7. [Denuvo Anti-Cheat Newer Datasheet (Archived 2023-07-05).](https://web.archive.org/web/20230705032400/https://resources.irdeto.com/media/datasheet-anti-cheat)
8. [Denuvo Anti-Cheat Newer Datasheet (PDF) (Archived 2023-07-05).](https://web.archive.org/web/20230705044213/https://paperflite-files.s3-accelerate.amazonaws.com/5f8ff4887a4e81372abac654/assets/25904998-9fa4-40b5-bcaf-d9698148587c?response-content-disposition=attachment%3B%20filename%3Ddatasheet_denuvo_anti_cheat.pdf&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20230705T044213Z&X-Amz-SignedHeaders=host&X-Amz-Expires=3600&X-Amz-Credential=AKIAID2JKNATMKKYBBBA%2F20230705%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=8880bb12bf47732dccda85898f3a9f0cfe9fe6a269520bec452bdd8b7bd9bbdb)
9. [Japanese Ubisoft & Denuvo Announcement (Archived 2023-07-05).](https://web.archive.org/web/20230705045142/https://resources.irdeto.com/media/ubisoft-denuvo-irdeto?page=%2Fdenuvo-anti-cheat&widget=619fdf56e86d6a0ef5bccc10)
10. [Chinese Ubisoft & Denuvo Case Study Landing Page (Archived 2023-07-05).](https://web.archive.org/web/20230705033918/https://irdeto.com/denuvo-chinese/case-study-ubisoft-and-denuvo)
11. [Chinese Ubisoft & Denuvo Case Study (Archived 2023-07-05).](https://web.archive.org/web/20230705033408/https://resources.irdeto.com/media/ubisoft-irdeto-case-study_cn)
12. [Chinese Ubisoft & Denuvo Case Study (PDF) (Archived 2023-07-05).](https://web.archive.org/web/20230705045944/https://paperflite-files.s3-accelerate.amazonaws.com/5f8ff4887a4e81372abac654/assets/02421749-56c3-428c-ba24-1f6d8949a741.pdf?response-content-disposition=attachment%3B%20filename%3DUbisoft%20%20Irdeto%20case%20study_CN.pdf&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20230705T045943Z&X-Amz-SignedHeaders=host&X-Amz-Expires=3600&X-Amz-Credential=AKIAID2JKNATMKKYBBBA%2F20230705%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=75b2790266e2ca31f71ae08f732a7ba64ccc3d4daa2e49fbf7c861358f98dfbb)
13. [AWS Marketplace listing for Denuvo Anti-Cheat (Archived 2023-07-05).](https://web.archive.org/web/20230705035916/https://aws.amazon.com/marketplace/pp/prodview-yrdjb756vte3m)
14. [BurnOutSharp's Denuvo page.](https://github.com/mnadareski/BurnOutSharp/blob/master/BinaryObjectScanner.Protection/Denuvo.cs)
15. [Client-Side Security Award for Denuvo Anti-Cheat (Archived 2023-07-5).](https://web.archive.org/web/20230705054156/https://cybersecurity-excellence-awards.com/candidates/denuvo-anti-cheat-5/)
16. ["Leveling the Playing Field with Denuvo Anti-Cheat" (Archived 2019-04-05)](https://web.archive.org/web/20190405085812/https://irdeto.com/news/leveling-the-playing-field-with-denuvo-anti-cheat/)
17. [Announcement that Denuvo Anti-Cheat is available on Steamworks (Archived 2023-07-05).](https://web.archive.org/web/20230705055423/https://irdeto.com/news/denuvo-anti-cheat-now-available-on-steamworks/)
18. [Announcement that Denuvo Anti-Cheat was available to PS5 publishers (Archived 2023-07-05).](https://web.archive.org/web/20230705055627/https://irdeto.com/news/denuvo-joins-exclusive-playstation5-tools-and-middleware-program-to-offer-anti-cheat-technology-to-game-developers/)
19. [Reddit post regarding the removal of Denuvo Anti-Cheat from Doom Eternal (Archived 2020-07-05)](https://web.archive.org/web/20200705043614/https://www.reddit.com/r/Doom/comments/gnjlo7/latest_information_on_update_1_anticheat/)
20. [PC Gaming Wiki article for Denuvo, including Anti-Cheat (Archived 2023-06-27).](https://web.archive.org/web/20230627100253/https://www.pcgamingwiki.com/wiki/Denuvo)
21. [Datasheet for Denuvo Anti-Cheat and Anti-Tamper on mobile. (Archived 2023-07-05).](https://web.archive.org/web/20230705074341/https://resources.irdeto.com/media/datasheet-anti-tamper-and-anti-cheat-technology-for-mobile)
22. [Datasheet for Denuvo Anti-Cheat and Anti-Tamper on mobile. (PDF) (Archived 2023-07-05).](https://web.archive.org/web/20230705074613/https://paperflite-files.s3-accelerate.amazonaws.com/5f8ff4887a4e81372abac654/assets/c1c24ebb-779c-4fc5-bcc5-c387e36ac6bb?response-content-disposition=attachment%3B%20filename%3Ddatasheet-anti-tamper-and-anti-cheat-technology-for-mobile.pdf&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20230705T074613Z&X-Amz-SignedHeaders=host&X-Amz-Expires=3600&X-Amz-Credential=AKIAID2JKNATMKKYBBBA%2F20230705%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=8a0e160d299e722174c16e4cc8b6f99ea7144e831fc9eee3d26aed36ddb1a422)
23. [Irdeto Global Gaming Survey Report (Archived 2023-07-05).](https://web.archive.org/web/20230705074835/https://resources.irdeto.com/media/irdeto-global-gaming-survey-report)
24. [Irdeto Global Gaming Survey Report (PDF) (Archived 2023-07-05).](https://web.archive.org/web/20230705074919/https://paperflite-files.s3-accelerate.amazonaws.com/5f8ff4887a4e81372abac654/assets/54529c74-2476-49b9-9bdb-2b7887c9d117?response-content-disposition=attachment%3B%20filename%3Dirdeto-global-gaming-survey-report.pdf&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20230705T074918Z&X-Amz-SignedHeaders=host&X-Amz-Expires=3600&X-Amz-Credential=AKIAID2JKNATMKKYBBBA%2F20230705%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=47c1e541ad6a8f1dd05f0eca4f448dde5623dfc16d31cb128942e77fe7ee907b)
25. [Denuvo Anti-Cheat brochure for PC games (Archived 2023-07-05).](https://web.archive.org/web/20230705075230/https://resources.irdeto.com/media/brochure-anti-cheat)
26. [Denuvo Anti-Cheat brochure for PC games (PDF) (Archived 2023-07-05).](https://web.archive.org/web/20230705075419/https://paperflite-files.s3-accelerate.amazonaws.com/5f8ff4887a4e81372abac654/assets/fc381848-80e2-4fd6-bea9-d5c101d452e8?response-content-disposition=attachment%3B%20filename%3Danticheatbrochure_forPCgames_final.pdf&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20230705T075418Z&X-Amz-SignedHeaders=host&X-Amz-Expires=3600&X-Amz-Credential=AKIAID2JKNATMKKYBBBA%2F20230705%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=0e3553514de76d7d6f255395348873eff300d0e45c1e469d4d7ee7858c2577c5)
27. [Denuvo Anti-Cheat brochure for console games (Archived 2023-07-05).](https://web.archive.org/web/20230705075635/https://resources.irdeto.com/media/brochure-anti-cheat-for-console-games)
28. [Denuvo Anti-Cheat brochure for console games (PDF) (Archived 2023-07-05).](https://web.archive.org/web/20230705075857/https://paperflite-files.s3-accelerate.amazonaws.com/5f8ff4887a4e81372abac654/assets/6b3fdb88-ce96-4181-a3e9-37aeb42c2033?response-content-disposition=attachment%3B%20filename%3Danti_cheat_brochure_console_Irdeto.pdf&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20230705T075857Z&X-Amz-SignedHeaders=host&X-Amz-Expires=3600&X-Amz-Credential=AKIAID2JKNATMKKYBBBA%2F20230705%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=4521514596ff848ad56125516bafdfc90f066246f3f759e210bb8594e9c5a761)
29. [Denuvo Anti-Cheat Kernel-Mode Driver FAQ (Archived 2023-07-05).](https://web.archive.org/web/20230705080029/https://resources.irdeto.com/media/q-a-about-denuvo-anti-cheat-and-windows-kernel-mode-drivers)
30. [Denuvo Anti-Cheat Kernel-Mode Driver FAQ (PDF) (Archived 2023-07-05).](https://web.archive.org/web/20230705151811/https://paperflite-files.s3-accelerate.amazonaws.com/5f8ff4887a4e81372abac654/assets/daf83521-666d-40eb-9ef2-ef0da7f9c2a7?response-content-disposition=attachment%3B%20filename%3Ddenuvo_qa_anti_cheat_kernel_mode_drivers.pdf&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20230705T151811Z&X-Amz-SignedHeaders=host&X-Amz-Expires=3600&X-Amz-Credential=AKIAID2JKNATMKKYBBBA%2F20230705%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=d98f2131eea7a38cc74c6a0fce56bb159277c69f1a9859f600619088950e0bc6)
31. [Denuvo Anti-Cheat Free Datasheet website (Archived 2023-07-07).](https://web.archive.org/web/20230705080631/https://irdeto.com/datasheet-denuvo-anti-cheat-the-only-transparent-solution-that-catches-all-cheaters/)
32. ["Denuvo Anti-Cheat: The only transparent premium cheat detection" (Archived 2023-07-05).](https://web.archive.org/web/20230705081130/https://resources.irdeto.com/media/datasheet-denuvo-anti-cheat-the-only-transparent-solution-that-catches-all-cheaters-landing-page)
33. ["Denuvo Anti-Cheat: The only transparent premium cheat detection" (PDF) (Archived 2023-07-05).](https://web.archive.org/web/20230705081326/https://paperflite-files.s3-accelerate.amazonaws.com/5f8ff4887a4e81372abac654/assets/aa2560a7-12ca-4e9d-bc70-57c0e016a2c7?response-content-disposition=attachment%3B%20filename%3Ddatasheet_denuvo_anti_cheat.pdf&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20230705T081326Z&X-Amz-SignedHeaders=host&X-Amz-Expires=3600&X-Amz-Credential=AKIAID2JKNATMKKYBBBA%2F20230705%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=c4fa26160a4be3f2bcdbcbb81ce6eb831538a049b39d2f3136927e17061d15a5)
34. [Main Denuvo website, which mentions Denuvo Anti-Cheat (Archived 2017-01-31).](https://web.archive.org/web/20170131030651/http://denuvo.com/)
35. ["Denuvo Joins Esports Integrity Coalition to Combat Cheating" (Archived 2019-04-05).](https://web.archive.org/web/20190405043008/https://irdeto.com/news/denuvo-joins-esports-integrity-coalition-to-combat-cheating/)
36. [Official Denuvo Anti-Cheat website (Archived 2021-06-11).](https://web.archive.org/web/20210611213309/https://irdeto.com/denuvo/anti-cheat/)
37. [Official Denuvo Anti-Cheat Resources (Page seemingly broken in Wayback) (Archived 2023-07-06).](https://web.archive.org/web/20230706052839/https://resources.irdeto.com/denuvo-anti-cheat)

### Footnotes:

[^1]: [Official Denuvo Anti-Cheat website (Archived 2023-07-05) (Additional Resource #1).](https://web.archive.org/web/20230705034105/https://irdeto.com/denuvo/anti-cheat/)
[^2]: ["Denuvo Anti-Cheat goes LIVE!" announcement. (Archived 2023-07-05) (Additional Resource #2)](https://web.archive.org/web/20230705040801/https://store.steampowered.com/news/app/782330/view/2187005925152148469)
[^3]: [DOOM Eternal Update 1 Changelog (Archived 2023-07-05) (Additional Resource #4).](https://web.archive.org/web/20230705041156/https://slayersclub.bethesda.net/en/article/2zHgbzsIV8gTzFUZ75ADGx/update-1)
[^4]: [DOOM Eternal Update 1.1 Changelog (Archived 2023-07-05) (Additional Resource #5).](https://web.archive.org/web/20230705041659/https://slayersclub.bethesda.net/en/article/7puA2mxWqIyP1beRNl23yB/doom-eternal-update-1-1-pc-only-patch-notes)
[^5]: [Chinese Ubisoft & Denuvo Case Study (PDF) (Archived 2023-07-05).](https://web.archive.org/web/20230705045944/https://paperflite-files.s3-accelerate.amazonaws.com/5f8ff4887a4e81372abac654/assets/02421749-56c3-428c-ba24-1f6d8949a741.pdf?response-content-disposition=attachment%3B%20filename%3DUbisoft%20%20Irdeto%20case%20study_CN.pdf&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20230705T045943Z&X-Amz-SignedHeaders=host&X-Amz-Expires=3600&X-Amz-Credential=AKIAID2JKNATMKKYBBBA%2F20230705%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=75b2790266e2ca31f71ae08f732a7ba64ccc3d4daa2e49fbf7c861358f98dfbb)
[^6]: [BurnOutSharp's Denuvo page (Additional Resource #14).](https://github.com/mnadareski/BurnOutSharp/blob/master/BinaryObjectScanner.Protection/Denuvo.cs)
[^7]: [Denuvo Anti-Cheat Troubleshooting website (Archived 2023-07-05) (Additional Resource #3).](https://web.archive.org/web/20230705040353/https://support.codefusion.technology/anti-cheat/)
[^8]: [Main Denuvo website, which mentions Denuvo Anti-Cheat (Archived 2017-01-31) (Additional Resource #34).](https://web.archive.org/web/20170131030651/http://denuvo.com/)
[^9]: ["Denuvo Joins Esports Integrity Coalition to Combat Cheating" (Archived 2019-04-05) (Additional Resource #35).](https://web.archive.org/web/20190405043008/https://irdeto.com/news/denuvo-joins-esports-integrity-coalition-to-combat-cheating/)
[^10]: [Reddit post regarding the removal of Denuvo Anti-Cheat from Doom Eternal (Archived 2020-07-05) (Additional Resource #19).](https://web.archive.org/web/20200705043614/https://www.reddit.com/r/Doom/comments/gnjlo7/latest_information_on_update_1_anticheat/)
[^11]: [Denuvo Anti-Cheat Kernel-Mode Driver FAQ (PDF) (2023-07-05) (Additional Resource #30).](https://web.archive.org/web/20230705151811/https://paperflite-files.s3-accelerate.amazonaws.com/5f8ff4887a4e81372abac654/assets/daf83521-666d-40eb-9ef2-ef0da7f9c2a7?response-content-disposition=attachment%3B%20filename%3Ddenuvo_qa_anti_cheat_kernel_mode_drivers.pdf&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20230705T151811Z&X-Amz-SignedHeaders=host&X-Amz-Expires=3600&X-Amz-Credential=AKIAID2JKNATMKKYBBBA%2F20230705%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=d98f2131eea7a38cc74c6a0fce56bb159277c69f1a9859f600619088950e0bc6)
[^12]: [Denuvo Anti-Cheat Newer Datasheet (PDF) (Archived 2023-07-05) (Additional Resource #8).](https://web.archive.org/web/20230705044213/https://paperflite-files.s3-accelerate.amazonaws.com/5f8ff4887a4e81372abac654/assets/25904998-9fa4-40b5-bcaf-d9698148587c?response-content-disposition=attachment%3B%20filename%3Ddatasheet_denuvo_anti_cheat.pdf&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20230705T044213Z&X-Amz-SignedHeaders=host&X-Amz-Expires=3600&X-Amz-Credential=AKIAID2JKNATMKKYBBBA%2F20230705%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=8880bb12bf47732dccda85898f3a9f0cfe9fe6a269520bec452bdd8b7bd9bbdb)
