Neato-XV-Series-Cruz-Rev-113-Update
===================================

 

Files for updating the firmware of a Neato XV Rev 113/Cruz board offline
------------------------------------------------------------------------

 

### The Problem:

As of November 2015, Neato has stopped providing firmware updates via their
previous online updater. I recently replaced the Rev 113/Cruz main board in my
XV21 and the new one shipped with firmware version 2.4.

 

Unfortunately, version 2.4 does not include many of the newest features of the
latest XV firmwares, such as corner cleaning/"Corner Clever”. Details on the
different versions of firmware are available on Wikipedia here:
<https://en.wikipedia.org/wiki/Neato_Robotics#Firmware>

 

I did find an offline updater for the Rev 64/Binky version under heXor’s
NeatoControl Bitbucket here:
<https://bitbucket.org/heXor/neatocontrol/downloads>. However, I made the
mistake of using that on my Rev 113/Cruz board and… bricked it. Oops...

 

So, with that in mind, I figured that the offline updater files provided by
heXor gave a good starting point… If I could only find firmware files for Rev
113/Cruz somewhere. Fortunately, I saw this note on the XV11 Hacking wikispace
(<https://xv11hacking.wikispaces.com/Hacking+with+Neato+v3.0>) - "The Neatos
that are delivered with Firmware 3.0 are a different hardware revision compared
to previous models. **Previous versions (incl. the Vorwerk VR100) are codename
'Cruz’.**"

 

With that in mind, I found multiple firmware files on the Vorwerk website here:
<http://kobold.vorwerk.de/de/service/software-updates/saugroboter/vr100/#>. Only
problem was - All of the ZIP files on the site were password protected, with no
password to be found. After a bit of digging, I found this tweet, which happened
to have the password for the ZIP files (VORVR100!%) -
<https://twitter.com/afripowered/status/427134106946650112>

 

Armed with that, I took each firmware file from Vorwerk’s site, and created an
update ZIP file based on heXor’s offline update script for each of the firmware
files provided by Vorwerk. I tested each of them on my own XV21 and they worked
for me personally. However, I take no responsibility if these cause any damage
to your Neats if you so choose to use them. Upgrade at your own risk!

 

### To Upgrade:

1.  Connect your Neato to your computer via a MicroUSB cable

2.  Download and unzip the respective firmware ZIP file from this github repo

3.  Double click/execute run.bat
