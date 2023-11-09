### Names: 

Freelock[^Freelock_Website_1999], FREELOCK[^Freelock_Website_1999], FreeLock[^BurnOut_Changelog]

[^Freelock_Website_1999]: [Official Freelock site as indicated in "FREELOCK.TXT" in Freelock 1.0-1.2a. (Archived 1999-10-01)](https://web.archive.org/web/19991001075001/http://www.geocities.com/SiliconValley/Code/6061/)

[^BurnOut_Changelog]: [Changelog for BurnOut that shows it supporting "FreeLock". (Archived 2023-10-02)](https://web.archive.org/web/20231002225132/https://www.softpedia.com/progChangelog/BurnOut-Changelog-103960.html)

***

### Categories: 

DRM Builder, Optical Copy Protection

***

### Developers:

Scooby II[^Freelock_Website_2001], Xperience[^Freelock_Website_1999]

[^Freelock_Website_2001]: [Official Freelock site as indicated in "FREELOCK.TXT" in Freelock 1.3. (Archived 2001-08-01)](https://web.archive.org/web/20010801181527/http://www.geocities.com/freelock_psx/)

***

### Years Active: 
1999[^Freelock_Website_1999] - 2000[^Freelock_Website_2001]

***

### Known Versions & Differences: 

* Version 1.0: Initial release. 

* Version 1.1: There is no known reference to this version ever having existed.

* Version 1.2: Added "overburn" protection and added a new option to improve compatibility with some drives.[^Freelock_1.2_Note]

* Version 1.2a: Patch to 1.2 that's seemingly more common, exact change unknown.

* Version 1.3: Separate intentionally bad data from main executable.[^Freelock_1.3_Note]

[^Freelock_1.2_Note]: Found by comparing the "FREELOCK.TXT" file present in 1.0 and 1.2.

[^Freelock_1.3_Note]: Mentioned in the "FREELOCK.TXT" file present in version 1.3, personally confirmed.

***

### Known Samples: 

#### Confirmed: 

* Freelock 1.0. [^Freelock_1.0_Download]

* Freelock 1.2. [^Freelock_1.2_Download]

* Freelock 1.2a. [^Freelock_1.2a_Download]

* Freelock 1.3. [^Freelock_1.3_Download]

* "Win Magazine 29" coverdisc that includes the Freelock 1.3 program. [^Win_Magazine_29]

#### Unconfirmed:

N/A.

[^Freelock_1.0_Download]: [Freelock 1.0. (Download) (Archived 2004-06-15)](https://web.archive.org/web/20040615215309/http://www.geocities.com/SiliconValley/Code/6061/programs/flock10.zip)

[^Freelock_1.2_Download]: [Freelock 1.2. (Download) (Archived 2009-10-27)](https://web.archive.org/web/20091027114741/http://geocities.com/siliconvalley/code/6061/programs/flock12.zip)

[^Freelock_1.2a_Download]: [Freelock 1.2a. (Download) (Archived 2004-06-13)](https://web.archive.org/web/20040613085437/http://www.geocities.com/SiliconValley/Code/6061/programs/Flock12a.zip)

[^Freelock_1.3_Download]: [Freelock 1.3. (Download) (Archived 2004-06-13)](https://web.archive.org/web/20040606222542/http://www.geocities.com/SiliconValley/Code/6061/programs/flock13.zip)

[^Win_Magazine_29]: ["Win Magazine 29" coverdisc that includes Freelock.](https://archive.org/details/WINMAG29)

***

### Protection Features:
Copy Prevention; Misleading Tracks; Disc Errors; Overburn

***

### Minimum Required Image Format to Run:
ISO (Assuming only the typical PSX data is needed) / CUE (Assuming multiple tracks contain actual audio/data)

***

### Software Known to Detect:

BurnOut[^BurnOut_Changelog], BinaryObjectScanner[^Freelock_BOS]

[^Freelock_BOS]: [BinaryObjectScanner's Freelock detection code.](https://github.com/SabreTools/BinaryObjectScanner/blob/master/BinaryObjectScanner/Protection/FreeLock.cs)


***

### Detection Related Information:

https://github.com/SabreTools/BinaryObjectScanner/blob/master/BinaryObjectScanner/Protection/FreeLock.cs
***

### Preservation Instructions:

[TODO]

***

### Overall Description:

Freelock was a free DRM that allowed end-users to burn copy protected PSX CD-Rs. It accomplished this by adding additional dummy tracks (by default, one mode 1 and one mode 2 track) to an image before burning, and then attempting to use a corrupted file to burn to these tracks. This caused the write process to fail at the end, after the PSX data has already finished being burned. It also had an optional feature to instead overburn the disc to a total of 95 minutes as well, using random data in random types of tracks. All together, these features were intended to make it passively difficult for another person to copy the resulting CD-R.

Official description of how it worked:[^Freelock_Description]

> Freelock alters the layout of a CD image prior to recording, making the
 resulting copy virtually impossible to duplicate.  This prevents most people
 making copies of your copies.
>
> Freelock's standard protection works by adding two additional tracks to the
 CD, a "Mode 1" data track and a "Mode 2" data track.  This is "illegal", and
 most writing software will refuse to copy the disc.  Just for good measure,
 though, the file used for the tracks is deliberately damaged (have you tried
 copying it yet?), so the writing process will ALWAYS fail!
>
> Freelock's "overburn" protection is different.  This adds extra tracks to the CD, boosting it up to 95 minutes.  Each of these extra tracks (a random mix of audio, "Mode 1" and "Mode 2" tracks) adds around 10Mb to the CD, potentially pushing the CD contents off the edge of the disc!  When you write
this CD, all of the PlayStation data will be written, then the CD will be
filled up until the CD writer runs out of space and spits out the disc!
The overburn feature of Freelock requires an extra 11Mb of your hard disk to
store the track data.  The file used for this can be created by running
GENLOCK.EXE, found on the Freelock diskette.  The file created by Genlock is
of random length between 9 and 11Mb (but is a multiple of 2352 bytes in
length - this is required by CDRWIN) and contains random data.
>
> NOTE: When Freelock is used to protect a CD, the copying process will be
abandoned when CDRWIN or DAO encounters the (deliberate) errors in the last
tracks.  In other words, CDRWIN OR DAO WILL ALWAYS STOP WITH AN "ERROR" WHEN
YOU WRITE A FREELOCKED CD!  This is normal.
>
> A new option has been added to support drives such as the HP 8100, which
cannot write Mode 1 and Mode 2 tracks on the same CD.  Using the /M option
forces FREELOCK to add either Audio or Mode 2 tracks, and prevents the
addition of Mode 1 tracks.  When used in conjunction with the /O option,
only Audio tracks are added.  This is a last-resort method of protection -
if you have a drive that is particularly fussy when it comes to writing
"strange" disks, it may be your only choice.

It is intended to be run off of a "key" floppy disk, with the first step being to install the provided IMG to a floppy disk. Next you use it to modify a CUE image with the protection options you want, and lastly burn the resulting image to a disc.

[TODO: Needs to be tested personally, currently untested due to OTVDM not currently working with Freelock.]

[^Freelock_Description]: Found in the "FREELOCK.TXT" file present in version 1.3.

***

### Known Associated Files:[^Freelock_Files]

#### "FREELOCK.IMG": 
The floppy disk image every version of Freelock is distributed in.

#### "FREELOCK":
The partition name for "FREELOCK.IMG" in Freelock 1.0-1.2a.

#### "FREELOCK.TXT"
A text file included with every version of Freelock.

#### "FREELOCK.EXE"
The main executable for every version of Freelock. Is intentionally corrupted in Freelock 1.0-1.2a.

#### "GENLOCK.EXE"
The executable that creates the "FREELOCK.DAT" file needed to use the overburn option in Freelock 1.2+.

#### "FREELOCK.DAT"
The file containing random data used by the overburn option in Freelock 1.2+.

#### "freelock.ico"
The icon for Freelock 1.2+.

#### "Freelock.pif"
The MS-DOS shortcut for Freelock 1.2+.

#### "FREELOCK.13"/"FREELOCK13"
The partition name for "FREELOCK.IMG" in Freelock 1.3.

#### "FL.DAT"
An intentionally corrupt file used instead of the main executable in Freelock 1.3.

[^Freelock_Files]: All of the listed files can be found within or when using the appropriate versions of Freelock.

***

### Additional Resources & Documentation:

#### Official Resources:

* [Freelock 1.0. (Download) (Archived 2004-06-15)](https://web.archive.org/web/20040615215309/http://www.geocities.com/SiliconValley/Code/6061/programs/flock10.zip)

* [Freelock 1.2. (Download) (Archived 2009-10-27)](https://web.archive.org/web/20091027114741/http://geocities.com/siliconvalley/code/6061/programs/flock12.zip)

* [Freelock 1.2a. (Download) (Archived 2004-06-13)](https://web.archive.org/web/20040613085437/http://www.geocities.com/SiliconValley/Code/6061/programs/Flock12a.zip)

* [Freelock 1.3. (Download) (Archived 2004-06-13)](https://web.archive.org/web/20040606222542/http://www.geocities.com/SiliconValley/Code/6061/programs/flock13.zip)

* [Official Freelock site as indicated in "FREELOCK.TXT" in Freelock 1.0-1.2a. (Archived 1999-10-01)](https://web.archive.org/web/19991001075001/http://www.geocities.com/SiliconValley/Code/6061/)

* [Official Freelock site as indicated in "FREELOCK.TXT" in Freelock 1.0-1.2a. (Archived 2000-08-22)](https://web.archive.org/web/20000822124542/http://www.geocities.com/SiliconValley/Code/6061/)

* [Official Freelock site as indicated in "FREELOCK.TXT" in Freelock 1.3. (Archived 2001-08-01)](https://web.archive.org/web/20010801181527/http://www.geocities.com/freelock_psx/)

* [Instructions for using Freelock ("FREELOCK FOR DUMMIES"). (Archived 1999-11-28)](https://web.archive.org/web/19991128071357/http://www.geocities.com/SiliconValley/Code/6061/instruct.htm)

* [Instructions for using Freelock. (Archived 2000-01-18)](https://web.archive.org/web/20000118061405/http://www.geocities.com:80/SiliconValley/Code/6061/instruct.htm)

* [Trademark infringement notice regarding the use of the phrase "For Dummies". (Archived 2000-10-17)](https://web.archive.org/web/20001017233343/http://www.geocities.com/SiliconValley/Code/6061/IDGBOOKS.htm)

* [Freelock joke disclaimer. (Archived 2001-04-11)](https://web.archive.org/web/20010411230821/http://www.geocities.com/SiliconValley/Code/6061/disclaimer.htm)

* [List of sites that featured Freelock. (Archived 2001-08-03)](https://web.archive.org/web/20010803222336/http://www.geocities.com/freelock_psx/links.htm)

#### Unofficial Resources:

* [Softpedia page for Freelock. (Archived 2023-10-02)](https://web.archive.org/web/20231002223608/https://www.softpedia.com/get/CD-DVD-Tools/CD-DVD-Images-Utils/Freelock.shtml)

* [CDMediaWorld page that includes multiple versions of Freelock. (Archived 2023-10-02)](https://web.archive.org/web/20231002223415/https://www.cdmediaworld.com/hardware/cdrom/cd_utils_3.shtml)

* [Forum post discussing Freelock and how it can be used for VCDs/SVCDs. (Archived 2023-10-02)](https://web.archive.org/web/20231002223238/https://forum.videohelp.com/threads/56579-How-to-copy-protect-a-VCD-SVCD-v2-0)

* [ConsoleCopyWorld page featuring both Freelock v1.3 and an unofficial GUI for Freelock. (Archived 2023-10-02)](https://web.archive.org/web/20231002222813/https://consolecopyworld.com/psx/psx_utils_misc.shtml)

* [Unofficial GUI for Freelock. (Download) (Archived 2023-02-09)](https://web.archive.org/web/20230209060909/https://dl.consolecopyworld.com/dl.php?c=psx&f=pfui_03!zip)

* ["Win Magazine 29" coverdisc that includes Freelock.](https://archive.org/details/WINMAG29)

* [Changelog for BurnOut that shows it supporting "FreeLock". (Archived 2023-10-02)](https://web.archive.org/web/20231002225132/https://www.softpedia.com/progChangelog/BurnOut-Changelog-103960.html)

* [BinaryObjectScanner's Freelock detection code.](https://github.com/SabreTools/BinaryObjectScanner/blob/master/BinaryObjectScanner/Protection/FreeLock.cscs)

***

### Authors/Contributors:

* TheRogueArchivist - Entry author.

***

### Footnotes:
