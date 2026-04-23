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

# IMPORTANT
> [!IMPORTANT]
> Builds are broken and being tested at the moment.
> Please wait for new fixed releases.

# What

This is Create Simulated's -> <a href=https://github.com/ryanhcode/sable>Sable</a> engine, ported to android.

Which is required for Create Aeronautics physics to work.

## Create Aeronautics on Android!

<b>With this repo, now you can play Create Aeronautics on android!<br>(via any pajov based launcher)</b>

# How can I..?

**Play?**

Sable from releases, anything else from their sources as usual.
- Get Android version of Sable from <a href="https://github.com/aksksklskdamkwkskskd-del/sable_android/releases/">releases</a> and Create, Create Aeronautics, etc. from their sources (eg. Modrinth).

- Using NeoForge **HIGHLY RECOMMENDED**.
- Fabric **is** included but **not tested** (Please inform me about Fabric, is it working fine?)

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

# Basic Q&A

<details>
   <summary><b>Q: Are you planning to & When will you, add [X] version to releases?</b></summary>
   
   **A:** Trying to add all versions to supported side as I can. Right now, all new releases from main repo gets ported everyday at 00:00. If everything is fine, automatic builds will occur 1 day (max) after the main repository versions are shared.</details>

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
</details><br>
<br><br><br>
<details>
   <summary><b>Q: how are you today</b></summary>
   
   **A:** mostly liquid (at room temperature)
</details>

# Plans List
- [x] Release building system.
- [x] First release (NeoForge)
- [x] Automation (auto deploy release)
- [x] Extra: Fabric support **(NOT TESTED)**
- [ ] Extra: Main instructions besides android-build.yml

# Details about building it (this)

Auto build via "Sable Native Android Port" action (.github/android-build.yml). Building it on github servers as github action.

It builds both imgui to satisfy veil and satisfy + build Sable itself.

It just compiles imgui and Sable for android compatibility, puts all into each other to make the ultimate android port.

# ~Building (termux)~

Originally, I did it inside my termux environment, on the same day it came out. This repo has simpler version of that process. (With a lot of AI help ofc.)

Instructions are not avaible for now.

> But planning to explain how i had it in the first place, termux version of instructions MIGHT be published here
> 
> (not an github professional here as you can see)
