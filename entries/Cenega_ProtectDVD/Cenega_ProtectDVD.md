### Names:

Cenega ProtectDVD[^1]

### Developers:

Cenega[^1]

### Years Active: 

~2006[^2] - ~2009[^3]

### Known Versions & Differences: 

There are two distinct versions that have been cataloged so far. One version displays a "Checking media" screen before attempting to start the game (Redump entries [31422](http://redump.org/disc/31422) and [85070](http://redump.org/disc/85070/)), and another displays an error message that says "Trwa weryfikacja nośnika. Proszę czekać…", which translates to "Media verification is in progress. Please wait…" (IA item ["speed-pack"](https://archive.org/details/speed-pack)).

Cenega error window present in IA item ["speed-pack"](https://archive.org/details/speed-pack):

!["Cenega" - "Virtual drive was detected please insert original disc in drive." - "Check disk" - "Cancel"](./Cenega_ProtectDVD_Error_Message.png "Cenega error window.")

Cenega "Media verification" window present in Redump entries [31422](http://redump.org/disc/31422) and [85070](http://redump.org/disc/85070/):

!["Cenega" - "Trwa weryfikacja nośnika. Proszę czekać…".](./Cenega_ProtectDVD_Media_Verification.png "Cenega 'Media Verification' Window")

### Known Samples: 

#### Confirmed: 

* Mafia (Redump entry [31422](http://redump.org/disc/31422)/IA item ["mafia_202106"](https://archive.org/details/mafia_202106)).
* Tomb Raider Ultimate Edition (Redump entry [85070](http://redump.org/disc/85070/)/IA item ["tr_ue_dvd2"](https://archive.org/details/tr_ue_dvd2)).
* Speed Pack (IA item ["speed-pack"](https://archive.org/details/speed-pack)).

#### Unconfirmed:

* [Venetica 1.02 (Polish)](https://fileforums.com/showthread.php?t=87754).
* [Majesty 2 (Non-Steam)](https://www.shouldiremoveit.com/Majesty-2-41020-program.aspx).[^4]
* [Myst Antologia (Polish) (Likely Erroneous)](http://redump.org/disc/31355/).
* [Enemy Territory: Quake Wars (Płyta Dodatkowa) (Likely Erroneous)](http://redump.org/disc/23716/).
* [All Redump entries listed as having "ProtectDVD" as a protection](http://redump.org/discs/quicksearch/protectdvd/protection/only).

### Categories: 

Optical Copy Protection

### Protection Features:

Virtual Drive Detection

### Minimum Required Image Format to Run:

ISO[^8]

### Software Known to Detect:

BurnOut [^5], BurnOutSharp[^6], ProtectionID[^7]

### Detection Related Information:

https://github.com/mnadareski/BurnOutSharp/blob/master/BurnOutSharp/ProtectionType/CenegaProtectDVD.cs

### Preservation Instructions:

A simple ISO dump of these games appears to suffice, as all the protection features currently known only detect virtual drive use. [TODO: Verify if (and if applicable, how) this DRM checks for burned discs.]

### Overall Description:

Cenega ProtectDVD is a Polish DVD copy protection created by the publisher Cenega. It verifies the authenticity of the disc through, at a minimum, virtual drive detection. In Redump entries [31422](http://redump.org/disc/31422) and [85070](http://redump.org/disc/85070/), mounting an ISO file as a SCSI virtual drive in Daemon Tools is seemingly enough to pass this check. A DT virtual drive doesn't work, and is presumably checked for by the DRM. Strangely, IDE virtual drives appear to crash the game at the protection check, though this doesn't appear to be an intentional protection feature. IA item ["speed-pack"](https://archive.org/details/speed-pack) specifically needs the ISO to be mounted to a physical drive in order to pass the protection check. This has been confirmed (but not by me) to be sufficient to allow the game to load at least in to the main game menu. Gameplay itself is untested.

It also appears to have a trial-ware component, based on strings such as "Trial period will expire after one execution." present in "cenega.dll". It is currently unknown if/when this is actually put to use, and further investigation on if they distributed trials of games online is needed.

[TODO: Verify if (and if applicable, how) this DRM checks for burned discs.]

### Known Associated Files:

#### "cenega.dll": 
The main protection library, found in every known sample so far.

#### "ProtectDVD.dll":
Not present directly, but is the internal export name of "cenega.dll".

#### Game Specific Files:

##### "game.exe":
The protected game file present in Redump entry [31422](http://redump.org/disc/31422).

##### "tra.exe":
The protected game file present in Redump entry [85070](http://redump.org/disc/85070).

#####  "Classic Car Racing.exe" and "som.exe":
The protected game file present in IA item ["speed-pack"](https://archive.org/details/speed-pack).

### Known Associated Executable Sections:

#### ".cenega":
A section found within seemingly every protected executable.

#### ".cenega0", ".cenega1", and ".cenega2":
Sections that are all consistently found within "cenega.dll".

### Additional Resources & Documentation:
[The homepage for ProtectionID, which includes a changelog that mentions the inclusion of "Cenega ProtectDVD" detection.](http://www.gameburnworld.com/cdridentifyingtools.shtml)

### Footnotes:
[^1]: https://web.archive.org/web/20210331144912/https://protectionid.net/
[^2]: [Redump entry 31355.](http://redump.org/disc/31355)
[^3]: [Redump entry 31422.](http://redump.org/disc/31422)
[^4]: The version of the game currently for sale on Steam has been checked and does not appear to have this DRM present.
[^5]: https://www.softpedia.com/progChangelog/BurnOut-Changelog-103960.html
[^6]: https://github.com/mnadareski/BurnOutSharp
[^7]: https://web.archive.org/web/20210331144912/https://protectionid.net/
[^8]: ISO is confirmed to allow the games to begin in Redump entries [31422](http://redump.org/disc/31422) and [85070](http://redump.org/disc/85070/) when mounted as a SCSI virtual drive using Daemon Tools, gameplay not thoroughly tested. IA item ["speed-pack"](https://archive.org/details/speed-pack) is confirmed to pass the protection check into at least the main game menu when mounted specifically to a physical drive using Daemon Tools. Unlike the rest of the samples, using a SCSI virtual drive doesn't pass the protection check.
