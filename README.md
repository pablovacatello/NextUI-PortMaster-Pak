# Portmaster.pak for NextUI

This is a first draft, I just took the https://github.com/ryanmsartor/TrimUI-Brick-and-Smart-Pro-Custom-MinUI-Paks files and removed everything that isn't needed for Portmaster, and applied the sound fix in the launch.sh file.

There is a lot of work that could be done to streamline this pak: remove the duplicate Portmaster folder in Apps, remove most of the System folder (TRIMUI_EX should have installed the needed files in the internal filesystem), allow changing the Roms/PORTS folder to a custom name, auto install the ports' artwork in a .media folder, etc.

## Steps to install Portmaster.pak on NextUI
1) Install TRIMUI_EX per the instructions from its repo (https://github.com/kloptops/TRIMUI_EX)
2) Install NextUI as normal and after finished, unzip the contents of the provided .zip file to the root of the sd card (if you already had nextui installed into an sd card, you can just unzip the file there, no need to reinstall)
3) Make sure you are connected to WiFi (install the WiFi pak from @josegonzalez if needed: https://github.com/josegonzalez/minui-wifi-pak)
4) Run Tools/Portmaster, it'll offer to update to the newest version, do so
5) Install a ready to run game to test Portmaster (I like Apotris or Open Tyrian, just make sure it's a game that is known to work on Trimui)
6) Run the game in PORTS/Your Game (the first time you launch a Portmaster game it'll stay a minute or so in a black screen, it's setting up some stuff I think, after the first time games launch quickly

## Troubleshooting
### I have a Mac and Portmaster crashes when fetching resources!
MacOS sometimes adds extra files to removable media, which might mess up Portmaster. In particular, check if the folder `Apps/PortMaster/PortMaster/config` in your SD card has any files that start with a dot, and delete those.
