# Greetings Traveller

So you came here to get information about linux or other stuff that might be useful to you? Well it _should_ be the right location.

Here I will try to cover a good starting portion of whats Important to know, what software might be worthwhile to look into and much more.

## Disclaimer

TODO

## Looking for something ?

Heres a short list of Anchors to quickly travel to your desired location.

-   [Greetings Traveller](#greetings-traveller)
    -   [Disclaimer](#disclaimer)
    -   [Looking for something ?](#looking-for-something-)
    -   [Distributions](#distributions)
    -   [How to Install](#how-to-install)
        -   [Bootable USB-Device](#bootable-usb-device)
        -   [Booting into Live-Mode](#booting-into-live-mode)
            -   [If you know your Motherboard Manufacturer](#if-you-know-your-motherboard-manufacturer)
            -   [If you do not know your Motherboard Manufacturer](#if-you-do-not-know-your-motherboard-manufacturer)
        -   [Installation](#installation)
            -   [**BACK UP YOUR DATA ON WINDOWS FIRST**](#back-up-your-data-on-windows-first)
            -   [Back in Live-Mode](#back-in-live-mode)
        -   [Useful Post-Installation Steps \[Linux Mint Focused\]](#useful-post-installation-steps-linux-mint-focused)
            -   [What are those things I mentioned above](#what-are-those-things-i-mentioned-above)
                -   [System Snapshots](#system-snapshots)
                -   [Driver Manager](#driver-manager)
                -   [Update Manager](#update-manager)
                -   [Firewall](#firewall)
    -   [Software](#software)
        -   [Software Manager \[Linux Mint\]](#software-manager-linux-mint)
        -   [Terminal](#terminal)
        -   [Installation through Website Visit](#installation-through-website-visit)
    -   [How do I troubleshoot things ?](#how-do-i-troubleshoot-things-)
    -   [Software List or replacement for other Software](#software-list-or-replacement-for-other-software)
        -   [Gaming](#gaming)
        -   [Artists](#artists)
        -   [Office Software](#office-software)
        -   [General purpose: Windows Applications on Linux](#general-purpose-windows-applications-on-linux)
        -   [General purpose: Searching for Software replacement](#general-purpose-searching-for-software-replacement)

## Distributions

As you might already know there isn't "the one" Linux. There are multiple Versions that exist which differs on the prebundled Software that exists for it.

So the thing you are more looking for at the start is "What are my needs?".

If you just want a System that is "plug and play", then look into "Distro for new Users" as those are the "Allrounder" with close to nothing you need to install yourself to make it just work.

My personal recommendation is [Linux Mint](https://www.linuxmint.com/)

It is the one I am using and it is the one which i assume you to use for the later points. Though I will cover stuff for other Distributions too.

If you are more into learning than a Daily Driver (Term: Using it for daily activities such as browsing, gaming, document editing, etc...), then you might want to look into more DIY Distros. One example would be [Arch Linux](https://archlinux.org/). It is the most well known Distro for it. There is also a big dedicated community around it with its own wiki called [ArchWiki](https://wiki.archlinux.org/).

There are of course a lot of other Distributions which are interesting to look at. Just take your time and look into them as your Usage may differ to mine.

But as a general Rule remember

**You can do everything on every Linux Distribution, just the Time required to setup may differ.**

## How to Install

So you found your Distribution which you want and downloaded the ISO file for it. Now what?

Here is a short list of steps that we will now do:

-   Install a Software to make a bootable USB-Device
-   Use given Software
-   Booting into the Live-Mode
-   Installing the Distribution

You will need the following things:

-   1x **Empty** USB-Flash-Drive with prefferably at least 8GB

It is **Important** that the USB-Flash-Drive is empty. To make it **Bootable** the Stick will be formatted which will **DELETE** everything on it.

So be sure to back the files up if there are any on it.

### Bootable USB-Device

The following two Softwares are the most commonly used ones to flash the ISO file to the usb drive.

[balenaEtcher](https://etcher.balena.io/) [rufus](https://rufus.ie/en/)

I recommend balenaEtcher as the interface is easier for beginners.

1. Select the Image file (ISO) of your Linux distribution.
2. Select the USB drive that you want to flash
3. Finally flash it.

After those steps you should have a Bootable USB drive.

Now safely remove the USB drive from your computer. If Windows asks to format the Drive click **NO**.

### Booting into Live-Mode

You have a bootable USB drive, what's next?

You will need to boot into the Live-Mode of the Distribution that you installed.

There are 2 ways to accomplish that and this depends on what your hardware is.

When your Computer makes a startup, there is often a logo screen wiith some text in the bottom row. You will have to Press the key in that screen.

Commonly used Keys for this may be:

`F1` `F12` `Delete`

-   Option 1: Boot Device Menu

Some motherboards have a dedicated Boot Device menu where you can select from which Drive to boot.

If that is your method, just select your USB drive and your good to go.

-   Option2 2: BIOS boot order

This one might be a bit more tricky to navigate if you are new to this but it is not as bad as it looks.

Here are the Steps

1. Find the "Boot" Settings
2. Find the Priority Order
3. Make the USB drive the highest priority
4. Save and Exit

As the BIOS is different for every Motherboard it sometimes isn't as straight forward to navigate

Here are some Tips that might help you

#### If you know your Motherboard Manufacturer

Search for the name of the manufacturer.

```
Example:
    MSI bios change boot order
Result:
    [How to change boot order? - msi.com](https://us.msi.com/support/technical_details/DT_Boot_Priority)
```

#### If you do not know your Motherboard Manufacturer

Search for your Device Model of the Computer/Laptop.

```
Example:
    Thinkpad x260 change boot order
Result:
    [Change Boot Order in Bios - lenovo.com](https://support.lenovo.com/us/en/videos/vid100791-how-to-change-boot-order-in-bios)

```

The results may not be as good as searching directly for the Manufacturer but usually you will find steps that should help you to find what you are looking for.

### Installation

So you made it this far... now the worst step of all, Installation.

Or is it?

If you have installed only Windows up until now you might feel annoyed as the Windows installation Process is time consuming and kind of privacy invasive (im talking about you, Microsoft accounts).

Linux on the other hand is simple and fast.

When you are in Live Mode and have decided you want to install the Operating System, the first step is

#### **BACK UP YOUR DATA ON WINDOWS FIRST**

Installing the Operating System will delete everything on your System if you do not make a "Dual Boot"

If you preffer to have both Operating Systems available by changing the Boot Device then look up how to Dual Boot it.

It is a bit more complex to set up, and sometimes having Windows on standby for whenever you need might be useful.

#### Back in Live-Mode

Double Click the "Install Linux [Instert Distribution Name]"

Then just follow the Installer and you are up and running.

Important things to look out:

-   If you don't know what you are doing: Install "Multimedia Codec's"
-   If you don't do a dual boot: Erase Disk and Install [Distro Name]
-   If you don't know what you are doing: Do not encrypt your Home drive

After following the installer you will shut down your Computer and pull out the USB Drive.

And then Boot the System up as usual.

If you did everything correct, you should now be in Linux Mint instead of Windows.

If something went wrong please write a message about what didn't work. I want this guide to be as easy, yet correct so that more people can be introduced to the easy world of Linux.

### Useful Post-Installation Steps [Linux Mint Focused]

So when you boot into the System there should come a "Welcome Screen" if you have chosen to use Linux Mint.

You should go through every Menu there as it is quite useful.

Heres a non finished list of things I personally recommend (Read further down for more specific information):

-   Setup System Snapshots
-   Driver Manager
-   Update Manager
-   System Settings
-   Firewall

#### What are those things I mentioned above

##### System Snapshots

This is a feature which will save your System Settings. If you break something this will help you restore your System to a previous State where it is not broken.

##### Driver Manager

Driver are Software that allows the Computer to interact with the Hardware. Usually almost all common devices are supported out of the box, but there may be exceptions to that.

One of those is NVIDIA Graphics Cards.

The Driver Manager will give you the ption of choosing Multiple drivers.

As of right now the Proprietary Drivers of NVIDIA are the recommended ones. And thus should be used.

This might change at one point in the future. If you are not [FOSS(Free and Open Source Software)](https://itsfoss.com/what-is-foss/) focused, taking the proprietary ones is not an issue.

Performance not good enough with NVIDA? Look under at the Gaming category.

##### Update Manager

Well that's the thing where you will Download updates. If you see a Shield in the Bottom right List with an Orage Dot, it means there are Updates.

Updating in Linux only rarely Requires a Reboot. Just do them when you see them. If there is one that Requires a reboot, well it is not Windows, it will just wait until you decide to Reboot.

##### Firewall

Now this one might sound scary, but don't worry.

All you do is activate the Slider right of the "Status" text. That just activates the Firewall.

## Software

Now that you completed an install of Linux and made basic configurations to your system, you of course want to install Software.

And there are quite a few ways of installing Software. But it is **a lot** safer than Windows

### Software Manager [Linux Mint]

The easiest way of installing is through the Software Manager. It is kind of like the Google Play Store just that it really isn't a Store, everything there is Free and Safe to download.

You can either Install things as System Package, or as Flatpak.

I personally recommend Flatpak as a lot of the software has more recent versions in the Flatpak format but it is more Space hungry than a System Package.

### Terminal

The all time classic. While everything can be done with the Terminal, on "Beginner Friendly" Distributions, there are other ways of installing.

Still here are some information about it.

Depending on your Distribution you will have a different command for installing things.

```
apt
dnf
pacman
```

Even if you don't need them it is still good to familiarize yourself with them as sometimes this might be the only way of installation.

### Installation through Website Visit

You should always look at the Website to see how to install an Application. But the 2 Ways above should be your get go for the actuall installation. But sometimes the website may be the only way of installing and then you should check that you are installing from a trustworthy site.

## How do I troubleshoot things ?

Get into the mentality of searching specificly.

You will need to troubleshoot stuff at some point. It's the same on Windows as it is on Linux.

Here is a short list of finding out your problem:

1. What exactly is not working?
2. What distribution are you on?
3. Is it a System Package or a Flatpak?
4. Have I done everything correctly?

If what you are doing isn't working try to first search how to do it?

Generally the format follows like this:

`linux [insert distribution name here] problem short yet specific`

Let's say you have a Software that you want to start when the Computer boots. There is a option for "Start Application on Boot" which you activated and it doesn't work.

```
Distro Example:Linux Mint
Software Example: EasyEffect
Install Type: Flatpak
```

As Flatpak is a type of bundle which is often System unrelated you should first look for (Our example case):

`flatpak Easyeffect not launching on startup`

If the information doesnt help, you should then try to look if it is a Distribution Problem and search for

`Linux Mint Easyeffect not launching on startup`

Usually after those 2 most of the problems will be solved. But sometimes it just takes multiple tries of searching. Don't feel discouraged and try to take breaks during troubleshooting. It is quite a tideous journey.

I hope this short example has helped you for learning how to generally troubleshoot, feel free to submit more examples of journeys on how to trouble shoot things.

## Software List or replacement for other Software

Sadly at the current point not all Software is available on Linux as on Windows.

There are often Alternatives but those are sometimes not on par with the Software that is on Windows and it would require you to learn a new Software.

I will try to keep the list Updated and accept recommendations.

### Gaming

Of course you can just download Steam. Generally it is good to always check out if your games Work on Linux though most stuff without Anti-Cheat should just work.

A good site to check for this is [ProtonDB](https://www.protondb.com/)

Users accumulate their experience with games and have steps that might help you to make a game run.

But generally, if something doesnt launch after a few minutes, cancel the launch.

1. Right-Click the game
2. Select Properties
3. Go to Compatibility
4. Enable "Force the use of specific Steam Play compatibility tool"
5. Try to launch the Game again

If that doesn't work, you can try a Software called [Lutris](https://lutris.net/)

Lutris is a Software which uses Installscripts made by the Community to give you the highest probability of the game just Running when you press launch. You can also connect other Accounts to it like GOG or Steam though I personally haved tried those features yet.

### Artists

The Adobe Suite currently is nonexistant in Linux. There are replacements for it but they will be different.

Here is a small table of replacement possibilities

| Adobe Software | Replacement Options               |
| -------------- | --------------------------------- |
| Photoshop      | Krita, Gimp, Photopea             |
| Premiere Pro   | DaVinci Resolve, Kdenlive         |
| Illustrator    | Inkscape, Vectr, LibreOffice Draw |
| After Effect   | DaVinci Resole\*, Blender         |

DaVinci Resolve includes Blackmagic Fusion which is the After Effect Programm

If you are looking for other Software, you can use this as a copy paste for searching for your Software replacement

`linux [Name] replacement`

Generally you will find a good list of replacement.

### Office Software

Microsoft Office

You can try the Browser Version. If that doesnt work you can try to use Libre Office which often comes preinstalled on Systems.

### General purpose: Windows Applications on Linux

If that still isn't good enough you might want to Look into [Bottles](https://www.youtube.com/watch?v=q9fZpkBNKRc).

Bottles is a Software that can run Windows applications and it is in the Software Manager

A good introduction into Bottles is a Video from [Michael Horn - Linux Gaming For Beginners: Run Any Game on Steam Deck/PC](https://www.youtube.com/watch?v=q9fZpkBNKRc). While it is a video focused about gaming, it the steps should be the same for any Windows application.

### General purpose: Searching for Software replacement

If you are looking for other Software, you can use this as a copy paste for searching for your Software replacement

`linux [Name] replacement`

Generally you will find a good list of replacement.
