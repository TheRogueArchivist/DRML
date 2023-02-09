### Names: 

Freelock[^1], FREELOCK[^1]

### Developers:

Scooby II[^1], Xperience[^1]

### Years Active: 
1999[^2] - 2000[^1]

### Known Versions & Differences: 

Version 1.0: Initial release. [[Download]](https://web.archive.org/web/20040615215309/http://www.geocities.com/SiliconValley/Code/6061/programs/flock10.zip)

Version 1.1: There is no known reference to this version ever having existed.

Version 1.2: Added "overburn" protection and added a new option to improve compatibility with some drives.[^3] [[Download]](https://web.archive.org/web/20091027114741/http://geocities.com/siliconvalley/code/6061/programs/flock12.zip)

Version 1.2a: Patch to 1.2 that's seemingly more common, exact change unknown. [[Download]](https://web.archive.org/web/20040613085437/http://www.geocities.com/SiliconValley/Code/6061/programs/Flock12a.zip)

Version 1.3: Separate intentionally bad data from main executable.[^4] [[Download]](https://web.archive.org/web/20040606222542/http://www.geocities.com/SiliconValley/Code/6061/programs/flock13.zip)

### Known Samples: 

#### Confirmed: 

[Coverdisc that includes the Freelock 1.3 program.](https://archive.org/details/WINMAG29)

#### Unconfirmed:

N/A.

### Categories: 

DRM Builder, Optical Copy Protection

### Protection Features:
Copy Prevention; Misleading Tracks; Other Errors [TODO: Verify what kind of error.]; Overburn

### Minimum Required Image Format to Run:
ISO (Assuming only the typical PSX data is needed) / CUE (Assuming multiple tracks contain actual audio/data)

### Detection Related Information:
https://github.com/mnadareski/BurnOutSharp/blob/master/BurnOutSharp/ProtectionType/FreeLock.cs

### Preservation Instructions:
[TODO]

### Overall Description:

Freelock is a DRM that allows end-users to burn a copy protected PSX CD-R for free. It accomplishes this by adding additional dummy tracks (by default, one mode 1 and one mode 2 track) to an image before burning, and then attempting to use a corrupted file to burn to these tracks. This causes the write process to fail at the end, after the PSX data has already finished being burned. It also has an optional feature to instead overburn the disc to a total of 95 minutes as well, using random data in random types of tracks. All together, these features are intended to make it passively difficult for another person to copy the resulting CD-R.

Official description of how it works[^5]:

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

### Known Associated Files:

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

#### "WINDOWS\freelock.ico"
The icon for Freelock 1.2+.

#### "WINDOWS\Freelock.pif"
The MS-DOS shortcut for Freelock 1.2+.

#### "FREELOCK.13"/"FREELOCK13"
The partition name for "FREELOCK.IMG" in Freelock 1.3.

#### "FL.DAT"
An intentionally corrupt file used instead of the main executable in Freelock 1.3.

### Additional Resources & Documentation:

* [Official site as indicated in "FREELOCK.TXT" in Freelock 1.0-1.2a (1999/10/01).](https://web.archive.org/web/19991001075001/http://www.geocities.com/SiliconValley/Code/6061/)
* [Official site as indicated in "FREELOCK.TXT" in Freelock 1.0-1.2a (2000/08/22).](https://web.archive.org/web/20000822124542/http://www.geocities.com/SiliconValley/Code/6061/)
* [Official site as indicated in "FREELOCK.TXT" in Freelock 1.3 (2001/08/1).](https://web.archive.org/web/20010801181527/http://www.geocities.com/freelock_psx/)
* [Official instructions ("FREELOCK FOR DUMMIES") (1999/11/28).](https://web.archive.org/web/19991128071357/http://www.geocities.com/SiliconValley/Code/6061/instruct.htm)
* [Official instructions (2000/01/18).](https://web.archive.org/web/20000118061405/http://www.geocities.com:80/SiliconValley/Code/6061/instruct.htm)
* [Trademark infringement notice regarding the use of the phrase "For Dummies" (2000/10/17).](https://web.archive.org/web/20001017233343/http://www.geocities.com/SiliconValley/Code/6061/IDGBOOKS.htm)
* [Freelock joke disclaimer (2001/04/11).](https://web.archive.org/web/20010411230821/http://www.geocities.com/SiliconValley/Code/6061/disclaimer.htm)
* [List of sites that featured Freelock (2001/08/03).](https://web.archive.org/web/20010803222336/http://www.geocities.com/freelock_psx/links.htm)
* [Softpedia page for Freelock.](https://www.softpedia.com/get/CD-DVD-Tools/CD-DVD-Images-Utils/Freelock.shtml)
* [CMW page that includes Freelock.](https://www.cdmediaworld.com/hardware/cdrom/cd_utils_3.shtml)
* [Forum post discussing Freelock and how it can be used for VCDs/SVCDs.](https://forum.videohelp.com/threads/56579-How-to-copy-protect-a-VCD-SVCD-v2-0)
* [Unofficial GUI for Freelock.](https://consolecopyworld.com/psx/psx_utils_misc.shtml)
* [Coverdisc that includes Freelock.](https://archive.org/details/WINMAG29)

### Footnotes:

[^1]: https://web.archive.org/web/20010801181527/http://www.geocities.com/freelock_psx/
[^2]: https://web.archive.org/web/19991001075001/http://www.geocities.com/SiliconValley/Code/6061/
[^3]: Possibly incomplete, put together via comparing the "FREELOCK.TXT" file present in 1.0 and 1.2.
[^4]: Mentioned in the "FREELOCK.TXT" file present in version 1.3, personally confirmed.
[^5]: Found in the "FREELOCK.TXT" file present in version 1.3.
