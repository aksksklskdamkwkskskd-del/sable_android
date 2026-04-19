<p align="center"><img src="./.idea/icon.png" alt="Logo" width="200"></p>
<h1 align="center">Sable for Android<br>
<div align="center">
   <a href="https://discord.gg/createaeronautics">
        <img alt="Discord" src="https://img.shields.io/discord/937435293294919690?style=flat&logo=discord&label=Discord&color=5865F2">
    </a>
    <a href="https://modrinth.com/mod/sable">
        <img src="https://img.shields.io/modrinth/dt/sable?logo=modrinth&amp;label=&amp;suffix=%20&amp;style=flat&amp;color=242629&amp;labelColor=5CA424&amp;logoColor=1C1C1C" alt="Modrinth Download"/>
    </a>
</div>
</h1>

# What?

I made android version of Create Aeronautics -> <a href=https://github.com/ryanhcode/sable>Sable</a> engine (with tons of ai help).
It's origin builded on the same day it came out on my termux environment. This repo has the simpler github action version of that building process.

# How

By building both imgui to satisfy veil and satisfy + build sable itself.
It just compiles imgui and sable for android compatibility, puts all into each other to make the ultimate android port.

# How do I get it running?

Download Sable from releases, get the create and create aeronautics from their sources (modrinth).
Put all 3 inside your pajov based launcher (Amethyst Launcher tested, so do recommended).
- Get inside Android/data/[YOUR LAUNCHER PACKAGE NAME]/files/.minecraft/mods and put the mods there. Just find the .minecraft, locate or create mods folder, insert these mods.
- For this: Zarchiver (file manager) and Shizuku (for accessing Android/data folder on high android versions) recommended.
- If you don't have these, install and let Zarchiver use shizuku privileges. You could find some tutorials.

- Just install and run the game on 1.21.1 NeoForge (high versions).

- For first time install, you will very likely to counter invisible shafts and moving parts of create stuff and similar. Just disable flywheel rendering by

## /flywheel backend flywheel:off

also zink rendering recommended if you have mali GPU
use these flags on your java arguments to fix some language based errors:

<p>-Duser.language=en -Duser.country=US</p>

# Building

planning to explain how i had it in the first place, termux version of instructions MIGHT be published here

(not a github professional here as you can see)
