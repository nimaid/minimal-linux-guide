# Minimal Linux Setup Guide
A collection of resources for creating a truly minimal Linux installation.

## Premise
It is no secret that Windows has become more and more bloated over the years. Telemetry, antivirus, countless services, all of these things take up an enormous amount of RAM, CPU, and disk space.

It is also no secret that, by comparison, Linux environments (with proprietary drivers) tend to be more performant than Windows on the same hardware. Additionally, popular distributions like Ubuntu come with extensive support and come pre-installed with open-source versions of tools like email clients, web browsers, office program suites, etc. For the average user, installing Ubuntu Desktop provides a lighter-weight OS than Windows without losing any functionality.

If you want a similar user experience to Ubuntu Desktop, but lighter-weight, distributions like Lubuntu fill that niche.

However, sometimes, you need to use the computer for a single task, and you want *every possible bit of CPU and RAM* available to your program. If this is you, then it's also likely this will not be your primary OS, because the applications and background services that make operating systems like Windows so user-friendly also use up precious compute resources. You want something that is so lightweight, **only** *essential* stuff like a window manager and file browser are installed. You want **complete** control over your computer resources and user experience.

Many tasks will be either easier, faster, or even made possible using such a minimal system on limited hardware, such as:
- Gaming (I myself am using it to play heavily modded Minecraft with no lag.)
- 3D Rendering
- Machine Learning
- Video Processing

The solution is to install Ubuntu Server (which is *just* a terminal, no mouse or desktop) and then go through the process of installing and configuring a minimal graphical environment. With this setup, your OS will only use somewhere around 350MB of RAM and virtually no CPU when idle. No Linux distribution with a  pre-configured desktop environment comes close to this low of an overhead.

Such a minimal system is probably not suitable to be your main OS, else if you were to make it suitable for that, it would no longer be a highly performant minimal system. Therefore, it is recommended to dual-boot this OS with your main OS. If you choose Windows as your main OS, make sure to install Windows *first* and Ubuntu Server *last*. (When preparing for the Ubuntu Server install, I suggest using a live USB with Ubuntu Desktop to access the gParted tool to resize, move, and create partitions, as the Ubuntu Server installer is very limited in this capacity.)

This guide will walk you through setting up such a system. Along the way, you will need to make many choices about how you want your system set up. I will do my best to explain every option in full.

A high-level overview of the system is as follows:
- Ubuntu Server (base OS)
- X / Xorg (window system)
- OpenBox (window manager)
- Tint2 (panel / system tray)
  - Technically optional if you want to only use Alt+Tab.

## Guide
1. [Prepare Your System](prepare-system.md)
2. [Install Ubuntu Server](install-ubuntu.md)
3. [Install The Graphical Environment](install-gui.md)
4. [Configure Your Desktop](config-gui.md)
