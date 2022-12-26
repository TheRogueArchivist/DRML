### Names:
Bitpool[^1]

### Developers:
Unknown.

### Years Active: 
1998[^2]-2003[^3]

### Known Versions & Differences: 
No official versions are used, but there are two distinct generations currently known to exist. 

The older generation (generally found on discs pre-1999) doesn't have any extra protection-related tracks, and contains between 1-4 errors per disc (TODO: Verify if these are C2 errors).

The newer generation of Bitpool adds a protection-related audio and data track to end of the disc when the game would otherwise only contain a single data track. This means that these discs have 3 tracks in total. When the game itself consists of a data track and game-related audio tracks, Bitpool doesn't add any additional tracks. This is likely due to the issues these tracks would cause if played as audio tracks in an audio CD player. It also has 1,000s-10,000s of errors per disc (TODO: Check if any of these are C2 errors).

Older, data track only: [Redump entry 48276.](http://redump.org/disc/48276)

Older, data and audio tracks: [Redump entry 51376.](http://redump.org/disc/51376)

Newer, data track only: [Redump entry 31782.](http://redump.org/disc/31782)

Newer, data and audio tracks: [Redump entry 44976.](http://redump.org/disc/44976)

### Known Samples: 
#### Confirmed: 
Redump entries
[31782](http://redump.org/disc/31782),
[35476](http://redump.org/disc/35476),
[35480](http://redump.org/disc/35480),
[44976](http://redump.org/disc/44976),
[48276](http://redump.org/disc/48276), 
[50229](http://redump.org/disc/50229), 
[51376](http://redump.org/disc/51376), 
[52626](http://redump.org/disc/52626), 
[67046](http://redump.org/disc/67046), and 
[68160](http://redump.org/disc/68160).

#### Unconfirmed:
[All Redump entries listed as having Bitpool as a protection.](http://redump.org/discs/quicksearch/bitpool/protection/only)

### Categories: 
Optical Copy Protection

### Protection Features:
Copy Prevention; Padded/Dummy Files; Misleading Tracks; C2 Errors [TODO: Verify this]; Other Errors

### Minimum Required Image Format to Run:
ISO (Assuming no active checks in place, needs to be double checked).

### Detection Related Information:
https://github.com/mnadareski/BurnOutSharp/blob/master/BurnOutSharp/ProtectionType/Bitpool.cs

### Preservation Instructions:
[TODO]

### Overall Description:
Bitpool is a copy protection found most commonly in German releases. It makes use of bad sectors [TODO: Check if these are C2 errors]. It is currently unknown if these bad sectors are merely to prevent the disc from being dumped, or if the game checks these as a signature. 

I'm not entirely sure of the extent that Bitpool "creatively uses" the ISO9660 filesystem, but there are many, many issues in the filesystems present on these discs. The most obvious example is the "CD.IDX" file universally found in Bitpool games, which is often reported as being too large of a file to fit on a CD, as well as various other files that do the same but tend to vary from disc to disc. Investigating these files in a hex editor gives confusing results, at times matching the setup executable, or having other seemingly valid data before reaching the erroneous part of the file.

The additional protection tracks used by newer Bitpool releases appear to be used to complicate dumping the disc. The purpose of the audio tracks (which SHOULD be audio silence) is unknown, aside from the added complexity. The extra data track is presumed to point towards the first data track, which is known to cause some older dumping software to incorrectly believe that there are two full-size data tracks, causing it to error out.

All that being said, it seems that both the older and newer generations of Bitpool seem to be a semi-passive protection. A pattern has been observed where the game itself stores some data exclusively on the disc, requiring you to use a CD (whether real or virtual) to play. It appears that essential game files are padded and corrupted, meaning that they can't be copied off the disc directly, while the game is able to only read the correct portions of the file. But extracting the data from track 1 to an ISO file directly, completely ignoring protected tracks and read errors, still allows you to run the game with seemingly no issue. This seems to indicate that aside from a basic disc check, no active checks are occuring and that the protection is mostly aimed at preventing the disc from being copied or dumped. Tested with Redump entries [51376](http://redump.org/disc/51376) and [61744](http://redump.org/disc/61744/).

TODO: Investigate executables to see if the disc check itself is Bitpool, or if it's implemented independently by the game developers.

### Known Associated Files:
#### "CD.IDX": 
Found in seemingly every Bitpool protected game, the contents of this file are not consistent. This file is generally padded to be larger than the capacity of a CD, causing errors when trying to copy this file off the disc.

#### "bitpool.rsc":
Found in some Bitpool protected games, and the purpose is currently unknown. It is likely the origin of the name "Bitpool". Found in Redump entry [61744](http://redump.org/disc/61744/).

#### "CRC_A", "CRC_B", "CRC_C", and "CRC_D":
A set of 4 identically sized (within the same game, not between games), padded files present in Redump entries [31782](http://redump.org/disc/31782) and [35476](http://redump.org/disc/35476).

#### "LEADOUT.OFS": 
A completely 00'd out file present in some Bitpool protected games, purpose currently unknown. Found in Redump entries [50229](http://redump.org/disc/50229) and [52626](http://redump.org/disc/52626).

#### "_":
A padded dummy file present in multiple games, appears in some cases to be a copy of CD.IDX. Found in Redump entries [35480](http://redump.org/disc/35480),  [67046](http://redump.org/disc/67046), and [68160](http://redump.org/disc/68160).

#### Game Specific Files:

##### "__":
A padded file present in Redump entry [50229](http://redump.org/disc/50229).

#####  "01.rsc" and "jmptable.rsc":
Padded files present in Redump entry [52626](http://redump.org/disc/52626).

##### "AMAZON.GDB", "DB.GDB",  "DV.GDB", "MENTOR.GDB", "PIMMONS.GDB", "SAJIKI.GDB", and "TUTORIALS.GDB":
Padded files found in Redump entry [44976](http://redump.org/disc/44976).

##### "BDA.cab" + "BDB.RSC":
Padded files present in Redump entry [67046](http://redump.org/disc/67046).
 
#####  "ds.dat": 
A padded file present in Redump entry [35476](http://redump.org/disc/35476).

### Additional Resources & Documentation:
[List of DRM detection tools, including one that explicitly detects Bitpool](http://www.gameburnworld.com/cdridentifyingtools.shtml)

[A similar list with two different tools that explicitly detect Bitpool](https://www.cdmediaworld.com/hardware/cdrom/cd_utils_2.shtml)

### Footnotes:
[^1]: No official source for this name, but it's commonly used and likely originated from the "bitpool.rsc" file.
[^2]: [Redump entry 48276.](http://redump.org/disc/48276)
[^3]: [Redump entry 50229.](http://redump.org/disc/50229)
