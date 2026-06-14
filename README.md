<p align="center"><img src="./.idea/icon.png" alt="Logo" width="200"></p>
<h1 align="center">Sable - Android<br>
<div align="center">
   <a href="https://discord.gg/createaeronautics">
        <img alt="Discord" src="https://img.shields.io/discord/937435293294919690?style=flat&logo=discord&label=Discord&color=5865F2">
    </a>
    <a href="https://modrinth.com/mod/sable">
        <img src="https://img.shields.io/modrinth/dt/sable?logo=modrinth&amp;label=&amp;suffix=%20&amp;style=flat&amp;color=242629&amp;labelColor=5CA424&amp;logoColor=1C1C1C" alt="Modrinth Download"/>
    </a>
    <a href="https://www.curseforge.com/minecraft/mc-mods/sable">
        <img src="https://img.shields.io/curseforge/dt/1312371?logo=curseforge&amp;label=&amp;suffix=%20&amp;style=flat&amp;color=242629&amp;labelColor=F16436&amp;logoColor=1C1C1C" alt="CurseForge Download"/>
    </a>
</div>
</h1>

# What

This is Create Simulated's -> <a href=https://github.com/ryanhcode/sable>Sable</a> engine, ported to android.

Which is required for Create Aeronautics physics to work.

## Create Aeronautics on Android!

<b>With this repo, now you can play Create Aeronautics on android!<br>(via any pajov based launcher)</b>

# IMPORTANT

About builds:

> [!IMPORTANT]
> Not all releases are tested especially Fabric, has an release anyway.

> [!NOTE]
> This README still needs some update.
> Some information might be deprecated, be aware.

# How to setup?

Sable from releases, anything else from their sources as usual.
- Get Android version of Sable from <a href="https://github.com/aksksklskdamkwkskskd-del/sable_android/releases/">releases</a> and Create, Create Aeronautics, etc. from their sources (e.g. Modrinth).

- Tested on Amethyst Launcher (pajov fork) on Android 14.
- Using MobileGlues or Zink with Java 21 seems fine.

#### Issues

- You can inform me about issues _caused by the port_.
- Please make sure it happens even if all other mods disabled. Try using base mods: Create, **Android Sable**, Create Aeronautics.
- Using Sodium and Podium should be ok but be sure.
- Try different versions to make sure.

#### Classic Mod Installing Steps

- Get your mods inside your launchers mods folder:
 - Use an file manager like Zarchiver and Shizuku (for accessing Android/data folder on newer android versions). You can find tutorials to setup correctly.
 - Go locate your game location (.minecraft) of your launcher.
Mostly under

> Android/data/[APP-PACKAGE-NAME]/files/.minecraft

or similar.
- Inside .minecraft, create 'mods' folder and put all your mods inside.
- Go to your launcher and select 1.21.1 NeoForge (-> use latest possible) profile.
- Launch your game.

- You may have some issues, here are basic regular ones:

## Some regular issues and fixes

### /flywheel backend flywheel:off

> [!IMPORTANT]
> Fixes invisible shafts and moving parts of the blocks. Caused by flywheel rendering, related to Create, as it's embedded.

### Game crash with (critical) Signal 6

> [!IMPORTANT]
> This indicates something important.
> Mobile phones/ARM uses ram as shared for both CPU and GPU.
> Which can limit the GPU vram or normal ram levels.

> First, make sure if the resources (ram) are enough (+for GPU use).
> Then, set allocated ram **predictably enough** amount for ram usage and GPU needs balance.
> Allocation too low: Lack of resources to run, game crash
> Allocation too high: No shared ram (vram) left for GPU to work, game crash as Signal 6 immediately
> Consider android system, game and GPU load.
> 8 GB as min. and ~12 GB native ram recommended.

> For example: 12 GB ram, allocated ~5 GB

# Basic Q&A

<details>
   <summary><b>Q: Are you planning to & When will you, add [X] version to releases?</b></summary>
   
   **A:** Trying to add all versions to supported side as I can. Right now, all new releases from main repo gets ported everyday at 00:00. If everything is fine, automatic builds will occur 1 day (max) after the main repository versions are shared (by tags).</details>

</details><br>

<details>
   <summary><b>Q: What happens when main changes their code and brokes the new builds?</b></summary>
   
   **A:** I would try to fix conflicts or issues happening and implement an new building way that works (If I can).
</details><br>

<details>
   <summary><b>Q: How long will you support this project?</b></summary>
   
   **A:** Not sure. But wouldn't leave it without notifying it. Also not planing to in the near future neither.
</details><br>

<details>
   <summary><b>Q: Is it playable?</b></summary>
   
   **A:** As from my experience and others feedbacks, it is. Haven't seen an issue yet. But you can inform me about <i>port issues</i> and similar. 
Still keep in mind that it can break anytime and be buggy anyway.
</details><br>
<br><br><br>
<details>
   <summary><b>Q: how are you today</b></summary>
   
   **A:** mostly liquid (at room temperature)
</details>

# Plans List
- [x] Release building system.
- [x] First release (NeoForge).
- [x] Automation (auto deploy release).
- [x] Extra: Fabric support **(NOT TESTED)**.
- [x] FIX: Fix builds including all old versions.
- [ ] Extra: Main instructions besides android-build.yml.

# Details about building it (this)

## OLD INFO

Auto build via "Sable Native Android Port" action (.github/android-build.yml). Building it on github servers as github action.

It builds both imgui to satisfy veil and satisfy + build Sable itself.

It just compiles imgui (dependency), Rapier (physics lib) and Sable (mod) for android compatibility, puts all into each other to make the ultimate android port.

# ~Building (termux)~

Originally, I did it inside my termux environment, on the same day it came out. This repo has simpler version of that process. (With lots of AI help ofc.)

Instructions are not avaible for now.

> But planning to explain how i had it in the first place, termux version of instructions MIGHT be published here
> 
> (not an github professional here as you can see)
