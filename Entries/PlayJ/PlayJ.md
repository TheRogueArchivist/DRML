### Names:

PlayJ[^1]

### Developers:

EverAd[^1]

### Years Active: 

~2000-02[^2] - ~2001-07[^3]

### Known Versions & Differences: 

[TODO: Document CDS version of format.]

Version 1: The initial release of the format, and seemingly by far the most commonly used version, based on how many samples have been found compared to version 2. This version did not contain any advertisements within the file itself, as they were downloaded exclusively by the music player. Information about the structure of the format can be found in BOS[^11].

Version 2: The updated version of the format, which changed some of the basic structure of the format, as well as adding some advertisements directly into the file. These were presumably intended to supplement the advertisements being downloaded by the player. Information about the structure of the format can be found in BOS[^11]. Interestingly, this version is seemingly much rarer than version 1. An example of it can be found in the file "lady.plj" from the PlayJ CDN[^6].

### Known Samples: 

#### Confirmed: 

* PLJ files hosted on the PlayJ CDN[^6].
* PLJ files hosted on TUCOWS Music[^7].

#### Unconfirmed:

* Possibly songs from Listen.com[^8].
* Possibly songs from Launch.com[^9].

### Categories: 

Multimedia DRM

### Protection Features:

Encryption/Obfuscation of data[^13]; Internet connectivity

### Software Known to Detect:

BinaryObjectScanner[^10]


### Preservation Instructions:

N/A

### Overall Description:

PlayJ by EverAd was a form of DRM protected audio that was intended to be distributed freely, but that showed advertisements to the listener. This format didn't live for very long, having started in the February of 2000 and ending with the parent company shutting down in 2001. The file format itself appears to be an encrypted MP3[^13]. The music itself can still be listened to by use of the official player[^14], as it allows for a limited number of songs to be played before needing to connect to its server (which is obviously now offline).

It was also used briefly for some early versions of CDS-200, as can be seen in the BOS detections for PlayJ[^10]. The "YUCCA.CDS" file appears to be a collection of PlayJ format audio files concatenated together, with an additional header and possibly other changes. [TODO: Add actual source]

#### Known Associated Executable Sections:

N/A

#### Known Associated Extensions:

".plj"[^4] + ".CDS"[^5]

#### Known Associated Files:

"YUCCA.CDS"[^5]

#### Known Associated Magic Numbers:

"FF 9D 53 4B"[^4]

### Media:

[TODO: Include photo of the PlayJ "Connect to Internet" error]

### Additional Resources:

1. [Official website for PlayJ.](https://web.archive.org/web/20000815053956/http://www.playj.com/)
2. [PlayJ official FAQ.](https://web.archive.org/web/20000815065805/http://www.playj.com/static/faq_page.html)
3. [PlayJ IANA assignment.](https://www.iana.org/assignments/media-types/audio/vnd.everad.plj)
4. [News article about the launch of PlayJ.](https://en.globes.co.il/en/article-383855)
5. [News article about the closure of PlayJ.](https://www.themarker.com/misc/2001-07-26/ty-article/0000017f-e690-df2c-a1ff-fed177870000)
6. [PlayJ Studio Installer.](https://web.archive.org/web/20010417025347/http://dlp.playj.com:80/playj/PlayJIns266.exe)
7. [PlayJ CDN contents.](https://web.archive.org/web/*/dlp.playj.com/*/)
8. [TUCOWS Music main site contents.](https://web.archive.org/web/*/http://music.tucows.com/*)
9. [TUCOWS Music "dia" mirror contents.](https://web.archive.org/web/*/http://dia.music.tucows.com/*)
10. [TUCOWS Music "eunet" mirror contents.](https://web.archive.org/web/*/http://eunet.music.tucows.com/*)
11. [TUCOWS Music "brightnet" mirror contents.](https://web.archive.org/web/*/http://brightnet.music.tucows.com/*)
12. [TUCOWS Music "terra-br" mirror contents.](https://web.archive.org/web/*/http://terra-br.music.tucows.com/*)
13. [TUCOWS Music "ev1" mirror contents.](https://web.archive.org/web/*/http://ev1.music.tucows.com/*)
14. [TUCOWS Music "fastex" mirror contents.](https://web.archive.org/web/*/http://fastex.music.tucows.com/*)
15. [TUCOWS Music "idirect" mirror contents.](https://web.archive.org/web/*/http://idirect.music.tucows.com/*)
16. [TUCOWS Music "uai" mirror contents.](https://web.archive.org/web/*/http://uai.music.tucows.com/*)
17. [NY Times article about PlayJ.](https://archive.nytimes.com/www.nytimes.com/library/tech/00/07/biztech/articles/07digital-music.html)
18. [Article about EverAd partnering with Launch.com.](https://www.dmnews.com/everad-launchcom-partner/)
19. [Article about EverAd partnering with J Records.](https://www.internetnews.com/marketing/everads-playj-partners-with-j-records/)
20. [BinaryObjectScanner protection information for PlayJ.](https://github.com/SabreTools/BinaryObjectScanner/blob/master/BinaryObjectScanner/Protection/PlayJ.cs)
21. [SabreTools PlayJ model data.](https://github.com/SabreTools/SabreTools.Models/tree/main/PlayJ)
22. [PlayJ page describing the launch of PlayJ.](https://web.archive.org/web/20000301013405/http://www.playj.com/digital_music.htm)
23. [Wired article about PlayJ.](https://www.wired.com/2000/03/ads-take-aim-at-online-music/)
24. [List of original PlayJ partners.](https://web.archive.org/web/20000229134632/http://www.playj.com/business_alliances.htm)

### Footnotes:

[^1]: [Official website for PlayJ. (Additional Resource #1)](https://web.archive.org/web/20000815053956/http://www.playj.com/)
[^2]: [News article about the launch of PlayJ. (Additional Resource #4)](https://en.globes.co.il/en/article-383855)
[^3]: [News article about the closure of PlayJ. (Additional Resource #5)](https://www.themarker.com/misc/2001-07-26/ty-article/0000017f-e690-df2c-a1ff-fed177870000)
[^4]: [PlayJ IANA assignment. (Additional Resource #3)](https://www.iana.org/assignments/media-types/audio/vnd.everad.plj)
[^5]: Found in some early CDS-200 music CDs. [TODO: Add source.]
[^6]: Found in the [PlayJ CDN contents](https://web.archive.org/web/*/dlp.playj.com*). Please note that not all songs seem to have been archived correctly, such as several that have seemingly been truncated to ~1 MB/MiB.
[^7]: Found in TUCOWS Music and its various mirrors (Additional Resources #8-#16). Please note that not all songs seem to have been archived correctly, such as several that have seemingly been truncated to ~1 MB/MiB.
[^8]: [NY Times article about PlayJ. (Additional Resource #17)](https://archive.nytimes.com/www.nytimes.com/library/tech/00/07/biztech/articles/07digital-music.html)
[^9]: [Article about EverAd and Launch.com beginning a partnership. (Additional Resource #20)](https://www.dmnews.com/everad-launchcom-partner/)
[^10]: [BinaryObjectScanner protection information for PlayJ. (Additional Resource #20)](https://github.com/SabreTools/BinaryObjectScanner/blob/master/BinaryObjectScanner/Protection/PlayJ.cs)
[^11]: [SabreTools PlayJ model data. (Additional Resource #21)](https://github.com/SabreTools/SabreTools.Models/tree/main/PlayJ)
[^12]: [PlayJ page describing the launch of PlayJ. (Additional Resource #22)](https://web.archive.org/web/20000301013405/http://www.playj.com/digital_music.htm)
[^13]: [Wired article about PlayJ. (Additional Resource #23)](https://www.wired.com/2000/03/ads-take-aim-at-online-music/)
[^14]: [PlayJ Studio Installer. (Additional Resource #6)](https://web.archive.org/web/20010417025347/http://dlp.playj.com:80/playj/PlayJIns266.exe)