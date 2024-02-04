# Greetings Traveller

So you came here to get information about Linux or other stuff that might be useful to you? Well it _should_ be the right location.

Here I will try to cover a good starting portion of whats important to know, what software might be worthwhile to look into and much more.

# Disclaimer

There is no affiliation to any of the projects, software or distribution which were mentioned inside of this guide.

Everything is based on my personal experience and preference about the software mentioned.

# Looking for something ?

Heres a short list of anchors to quickly travel to your desired location.

- [Greetings Traveller](#greetings-traveller)
- [Disclaimer](#disclaimer)
- [Looking for something ?](#looking-for-something-)
- [Distributions](#distributions)
- [How to Install](#how-to-install)
  - [Bootable USB-Drive](#bootable-usb-drive)
  - [Booting into Live-Mode](#booting-into-live-mode)
    - [If you know your Motherboard Manufacturer](#if-you-know-your-motherboard-manufacturer)
    - [If you do not know your Motherboard Manufacturer](#if-you-do-not-know-your-motherboard-manufacturer)
  - [Installation \[Linux Mint Example\]](#installation-linux-mint-example)
    - [**BACK UP YOUR DATA ON WINDOWS FIRST**](#back-up-your-data-on-windows-first)
    - [Back in Live-Mode](#back-in-live-mode)
  - [Useful Post-Installation Steps \[Linux Mint Focused\]](#useful-post-installation-steps-linux-mint-focused)
    - [What are those things I mentioned above?](#what-are-those-things-i-mentioned-above)
      - [System Snapshots](#system-snapshots)
      - [Driver Manager](#driver-manager)
      - [Update Manager](#update-manager)
      - [Firewall](#firewall)
  - [Further Customization](#further-customization)
- [Software](#software)
  - [Software Manager \[Linux Mint\]](#software-manager-linux-mint)
  - [Terminal](#terminal)
  - [Installation through Website Visit](#installation-through-website-visit)
- [How do I troubleshoot things ?](#how-do-i-troubleshoot-things-)
- [Software List or Replacement for other Software](#software-list-or-replacement-for-other-software)
  - [Gaming](#gaming)
    - [Steam](#steam)
    - [Epic Games Launcher, GOG \& Prime Gaming](#epic-games-launcher-gog--prime-gaming)
    - [Check game compatibility](#check-game-compatibility)
    - [Lutris](#lutris)
    - [NVIDIA Settings](#nvidia-settings)
  - [Adobe Suite](#adobe-suite)
  - [Microsoft Office Suite](#microsoft-office-suite)
  - [Audio Equalizer](#audio-equalizer)
- [General purpose:](#general-purpose)
  - [Windows Applications on Linux](#windows-applications-on-linux)
  - [Searching for Software replacement](#searching-for-software-replacement)
  - [Issues](#issues)
    - [Desktop Applications suddenly lagging](#desktop-applications-suddenly-lagging)

# Distributions

As you might already know there isn't _the one_ Linux. There are multiple versions that exist which differs around the prebundled software that exists for it.

So the thing you are more looking for at the start is: **_What are my needs?_**

If you just want a system that is _plug and play_, then look into "Distro for new Users" as those are the **allrounder** with close to nothing you need to install yourself to make it just work.

My **personal recommendation** is [Linux Mint](https://www.linuxmint.com/)

It is the one I am using and it is the one which I assume you to use for the instructions down below. Though I will try to cover stuff for other distributions too.

If you are more into learning than a daily driver, then you might want to look into more DIY distros. One example would be [Arch Linux](https://archlinux.org/). It is the most well known distribution as it expects you to know what you are doing. There is also a big dedicated community around it with it's own wiki called [ArchWiki](https://wiki.archlinux.org/).

There are of course a lot of other distributions which are interesting to look at. Just take your time and look into them as your usage may differ to mine.

But as a general rule remember

**You can do everything on every Linux distribution, just the time required to setup may differ.**

Tip: If you are unsure about what you want, then i recommend to test the distributions inside a Virtual Machine.

# How to Install

So you found your distribution which you want and downloaded the ISO file for it.

_Now what?_

In this section we will go over the following steps:

-   Install a Software to make a bootable USB-Device
-   Use given Software
-   Booting into the Live-Mode
-   Installing the Distribution

You will need the following things:

-   1x **Empty** USB-Flash-Drive with prefferably at least 8GB

It is **important** that the USB-Drive is empty. To make it **bootable** the USB-Drive will be formatted which will **DELETE EVERYTHING** on it. So be sure to back the files up if there are any on it. You can later format the USB-Drive again and then continue to use it normally.

## Bootable USB-Drive

The following two softwares are well known for flashing the ISO file to a USB-Drive.

-   [balenaEtcher](https://etcher.balena.io/)
-   [rufus](https://rufus.ie/en/)

I recommend balenaEtcher as the interface is easier for beginners.

1. Select the Image file (ISO) of your Linux distribution.
2. Select the USB-Drive that you want to flash
3. Finally flash it.

After those steps you should have a bootable USB-Drive.

Now safely remove the USB-Drive from your computer. If Windows asks to format the drive click **NO**.

## Booting into Live-Mode

You have a bootable USB-Drive.

_What's next?_

You will need to boot into the Live-Mode of the distribution that you flashed. There are 2 ways to accomplish that and this depends on what your hardware is. When your computer boots, there is often a logo screen with some text at the bottom. You will have to press the key in that screen.

Commonly used keys for this may be:

`F1` `F12` `Delete`

-   Option 1: Boot Device Menu

Some motherboards have a dedicated "Boot-Device-Menu" where you can select which drive to boot from.

If that is your method, just select your USB-Drive and your good to go.

-   Option 2: BIOS Boot Order

This one might be a bit more tricky to navigate if you are new to this but it is not as bad as it looks.

Here are the Steps:

1. Find the "Boot" Settings
2. Find the Priority Order
3. Make the USB-Drive the highest priority
4. Save and Exit

As the BIOS is different for every motherboard it sometimes isn't as straight forward to navigate

Here are some tips that might help you

### If you know your Motherboard Manufacturer

Search for the name of the manufacturer.

```
Example:
    MSI bios change boot order
Result:
    [How to change boot order? - msi.com](https://us.msi.com/support/technical_details/DT_Boot_Priority)
```

### If you do not know your Motherboard Manufacturer

Search for your device model.

```
Example:
    Thinkpad x260 change boot order
Result:
    [Change Boot Order in Bios - lenovo.com](https://support.lenovo.com/us/en/videos/vid100791-how-to-change-boot-order-in-bios)

```

The results may not be as good as searching directly for the manufacturer but usually you will find steps that should help you to find what you are looking for.

## Installation [Linux Mint Example]

So you made it this far... now the worst step of all, installation.

_Or is it?_

If you have installed only Windows up until now, you might feel reluctant as the Windows installation process is time consuming and kind of privacy invasive (I'm talking about you, Microsoft accounts).

Linux on the other hand is simple and fast.

When you are in Live-Mode and have decided you want to install the Operating System, the first step is:

### **BACK UP YOUR DATA ON WINDOWS FIRST**

Installing the Operating System will delete everything on your system if you do not make a "dual boot".

If you preffer to have both Operating Systems available by changing the boot device then look up how to dual boot it. It is a bit more complex to set up, but sometimes having Windows on standby for whenever you need might be useful.

### Back in Live-Mode

Double click "Install Linux Mint".

Then just follow the Installer and you are up and running.

Important things to look out:

-   If you don't know what you are doing: Install "Multimedia Codec's"
-   If you don't do a dual boot: Erase Disk and Install Mint
-   If you don't know what you are doing: Do not encrypt anything

After following the installer you will shutdown your system and pull out the USB-Drive. On Linux mint there will be a screen that tells you to pull out the USB-Drive. And then boot the system up as usual.

If you did everything correct, you should now be in Linux Mint instead of Windows.

If something went wrong, please start a discussion about what didn't work. I want this guide to be as easy yet correct so that more people can be introduced to the beautiful World of Linux.

## Useful Post-Installation Steps [Linux Mint Focused]

So when you boot into the System there should come a "Welcome Screen" if you have chosen to use Linux Mint.

You should go through every Menu there as it is quite useful.

Heres a non finished list of things I personally recommend (Read further down for more specific information):

-   Setup System Snapshots
-   Driver Manager
-   Update Manager
-   System Settings
-   Firewall

### What are those things I mentioned above?

#### System Snapshots

This is a feature which will save your system settings. If you break something this will help you restore your system to a previous state where it is not broken.

#### Driver Manager

Driver are software that allows the computer to interact with the hardware. Usually almost all common devices are supported out of the box, but there may be exceptions to that.

One of those is NVIDIA graphics cards. The Driver Manager will give you the option of choosing multiple drivers. As of right now the proprietary drivers of NVIDIA are the recommended ones. And thus should be used. This might change at one point in the future. If you are not [FOSS(Free and Open Source Software)](https://itsfoss.com/what-is-foss/) focused, taking the proprietary ones is not an issue.

Performance not good enough with NVIDA? [Click here](#nvidia-settings)

#### Update Manager

Well that's the thing where you will download updates. If you see a shield in the bottom right list next to the time with an orange dot, it means there are updates.

Updating in Linux only rarely requires a reboot. Just do them when you see them. If there is one that requires a reboot, well it is not Windows, it will just wait until you decide to reboot.

#### Firewall

Now this one might sound scary, but don't worry. All you do is activate the slider right of the "Status" text. That just activates the firewall.

## Further Customization

Finding out the name of some things to customize can be quite difficult. So here is a short list of names of components and what they are.

| Name       | Description                                                                           |
| ---------- | ------------------------------------------------------------------------------------- |
| Actions    | It is the Linux equivalent of the Windows Context Menu (right-click window actions)   |
| Applets    | Used to customize the panel (equivalent of Windows Taskbar)                           |
| Desklets   | The mini applications that were often seen on Windows 7 Desktops like clocks or notes |
| Extensions | General Desktop Extensions. Includes Window effects, Panel transparancy and much more |

# Software

Now that you completed an install of Linux and made basic configurations to your system, you of course want to install software.

And there are quite a few ways of installing software. But it is **a lot** safer than Windows.

## Software Manager [Linux Mint]

The easiest way of installing is through the Software Manager. It is kind of like the Google Play Store just that it really isn't a store, everything there is free and safe to download as they are rigorously maintained (though obviously you should not install anything that you don't know).

You can either install things as **System Package**, or as **Flatpak**.

I personally recommend Flatpak as a lot of the Software has more recent versions in the Flatpak format but it is more Space hungry than a System Package.

But going into details would be to big for this guide.

## Terminal

The all time classic. While everything can be done with the terminal, on "Beginner Friendly" distributions, there are other ways of installing.

Still here are some information about it.

Depending on your distribution you will have a different command for installing things.

`apt` `dnf` `pacman`

Even if you don't need them it is still good to familiarize yourself with them as sometimes this might be the only way of installation.

## Installation through Website Visit

You should always look at the website to see how to install an application. But the 2 ways above should be your get go for the actual installation. But sometimes the website may be the only way of installing and then you should check that you are installing from a **trustworthy site**.

# How do I troubleshoot things ?

Get into the mentality of searching specificly.

You will need to troubleshoot stuff at some point. It's the same on Windows as it is on Linux.

Here is a simple list of finding out most of your your problems:

1. Do i have an **Error Message**?
2. What exactly is not working?
3. What distribution are you on?
4. Is it a "System Package" or a "Flatpak"?
5. Have I done everything correctly?

If what you are unsure about if you did something correctly try to first search how to do it?

If you get an error message, perfect. Most likely people have had this issue too, so search about it.

If there is no error message or you didn't do something wrong then follow the general format. It looks like this:

`linux [insert distribution name OR the install type] [problem short yet specific]`

Let's say you have a software that you want to start when the computer boots. There is a option for "Start Application on Boot" which you activated and it doesn't work.

```
Distro Example:Linux Mint
Software Example: EasyEffect
Install Type: Flatpak
```

As flatpak is a type of bundle which is often system unrelated you should first look for (our example case):

`flatpak easyeffect not launching on startup`

If the information doesnt help, you should then try to look if it is a distribution problem and search for:

`Linux Mint Easyeffect not launching on startup`

Usually after those 2 most of the problems will be solved. But sometimes it just takes multiple tries of searching. **Don't feel discouraged** and try to take breaks during troubleshooting. It is quite a tideous journey sometimes.

I hope this short example has helped you for learning how to generally troubleshoot, feel free to submit more examples or improvements on how to trouble shoot things.

# Software List or Replacement for other Software

Sadly at the current point not all software is available on Linux as it is on Windows.

There are often alternatives but those are sometimes not on par with the software that is on Windows and it would require you to learn a new Software.

I will try to keep the list updated and accept recommendations.

## Gaming

### Steam

Of course you can just download Steam. Generally it is good to always check out if your games work on Linux though most stuff without Anti-Cheat should just work.

### Epic Games Launcher, GOG & Prime Gaming

There is a neat FOSS application that combines all three programs into one.

[Heroic Games Launcher](https://heroicgameslauncher.com/) let's you access the stores of all 3 applications, install and launch the games, shows Proton and Steamdeck compatibility tier per game and more. It is also a lot faster than the Epic Games Launcher.

If you play games through Epic Games it is a good alternative as the Epic Games Launcher doesn't exist for Linux.

### Check game compatibility

A good site to check for this is [ProtonDB](https://www.protondb.com/)

Users accumulate their experience with games and have steps that might help you to make a game run.

But generally, if something doesnt launch after a few minutes, cancel the launch.

1. Right-Click the game
2. Select properties
3. Go to compatibility
4. Enable "Force the use of specific Steam Play compatibility tool"
5. Try to launch the game again

If that doesn't work, you can try a software called Lutris.

### Lutris

[Lutris](https://lutris.net/) is a software which uses installscripts made by the community to give you the highest probability of the game just running when you press launch. You can also connect other accounts to it like GOG or Steam though I personally haved tried those features yet.

### NVIDIA Settings

If you have NVIDIA drivers installed, open "NVIDIA X Server Settings"

1. Click on "X Server Display Configuration"
2. Press the advanced button
3. Enable "Force Composition of Pipeline"
4. Enable "Force Full Composition of Pipeline"

## Adobe Suite

The Adobe Suite currently is nonexistant in Linux. There are replacements for it but they will be different.

Here is a small table of replacement possibilities:

| Adobe Software | Replacement Options               |
| -------------- | --------------------------------- |
| Photoshop      | Krita, Gimp, Photopea             |
| Premiere Pro   | DaVinci Resolve, Kdenlive         |
| Illustrator    | Inkscape, Vectr, LibreOffice Draw |
| After Effect   | DaVinci Resole, Blender           |

*DaVinci Resolve includes Blackmagic Fusion which is the After Effect Programm.

If you are looking for other software, you can use this as a copy paste for searching for your software replacement:

`linux [Name] replacement`

Generally you will find a good list of replacement.

## Microsoft Office Suite

You can try the browser version. If that doesn't work you can try to use Libre Office which often comes preinstalled on systems.

If not try the "General Purpose" section to install Windows applications on Linux.

## Audio Equalizer

Find out which audio server you are running by executing this command in the terminal

`pactl info | grep "Server Name"`

First of all no matter which program you use, **use the flatpak version** if you are on Linux Mint. The System Packages are outdated.

If you are using **PulseAudio** then use PulseEffects. Though it is recommended to upgrade to Pipewire as PulseEffects development stopped because the developers swapped from PulseAudio to Pipewire and now develop EasyEffects.

For Pipewire **(Yes that includes if it says `PulseAudio (on PipeWire 0.X.XX)`)** you should use EasyEffects.

# General purpose:

## Windows Applications on Linux

If the Linux alternatives still aren't good enough, you might want to look into [Bottles](https://usebottles.com/).

Bottles is a software that can run Windows applications and it is available inside the Software Manager(Linux Mint)

A good introduction into Bottles is a video from [Michael Horn - Linux Gaming For Beginners: Run Any Game on Steam Deck/PC](https://www.youtube.com/watch?v=q9fZpkBNKRc). While it is a video focused about gaming, it the steps should be the same for any Windows application.

## Searching for Software replacement

If you are looking for other software, you can use this as a copy paste for searching for your software replacement.

`linux [software name] replacement`

Generally you will find a list of replacement.

## Issues

### Desktop Applications suddenly lagging

Disable Discord hardware acceleration.

Linux Mint: Switch themes back to non 3rd party themes.
