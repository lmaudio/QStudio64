RELEASE-NOTES      
-------------  

Welcome to QStudio64 - a Linux Mint-based A/V-system for creative people!  


INTRODUCING 
----------- 

QStudio64 is an unofficial community-release for people interested in Linux Mint and Multimedia-Production.

Following older releases we bring it together with the great KXStudio-Repositories for professional A/V-productions!

So QStudio64 is not really an own distribution, as more a modified Linux Mint with integrated KXStudio-Repos and 
own improvements to give people who love Linux Mint (and MATE as the favourite desktop) 
an easy and stable entrance to the great world of making music, video and graphics-art with GNU/Linux! 

QStudio64 depends on open-source and it's philosophy. All software is free to use and share!*
[ATTENTION! *contains unfree propietary codec-librarys & closed-source Bitwig Studio]

As LTS-version it gets updates untill 2027! 


More informations about the KXStudio-Project you get here: https://kx.studio/

Documentation: https://kx.studio/Documentation


QStudio64-Blog: http://qstudio64.tumblr.com 

QStudio64-Homepage: https://qstudio64.io 



°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°
NOTE: QStudio64 21.1-Xi is our 10y anniversary-release with some fixes and upgrades. 
If you have QStudio64-21.1-SE/SX/XP installed you DON'T need to install it - just update!
°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°

Changes (XE/XP->Xi):

- All updates <17072025
- Kernel Linux 5.15.0-144-lowlatency x86_64 
- UEFI-SHIM Upgrade (Cert-Bugfix)
- Bitwig Studio 5.3.12*
- Mixxx 2.5.2 



Features:


SYSTEM
------
- basing on Linux Mint 21.1 (Vera), Mate 1.26
- Kernel Linux 5.15.0-xx-lowlatency x86_64 
- Ubuntu 22.04 package base

- KXStudio-Repositories** 

- Long-Term-Support until >April 2027
- upgradable to coming Linux Mint versions

- ALSA/Jack Soundsystem 

- supports modern A/V-Codecs and -Formats 
- supports many MIDI/DJ-Controllers & Audiointerfaces
- supports Touchscreens
-..


AUDIO-PRODUCTION
----------------
- Ardour 
- Bitwig Studio [Demo]
- Audacity 
- MIXXX 
- Qtracktor
- Hydrogen

- Cadence/Carla/Catia/Claudia
 
- non-mixer 
- non-sequenzer 
- non-timeline

- LMMS

- CALF-Plugins
- Guitarix
- Rakarrack

- QSampler
- Amsynth
- Hexter
- Helm
- Nekobee
- drumkv1
- Jamin
- Phasex
- QTractor
- setbfree
- ZynAddSubFx
- Synthv1

- Mudita24
- Asunder
- Soundconverter

- VLC-Player 
- Audacious 
- ...

PHOTO/GRAPHIC-PRODUCTION
------------------------

- Blender
- Darktable
- Gimp
- Inkscape
- Rawtherapee
- Pix
- Converseen
- Drawing

VIDEO-PRODUCTION
----------------
- Shotcut
- Handbrake
- WinFF
- xjadeo


OFFICE/INTERNET
---------------

- Brave Web-Browser

- Thunderbird (Mail)

- Element (Matrix-Chat)

- Libre Office

- Transmission





REQUIREMENTS:
-------------
Minimum: 1 GB of RAM, > 1,6 Ghz Processor (CPU, 64bit), 20GB of free harddisk
Recommend: > 4-8 GB RAM, >1,6 Ghz Dual-Core-Processor, > 100 GB of free harddisk/SSD 

QStudio64 ONLY supports modern 64bit-processors (CPU).
ON SYSTEMS WITH JUST 32bit-PROCESSORS IT WON`T BE BOOTING!

Before you start read the official Linux Mint 21.1 Release Notes:
https://linuxmint.com/rel_vera_mate.php




INSTALLATION:
-------------

To try QStudio64 just burn the iso-file on DVD or use USB/SD-Card with the "usb-image-writer" (Accessoires/Zubehör) and boot it as a Live-System from dvd/usb 

Install it from the booted live-system with the INSTALL-RELEASE-Button in ControlCenter (Steuerzentrale) onto your harddisk OR just use it as a special live system from stick.


The user/password-settings in live-system are the Linux Mint defaults:

user: mint

password: "empty"



It is recommend to have a clean offline install!



HOME DIRECTORY ENCRYPTION

---------------------------------------------------------------------------
IT S NOT RECOMMEND TO CHOOSE ENCRYPTION OF THE HOME-FOLDER DURING INSTALL!
---------------------------------------------------------------------------

- Encryption of the home-folder gots a bug in installer and ends maybe in an unfinished install!

- For performance and security-reasons better choose LUKS-Encryption of whole partitions!

Benchmarks have demonstrated that, in most cases, home directory encryption is slower than full disk encryption.

The move to systemd caused a regression in ecrypts which is responsible for mounting/unmounting encrypted home directories when you login and logout. 
Because of this issue, please be aware that in Mint 20 and newer releases, your encrypted home directory is no longer unmounted on logout: 

https://bugs.launchpad.net/ubuntu/+source/gnome-session/+bug/1734541.


-----------------------------------------------------------------------------
- Ignore the message of missing UEFI-partition on a NON-UEFI CSM/BIOS-System!
-----------------------------------------------------------------------------


Wait until the install-process is done!

Reboot and start QStudio64.





UEFI/MULTIBOOT:
---------------

QStudio64 supports UEFI with or without Secure Boot!

-> set secure-boot-password in installer!

It is recommend to give >20GB free space before installation if you have another OS installed!

More informations about Multiboot (with OSX/Windows) and UEFI you get in the documentations of LinuxMint/Ubuntu 
or the KXStudio webside: 

http://kxstudio.linuxaudio.org/Documentation:Manual:installing_kxstudio

-> boot usb-live-system in uefi-modus (EFI/UEFI)

-> start the installer - it will recognized other OS automaticly and lead you through the install process!

-> for advanced users/something else: create 1MB Bios Bootsector and an EFI-Partition (fat32)

-> Create an ext4-Linux-partition with mountpoint: /

-> delete old SWAP if exist because QStudio64 will use a swapfile!*
   
-> Install bootloader on first partition sda or on logical Linux-partition!

-> Install QStudio64 after partitioning!


If UEFI-Modus makes problems choose the normal CSM-BIOS-Mode and disable UEFI in your BIOS!





Partitioning:
-------------

Start the installer from live-system!

--> Default keyboard-preference is english > Select your desired keyboard-layout!

Choose INSTALL QStudio64 if you have a clean disk without another operating-system beneath!

The installer will recognize all free space and will format your drive with ext4!

For security reasons you can choose encrypted-installation. [Don't works with auto-login!!!]

For a dual-boot-system you maybe have to resize another partition to get free space!

QStudio64 will recognize your Linux/Windows/OSX-systems and all other partitions or free space,

and lead you through the install process.


Be sure to have min. >20 GB or more of free space (or an old partiton that can be deleted!).
QStudio64 will install ca. 17 GB of data on your harddisk!


Now you are ready to install QStudio64.



Swap-partition*:

A SWAPFILE will be used by default and there is nothing else to do. If you want to set up a SWAP-PARTITION you have to:

Choose 80- 110% the size of your physical RAM, e.g. if you have 4 GB RAM, choose 3,8 GB ore some more for the swap-file.

Create a Linux-Swap as filesystem with gparted instead of ext4!

Create and format an ext4-partition with mountpoint: /

and start the install-process.


NOTE: If you use a swap-partition instead of the default /swapfile you should check and edit:

/etc/fstab and /etc/initramfs-tools/conf.d/resume for the right UUID of your swap in installed system. 

See more details in the swap-repair*-chapter!




Language, keyboard-layout and timezone:

Choose your right keyboard-layout and language, timezone and give user-name and password.

Wait until the install-process is done!


Reboot and start QStudio64. 



-----------
FIRST STEPS
-----------

..to configure QStudio64:

While Qstudio64 comes with a lot of pre-configured software,
you just have to do some easy steps to fine-tune your system:



1. Choose your language!

Qstudio64 comes in english by default, but there are many language packs
for german, french and spanish .. languages pre-installed!
All other language packs you can install over internet.

To change the language after install go to Control Center (Steuerzentrale) in your Start-Menu:

english: /System/Control Center/Languages
german: /System/Steuerzentrale/Sprachen


- choose/add your favourite language

- Apply your choosen language system-wide!


The preference of your keyboard-layout you are able to change in Control Center/Keyboard (Tastatur)!

- Restart the computer to apply your changes!


NOTE:
      To change the language permanent on a pure usb/sd-live-system, you have to burn QStudio64-Image
      on an Usb-Stick or bootable Sd-Card with a persistence-volume of min. 2GB to safe settings!

--->  After reboot the live-system comes in your choosen language and you are able to run updates.



2. Update your system

- with the mintupdate-launcher of your taskbar!

- in terminal directly: sudo apt update && sudo apt upgrade


Reboot your system!




3. Optimize your system


Add user to group audio:


sudo adduser yourusername audio




Choose your desired kernel with grub-customizer (optional)

-> (lowlatency-kernel is recommend!)



Check if real-time-priority is set for group audio:

Configure with editor as root: /etc/security/limits.conf 

@audio          -       rtprio          99
@audio          -       memlock         unlimited



-> at the end of the script!

- REBOOT THE SYSTEM!




4. Install drivers

Go to Driver Manager and check if there are some available driver for your connected hardware
that was not recognized and configured by system!

- REBOOT THE SYSTEM!



5. Configuring soundcards with ALSA/Jack

- use mate-mixer to control the volume of your onboard-chip!

- use Cadence to configure and control your soundcard(s) with Jack Audio Server (recommend for Ardour/Bitwig)

- use mudita24 if you use Envy24/IC1712-chipset-cards (e.g. M-Audio Delta-series)

- Note: a lot of usb-soundcards comes without a software-mixer! (Use hardware-controls or volume-button in software)

- choose your favourite soundcard in software! (eg.vlc-player/ardour/bitwig/mixxx,,)


-------------------------

ALSA Soundconfiguration
------------------------

QStudio64 (QS64) detects & configures mostly the (onboard) soundcard as default soundcard.
 
Sometimes the hdmi-output could be autoconfigured by ALSA as the default and if you have more than one soundinterface, you should select your desired default soundcard too!


Identify Sound Cards: 

Use the following commands:


List of kernel-modules:

cat /proc/asound/modules 
 0 snd_hda_intel
 1 snd_usb_audio



aplay -l 

to list all available sound cards and their corresponding device numbers. For example, the output might look like this:

**** List of PLAYBACK Hardware Devices ****
card 0: MyCard1 [My Sound Card 1], device 0: Device 0 [Device 0]
card 1: MyCard2 [My Sound Card 2], device 0: Device 0 [Device 0]



To select a default sound card in ALSA on QStudio64, you have many options:


1. Open alsamixer in terminal: 

alsamixer

Use the F6 key to select the desired sound card. Then, save the settings with 
sudo alsactl store


2. A fast and easy way to control multiple soundcards in QS64 is to use the JACK AUDIO SERVER,
choosing your desired soundinterface in Cadence under "Configure/Driver/ALSA", starting an ALSA-LOOP-JACK-Bridge 
to have sound in browsers over usb and to mark "Auto-start JACK or LADISH at login" to have JACK as an autostart service! (Recommend for professional daw usage!)
 

3. Also you can configure your default soundcard just in ALSA with:

#Find your desired card:

cat /proc/asound/cards


#and then create /etc/asound.conf with the following entries:

defaults.pcm.card 1
defaults.ctl.card 1

#Replace 1 with number of your card determined above. 

Source: https://www.alsa-project.org/wiki/Setting_the_default_device



USB-soundinterface On/Off-"Button"-script:
-----------------------------------------

If you have configured asound.conf and choosed (for example) card "2" for your usb-interface
you can execute an own written bash-script as On/Off-button or just using the renaming commands!

Create 2 files without ending und give the entry:


This renames and deactivates asound.conf and brings the usb-soundinterface back as default:
 
#!/bin/bash
sudo mv /etc/asound.conf /etc/asoundOFF.conf


This renames and activates asound.conf and brings onboardsound back as default:

#!/bin/bash
sudo mv /etc/asoundOFF.conf /etc/asound.conf

Save and make them executable, start with terminal!


You can also just use the single mv commands in terminal to activate/deactivate your configured usb-interface as default soundcard!!

---

Advanced config example:

Playback on your build in sondcard and capture (microphone) from external USB device.

Your external device is listed as card 2: device 0 and your build in soundcard as card 0: device 0

your asound.conf should look something like this:


pcm.!default
{
  playback.pcm
  {
    type hw
    card 0
    device 0
  }


Other method:

 
4. Change priority:


Edit /etc/modprobe.d/alsa-base.conf:

Open the file with a text editor as root:

sudo nano /etc/modprobe.d/alsa-base.conf

Add the following lines to specify the index for your preferred sound card:


options snd-usb-audio index=-2
options snd-hda-intel index=0


Replace snd-usb-audio and snd-hda-intel with the appropriate driver for your sound card. 
The index values -2 and 0 are used to set the priority of the sound cards.

example:

options snd-usb-audio index=0
options snd-hda-intel index=1

-> is setting the usb-soundinterface as default soundcard!

Save settings and reboot!



Other way:

6. Edit Configuration Files: Modify the /etc/asound.conf or ~/.asoundrc file to specify the default sound card. 
For example, to set the default sound card to card 1, you can add the following lines to the configuration file:


pcm.!default {
    type hw
    card 1
}
ctl.!default {
    type hw
    card 1
}


Kernel Module Options: Adjust the kernel module options to disable or enable specific sound cards. For instance, to disable the second card operated by a module, you can add the following to /etc/modprobe.d/alsa-base.conf:
options module_name enable=1,0

Use alsactl: Save the current ALSA settings with alsactl store and restore them on boot. This ensures that your preferred sound card settings persist across reboots.

Blacklisting Modules: If you want to disable a specific sound card, you can blacklist its kernel module by adding a line to /etc/modprobe.d/blacklist.conf. For example, to disable the second sound card, you might add:

blacklist snd_hda_intel


Check Device Files: Identify processes using sound device files with 

fuser --all --verbose /dev/snd/* 

and stop them before reloading ALSA driver configuration.


These methods should help you configure ALSA to use your preferred sound card.



!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
For JACK use you can configure your default soundcard in Cadence gui under (ALSA) settings!
!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!


More infos: 

https://kx.studio/Documentation:Manual:alsa_and_kxstudio

https://www.alsa-project.org/main/index.php/Asoundrc

https://search.brave.com/search?q=soundcard+alsa+selector+




CADENCE (JACK)
--------------

Cadence is THE tool to configure and control the Jack-Server for professional audio:

Configure your soundcard(s) right in cadence and choose your favourite soundcard (Alsa)!

more: https://kx.studio/Documentation:Manual:cadence_introduction

      https://kx.studio/Documentation:Manual:jack_configuration


There are some recommend configuration-settings and bridge-modes with cadence:

- start a (Alsa>Loop>Jack)-bridge to hear sound from e.g. Browser through Jack
on an external soundcard!

(Don't forget to stop the bridge and put the settings on "None"-bridge and restart Jack
to get normal sound over ALSA again!)




HEAR NO SOUND?
--------------

- Check in terminal if your soundcard is loaded by linux-kernel:

    cat /proc/asound/cards

- Check if some mixer-channel is muted! (alsamixer)

- Check if Cadence is configured right!

- Choose your favourite soundcard in software


NOTE: Some chipsets defines the hdmi-channel as main-output! So if you HEAR NO SOUND in QStudio64
you have just to check and configure your alsa-base.conf (Step 5)!

To make your usb-soundcard as the default soundinterface follow Step 5 too!


It s also recommend to DISABLE THE STANDBY OR SUSPEND-MODUS in energy-settings (Control-Center)!



-----------------------------------------------------------------------

 To run an ICECAST-webradio-server go to manuals in home/README/Tweaks.

-----------------------------------------------------------------------

------------------------------------------------------------------
Bluetooth in QStudio64 (for ALSA-based systems without pulseaudio)
------------------------------------------------------------------

#Install bluez-alsa-utils

sudo apt install bluez-alsa-utils libasound2-plugin-bluez

Connect, Pair and trust with the blueman-applet in taskbar!
Notice the MAC-Adress of your bluetooth devicde!

Create a hidden file .asoundrc in /home with the content:

defaults.bluealsa.service "org.bluealsa"
defaults.bluealsa.device "XX:XX:XX:XX:XX:XX"
defaults.bluealsa.profile "a2dp"
defaults.bluealsa.delay 10000

and fill in the mac-adress of your bluetooth device!


Choose "bluealsa -Bluetooth Audio Hub" as audiodevice
and "bluealsa" as mixer in player (e.g. vlc, audacious)

Enjoy the sound! :)

-> After using bluetooth you have to delete (or rename) .asoundrc to get audio working!*

-> IF you face problems to connect or error-messages just reboot the system
and try again!

It works!!!



-------------------------------
*Bluetooth On/Off-Button-Script 
-------------------------------

Here is a little workaround to create two On/Off-"Button"-script-files to start or end the bluez-alsa
connection with .asoundrc (after you configured and tested it succesfully):

Just create 2 files with:


#!/bin/bash
cd /home/YOURUSERNAME/
mv .asoundrcOFF .asoundrc


->this script is to start bluetooth asoundrc!

and in another file:


#!/bin/bash
cd /home/YOURUSERNAME/
mv .asoundrc .asoundrcOFF


-> this script is to rename .asoundrc and deactivate it!

(-> replace YOURUSERNAME with your given username)


You can give titles like "BT-ON" "BT-OFF" and own buttonicons. ;)


-> Be sure to make the files executable!

-> Execute in terminal to start and stop bt-audio

-> ATTENTION: If .asoundrc is not deleted/disabled 
   after bluetooth-session you will hear no sound!



more infos:

https://github.com/arkq/bluez-alsa

https://github.com/arkq/bluez-alsa/wiki


To get bluetooth really fast working (re-)install Pulseaudio:

sudo apt-get install pulseaudio libcanberra-pulse pulseaudio-module-bluetooth pulseaudio-module-jack 


NOTE: While installing pulseaudio you reset to Linux Mint default sound settings! (NOT recommended!)
                          



SOUNDINTERFACES
---------------

a lot of actual and Class A-soundinterfaces (like the Focusrite Scarlett-series,..) are supported plug n play in QStudio64. A list of some interfaces is shown here: http://www.alsa-project.org/main/index.php/Matrix:Main
but also there are some cards and usb-interfaces with supported chipset NOT listed (e.g. Presonus Audiobox USB) but work fine out of the box!

Tip: Most class-compliant-interfaces do so.

So try if your interface is supported or buy some interface that is known supported!


TO GET THE BEST SOUND WITH MINIMUM LATENCY AND LESS SOUND-ISSUES IT'S RECOMMEND TO MAKE THE JACKAUDIO-SERVER WITH CADENCE AN AUTO-LOGIN-SERVICE! 
s. http://kxstudio.linuxaudio.org/Documentation:Manual:cadence_introduction

http://kxstudio.linuxaudio.org/Documentation:Manual:jack_configuration

Cadence and Jack is for Linux like the ASIO-Driver for Windows and is more recommend for Linux Audio Systems than Pulseaudio, because of more stability with synths, plugins and lowlatency-kernel and of course because its flexibility, less latency (which is important for playing midi-instruments and synth-plugins live),routing-options and high definition-soundquality!

NOTE: If you want/need pulseaudio instead of Alsa/Jack you have to install it back with synaptic/terminal.


For more informations, tricks and tips about Linux Audio and how to use (soundcards, apps, e.g.) read these manuals:

http://kxstudio.linuxaudio.org/Documentation:Manual:linux_audio_overview

http://kxstudio.linuxaudio.org/Documentation:Manual:alsa_and_kxstudio

http://kxstudio.linuxaudio.org/Documentation:Manual:cadence_introduction

Libre Music (Linux Audio Website): http://libremusicproduction.com/

Linux-Audio-Forum: https://linuxmusicians.com/





BITWIG Studio/8track/Demo
------------------------- 

Qstudio64 21.1 contains Bitwig Studio*.


--> It's recommended to use always the latest version from bitwig.com!

<A CPU which supports the SSE 4.1 instruction set is required!>



REGISTRATION
------------

NOTE: Create an acount on bitwig.com and registrate with your licence-key! Download and install the latest version!

Start the program and activate the licence. Now you have the full 8-track OR bitwig studio-version ready to work!


--> If you don't have a licence-key you can try Bitwig Studio in DEMO-MODE with saving/export-options disabled.


PROMO
-----

Write us an email to lmaudio@subvertising.org and maybe get one of 100 Bitwig Studio 8-Tracks licences ;)


Audio-Settings
--------------

-> Choose ALSA or JACK-Audiodriver!

To use JACK you have to configure your soundcards with Cadence (ALSA-Driver) before you start the soundserver!


!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

Big thanx to Placidus and the Bitwig-Team!



MIXXX 
-----

TROUBLESHOOT: Mixxx freezes, crashes, or otherwise misbehaves with some nVidia graphics cards:

Before you try anything else, please update or reinstall your nVidia graphics driver. (This applies to all OSes.) 
Even if it is the same exact version, apparently it is fickle and needs to be rebuilt/reinstalled any time things change in the OS. 
Try this first before going any further.
!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
Mostly the actual nonfree-nVidia-driver has to be installed via driver-manager! 
!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

If you have staying issues try uninstalling the proprietary nVidia driver and using the free nouveau driver.

more informations: http://mixxx.org/wiki/doku.php/troubleshooting



--------------------------------------
Graphic-card-issues (nVidia-chipsets):
--------------------------------------
!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
The actual nonfree-nVidia-driver is recommend to fix issues with nvidia-chipsets! Install with driver-manager! 
!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

-> To go back to the opensource nouveau-driver you have to remove and clean the propietary nvidia-driver:

sudo apt purge nvidia*

sudo reboot

Read the official Linux Mint Release Notes for more informations: https://linuxmint.com/rel_tessa_mate.php



---------------------
KXStudio-Repositories
---------------------

NOTE: The packages file link might change at anytime, and so the instructions themselves.
Check: https://kx.studio/Repositories for actual KXStudio-Repositories please!



Different Desktop-Environments
------------------------------
QStudio64 comes with great and lightweight MATE-desktop.
It's designed to configure your desktop individual in every detail!

If you want to change your DE you have to install the Cinnamon,
KDE or XFCE-meta with softwarecenter or Synaptic packetmanager!

-> Be sure to disable “autologin” & “Remember last user” in MDM
-> Restart computer!
-> Login with your favourite DE-session

It’s recommend to decide for one desktop-environment and NOT to switch!

(-> QStudio64 was made with&for MATE DE! Do it by your own risk!)



Language (bug 173-sx-03)
------------------------

QStudio64 just saves your choosen language of the beginning maybe as system default!

If you change the language after install again, you maybe will find your old keyboard-layout in mdm-login!

Attention: If you used difficult passwords with special signs you maybe can't login again 
(or you just have to know where to find the right letters on new keyboard)!

To fix this, just open as root: /etc/default/keyboard

and change your default tastatur-layout:


XKBLAYOUT="de"
XKBVARIANT=""


Write your favourite language like "en" "fr" "es" "us".. !


Use CTRL-ALT-F1 and login with your username and password.

Type: setupcon

After reboot your new language-keyboard-layout works in mdm-login (and terminal boot) too.


To check the keyboard-layout you can type in terminal:

cat /etc/default/keyboard


Note: This just happens if you change your systems language after install!

If you choosed your right language and keyboard-layout during the install-process,
everything will work fine and you just have to follow STEP 1 from FIRST STEPS to
apply your choosen language system-wide!


more informations about this bug: 

http://www.linuxmintusers.de/index.php?topic=19927.0

http://unix.stackexchange.com/questions/136382/mint-login-screen-wrong-keyboard-layout

http://www.linuxmintusers.de/index.php?topic=26683.msg425917#msg425917




Grub-Menu:
----------

If you wanna hide grub-menu at boot, modify grub in /etc/default:

    GRUB_DEFAULT=0
    GRUB_HIDDEN_TIMEOUT=5
    GRUB_HIDDEN_TIMEOUT_QUIET=true
    GRUB_TIMEOUT=0
    GRUB_DISTRIBUTOR=`lsb_release -i -s 2> /dev/null || echo Debian`
    GRUB_CMDLINE_LINUX_DEFAULT=“quiet splash”
    GRUB_CMDLINE_LINUX=“”
    
    # Set this if you hide grubmenu at boot! hidden-timeout has to be 0-10
    # NOT recommend with dual-boot systems
    # Type ESC/ENTER at boot to make grub-menu visible again! 
    # in this case hidden-timeout has to be 3-10
    GRUB_DISABLE_OS_PROBER=true

write in terminal: sudo update-grub 
to apply changes!

....................................................................




Login-Manager
-------------

Write your username to get login without password!

NOTE: Replace STUDIO under USER with your username. 




BROWSERS
--------

Qstudio64 comes with one of the fastest and most secure Web-Browser:


BRAVE

It includes an advanced privacy and security-orientated preset

NOTE: -> After password changes you have to enter the last password before change 
in the passphrase-prompt for keyring if you start the Brave Web Browser first time!



FIREFOX52* 
---------

Since Firefox 52 there is the hard-dependency with Pulseaudio to have sound:

https://bugzilla.mozilla.org/show_bug.cgi?id=1247056

https://bugzilla.mozilla.org/show_bug.cgi?id=1345661

https://ubuntuforums.org/showthread.php?t=2355092


QStudio64 was primary build for stable and latency-free multimedia-productions
basing on ALSA and Jack as the default soundsystem without Pulseaudio:

http://kxstudio.linuxaudio.org/Documentation:Manual:linux_audio_overview

“For serious audio work, it is better to avoid pulseaudio.
The main reason is because pulseaudio make no guaranty about the latency.
The latency of pulseaudio will increase in case of xruns, and the only possibility to decrease it, is to stop and restart pulseaudio.”

https://proaudio.tuxfamily.org/wiki/index.php?title=DAW_Digital_Audio_Workstation#PulseAudio


If you want Firefox/Tor-Browser&Chromium with sound, (re-)install Pulseaudio:

sudo apt-get install pulseaudio libcanberra-pulse pulseaudio-module-bluetooth pulseaudio-module-jack 

(NOT recommend if you want to use QS64 as an ALSA/JACK based Audio-Workstation!)


A good alternative for Firefox is the Palemoon-Project, which is working with ALSA-based Linux systems: 
https://www.palemoon.org/




Closed-source-browser:
----------------------

e.g.:

OPERA 

(Chrome-based)

download & install latest .deb from the opera-website:

https://www.opera.com/



VIVALDI 

(Chrome-based, Amazon&Netflix compatible)

https://vivaldi.com/

-> Download the 64bit-deb-file and install vivaldi!


Video-Support in Opera/Vivaldi:

Open vivaldi with terminal. Now you can read n`paste the code and download the missing codecs.

The file "libffmpeg.so" will be extracted in your vivaldi-folder in hidden-files of your home directory!
Copy it to /usr/share/opera to get video-support in opera too!


So there are many ways to browse the internet.

 



Keyrings Password-Reset:
------------------------

To reset the keyrings passphrase:

write in terminal:

rm /home/USER/.local/share/keyrings/login.keyring
rm /home/USER/.local/share/keyrings/user.keystore

(Write your given user-name instead of “USER”!)

Restart the computer!

Now the keyring got the same pw that you choosed for system.


-> After password changes you have to enter the last password before change 
in the passphrase-prompt for keyring if you start the Brave Web Browser first time!

If you don't know the old password you given you have to reset the keyrings!

(It's not a bug - it's about security! ;-)



--> Debugging APT-CACHE/Sources.lists 
-------------------------------------

If there is an error-message about "corrupted apt" in the Mintupdate
or problems with mirror-switching and sources.lists-lock..

write in terminal:


sudo apt-get clean

sudo apt-get check
 
sudo dpkg --configure -a

sudo apt-get -f install

sudo apt-get update && sudo apt-get dist-upgrade



If this don't work, type in terminal:

sudo rm -rf /var/lib/apt/lists/*
sudo mkdir /var/lib/apt/lists/partial 
sudo rm /var/cache/apt/*


sudo apt-get update && sudo apt-get upgrade


if you have always problems, type in terminal:

apt-cache policy | grep 700

cat /etc/apt/preferences.d/official-*


Reboot!




SWAP-Repair*
-----------

QStudio64 installer is detecting and using an existing SWAP-PARTITION.
If there is no SWAP-PARTITION it will create a SWAP-FILE in system.

If you use existing SWAP-PARTITION you have to create 
a resume-file with the UUID of your SWAP after install:

write in terminal:

swapon --show
#shows swap

df -h
#list all partitions

ls -l /dev/disk/by-uuid
#list of uuids l

echo 'RESUME=UUID=YOURUUIDNUMBER' | sudo tee -a /etc/initramfs-tools/conf.d/resume             

#replace YOURUUIDNUMBER with the UUID of SWAP


sudo update-grub

sudo update-initramfs -u -k all

Reboot

------------

This is about creating a new swap-partition after install with /swapfile:

Reboot with a linux-livesystem from an usb pendrive and start gparted!
Resize your partition and give minimum 2-8GB free space.
Create Swap of the empty space with gparted.

Reboot your installed system!

Terminal:

df -h
#list all partitions

sudo swapoff -a
#disable old swapfile

sudo rm -i /swapfile
#delete old swapfile


Start gparted and activate with SWAPON the Swap.

swapon --show
#shows swap

df -h
#list all partitions

ls -l /dev/disk/by-uuid
#list of uuids l

sudo swapon -U UUID-NUMBER-OF-YOUR-SWAP
#activates swap


Edit etc/fstab:

xed admin:///etc/fstab

delete old /swapfile entry if always there

write: UUID=UUID OF YOUR SWAP       sw              0       0

example:

# <file system> <mount point>   <type>  <options>       <dump>  <pass>
# / was on /dev/sda3 during installation
UUID=1462245-10fc-2349-b120-1f3e456028c6 /               ext4    errors=remount-ro 0       1
# /boot/efi was on /dev/sda2 during installation
UUID=0124-CB2F  /boot/efi       vfat    umask=0077      0       1
UUID=eac56982-b6e0-49652-a0c2-ac0d9b65784e3       sw              0       0                                     #SWAP in this example


Modify /etc/initramfs-tools/conf.d/resume as root with:

sudo cp /etc/initramfs-tools/conf.d/resume /etc/initramfs-tools/conf.d/resume.bak

echo 'RESUME=/swapfile' | sudo tee -a /etc/initramfs-tools/conf.d/resume

xed admin:///etc/initramfs-tools/conf.d/resume

write:
RESUME=/swapfile          #or RESUME=UUID=.....-> if you use a swap-partition instead a swapfile!

(-> Overwrite/Delete older swap-resume-entrys if exists!)

write in terminal:
sudo update-initramfs -u -k all

or

sudo update-initramfs -u

to refresh the initramfs.

That’s it! Exit the terminal.

Reboot!


Check in terminal if everything is right:
swapon -s






Initramfs
---------

If you find issues with initramfs like 'command not found' or problems while updating, 
you have to uninstall remastersys and all its dependencies with this commands:


sudo apt autopurge

sudo apt autoremove

sudo apt autoclean

sudo apt clean

sudo update-initramfs -u -k all





DNS
---

Run "resolvectl status" to see details about the uplink DNS servers currently in use.

To verify that DNS works, run these commands:

cat /etc/resolv.conf
ping google.com


If you find problems with DNS-resolving/internetconnection, write in terminal:

sudo rm /etc/resolv.conf

sudo ln -s /run/systemd/resolve/stub-resolv.conf /etc/resolv.conf 


if this do not works try:

sudo systemctl restart NetworkManager

and/or reboot!

try also:

sudo systemctl restart systemd-networkd

sudo systemctl restart systemd-resolved

#options: start restart stop enabled disabled




BACKUP
---------
It's recommend to use Timeshift and/or the Backup-Tool to safe stable configurations!

With remastersys you can create your own backup.iso-files for USB-pendrives.




Distro-Info
-----------

The Operation System-Info in Cadence is showing nothing?

To make the Distro-Info visible in some apps you have to 

write in terminal:

xed admin:///etc/lsb-release

give the entry at the end:

DISTRIB_DESCRIPTION="QStudio64-21.1-SX"

and save the file.

write in terminal:

sudo update-initramfs -u -k all

Reboot!



SNAP STORE
----------

Backdoor via APT
When Snap was introduced Canonical promised it would never replace APT. This promise was broken. 
Some APT packages in the Ubuntu repositories not only install snap as a dependency but also run snap commands 
as root without your knowledge or consent and connect your computer to the remote proprietary store operated by Canonical.

Disabled Snap Store in Linux Mint 20
Following the decision made by Canonical to replace parts of APT with Snap and have the Ubuntu Store install itself without users 
knowledge or consent, the Snap Store is forbidden to be installed by APT in Linux Mint 20.

Note

For more information read the announcements made in May 2020 and June 2019.

https://linuxmint-user-guide.readthedocs.io/en/latest/snap.html


How to install the Snap Store in Linux Mint 20
Recommended or not, if you want to use the Snap Store, re-enabling and installing it is very easy.

sudo cp /etc/apt/preferences.d/nosnap.pref /etc/apt/preferences.d/nosnap.pref.bak

sudo rm /etc/apt/preferences.d/nosnap.pref

apt update

apt install snapd


After UNINSTALL Snap (all packages) you have to: 

sudo cp /etc/apt/preferences.d/nosnap.pref.bak /etc/apt/preferences.d/nosnap.pref




RISEUP-VPN
----------

Snap Installation

sudo apt install snapd gnome-software-plugin-snap

Then, search for RiseupVPN in the Software Center or write in terminal:

sudo snap install --classic riseup-vpn


more informations: https://riseup.net/en/vpn




Linux Mint Upgrade (optional)
-----------------------------

QStudio64-21.1 gets updates until April 2027.

Optional you can upgrade to a higher version of Linux Mint: 
Since Linux Mint 19.x it is really easy to upgrade with the update-manager.
All apps and settings will be saved.
  

-> Backup all your personal data and/or make a snapshot with timeshift before!

Our focus is on stability and multimedia-production - do it on your own risk.

-> If you are not sure what to do and/or have no hardwaredriver-problems, 
it's recommend to stay with the solid Linux Mint 21.1 base.





KNOWN ISSUES AND UPDATED INFORMATIONS
-------------------------------------
...you will find in the updated RELEASE NOTES at our project-blog: http://qstudio64.tumblr.com

or on our new homepage: https://qstudio64.io (Big thanx to Ruffy <3 !)





Enjoy!

;-)


HAVE FUN- BE CREATIVE!
_______________________

c.h.a.l.e.e. 17/07/2025
_______________________
 
BIG THANX TO:

https://www.bitwig.com/

https://mixxx.org/

https://ardour.org/

https://kx.studio/

https://linuxmint.com



GIVE DONATIONS! :-)

-----------------------------------------------------------------------------

NO WARRANTYS! UNDER THE GPL 2/3.0./// FREE TO USE AND SHARE!*
_____________________________________________________________________________

                                                         Rev.beta11_2-Xi*
