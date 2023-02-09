### Names:

Cenega ProtectDVD[^1]

### Developers:

Cenega[^1]

### Years Active: 

~2006[^2] - ~2009[^3]

### Known Versions & Differences: 

There are two distinct versions that have been cataloged so far. One version displays a "Checking media" screen before attempting to start the game (Redump entries [31422](http://redump.org/disc/31422) and [85070](http://redump.org/disc/85070/)), and another displays an error message that says "Trwa weryfikacja nośnika. Proszę czekać…", which translates to "Media verification is in progress. Please wait…" (IA item ["speed-pack"](https://archive.org/details/speed-pack)).

[TODO: Investigate what causes this error to occur, and what the "Media verification" screen checks for.]

Cenega error window present in IA item ["speed-pack"](https://archive.org/details/speed-pack):

!["Cenega" - "Virtual drive was detected please insert original disc in drive." - "Check disk" - "Cancel"](./Cenega_ProtectDVD_Error_Message.png "Cenega error window.")

Cenega "Media verification" window present in Redump entries [31422](http://redump.org/disc/31422) and [85070](http://redump.org/disc/85070/):

!["Cenega" - "Trwa weryfikacja nośnika. Proszę czekać…".](./Cenega_ProtectDVD_Media_Verification.png "Cenega 'Media Verification' Window")

There is a disc that appears to contain an older, pre-2009 version that's present on Redump entry [31355](http://redump.org/disc/31355). Any differences in version are currently unknown, due to this entry being MIA.

### Known Samples: 

#### Confirmed: 

* Mafia (Redump entry [31422](http://redump.org/disc/31422)/IA item ["mafia_202106"](https://archive.org/details/mafia_202106)).
* Tomb Raider Ultimate Edition (Redump entry [85070](http://redump.org/disc/85070/)/IA item ["tr_ue_dvd2"](https://archive.org/details/tr_ue_dvd2)).
* Speed Pack (IA item ["speed-pack"](https://archive.org/details/speed-pack)).

#### Unconfirmed:

* [Venetica 1.02 (Polish)](https://fileforums.com/showthread.php?t=87754).
* [Majesty 2 (Non-Steam)](https://www.shouldiremoveit.com/Majesty-2-41020-program.aspx).[^4]
* [All Redump entries listed as having "ProtectDVD" as a protection.](http://redump.org/discs/quicksearch/protectdvd/protection/only).

### Categories: 

Optical Copy Protection

### Protection Features:

[TODO]
IA item ["mafia_202106"](https://archive.org/details/mafia_202106) confirmed not to use DMI, as all DMI data from this disc is 00. DPM is next current suspicion.

### Minimum Required Image Format to Run:

MDS (Assuming this protection uses DPM, currently unconfirmed). ISO is confirmed to not work on IA items ["speed-pack"](https://archive.org/details/speed-pack) and ["mafia_202106"](https://archive.org/details/mafia_202106).

### Detection Related Information:

https://github.com/mnadareski/BurnOutSharp/blob/master/BurnOutSharp/ProtectionType/CenegaProtectDVD.cs

### Preservation Instructions:

[TODO]

### Overall Description:

Cenega ProtectDVD is a Polish DVD copy protection created by the publisher Cenega. It appears to check for DPM (or something similar) to verify the authenticity of the disc. It also appears to have a trial-ware component, based on strings such as "Trial period will expire after one execution." present in "cenega.dll".

[TODO: Investigate exactly what's needed to get a protected game to run successfully.]

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
