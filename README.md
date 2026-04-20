<p align="center"><img src="./.idea/icon.png" alt="Logo" width="200"></p>
<h1 align="center">Sable - Android<br>
<div align="center">
   <a href="https://discord.gg/createaeronautics">
        <img alt="Discord" src="https://img.shields.io/discord/937435293294919690?style=flat&logo=discord&label=Discord&color=5865F2">
    </a>
    <a href="https://modrinth.com/mod/sable">
        <img src="https://img.shields.io/modrinth/dt/sable?logo=modrinth&amp;label=&amp;suffix=%20&amp;style=flat&amp;color=242629&amp;labelColor=5CA424&amp;logoColor=1C1C1C" alt="Modrinth Download"/>
    </a>
</div>
</h1>

# What

This is Create Simulated's -> <a href=https://github.com/ryanhcode/sable>Sable</a> engine, ported to android.

Which is required for Create Aeronautics physics to work.

## Create Aeronautics on Android!

<b>With this repo, now you can play Create Aeronautics on android!<br>(via any pajov based launcher)</b>

# How

Some Sable libraries require pc native (x86-x64) environment.

We build the android port from original sources with Android NDK to fill that blank (aarch64, android 24).

~Details bellow.~ (NOT READY)

# How can I..?

Play?

Sable from releases, anything else from their sources as usual.
- Get Android version of Sable from <a href="https://github.com/aksksklskdamkwkskskd-del/sable_android/releases/">releases</a> and Create, Create Aeronautics, etc. from their sources (eg. Modrinth).

- Use NeoForge as modloader.
> I didn't included Fabric externally, it doesn't have the main support directly in the ecosystem.
> If you want it, inform me about it and MIGHT add fabric releases too (already in plans but not soon).

- Tested on Amethyst Launcher (pajov fork, some late 2025 version) on Android 14.
- Using Java 21 seems fine.
- Mali (GPU) users may use Zink.
- You can inform me about issues _caused by the port_. 

#### Classic Mod Installing Steps

- Get your mods inside your launchers mods folder:
 - Use an file manager like Zarchiver and Shizuku (for accessing Android/data folder on newer android versions). You can find tutorials to setup correctly.
 - Go locate your game location (.minecraft) of your launcher.
Mostly under

> Android/data/[APP-PACKAGE-NAME]/files/.minecraft

or similar.
- Inside .minecraft, create 'mods' folder and put all your mods inside there.
- Go to your launcher and create 1.21.1 (-> current of April) NeoForge (-> use latest possible) profile.
- Launch your game.

- You may have some issues, here are basic regular ones:

## Some regular issues and fixes

### /flywheel backend flywheel:off

> [!IMPORTANT]
> Fixes invisible shafts and moving parts of the blocks. Caused by flywheel rendering, related to Create, as it's embedded.

# Plans List
- [x] Release building system.
- [x] First release (NeoForge)
- [ ] Automation (auto deploy release)
- [ ] Extra: Fabric support
- [ ] Extra: Main instructions besides android-build.yml

# Details about building it (this)

Auto build via "Sable Native Android Port" action (.github/android-build.yml). Building it on github servers as github action.

It builds both imgui to satisfy veil and satisfy + build Sable itself.

It just compiles imgui and Sable for android compatibility, puts all into each other to make the ultimate android port.

# ~Building (termux)~

Originally, I did it inside my termux environment, on the same day it came out. This repo has simpler version of that process. (With a lot of AI help ofc.)

Instructions not avaible for now. Its just the .github/android-build.yml but on termux and extra tricky.

> but planning to explain how i had it in the first place, termux version of instructions MIGHT be published here
> 
> (not an github professional here as you can see)
