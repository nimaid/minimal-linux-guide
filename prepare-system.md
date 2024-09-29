# Prepare Your System
*[Back to the main page.](README.md)*

If you want to install Ubuntu Server as your primary OS, you can skip this step.

Additionally, if you have separate hard drives for separate operating systems, and you plan on giving Ubuntu Server it's own hard drive, you can skip this step.

## A Word On Disk Space and Filesystems
These instructions assume you have your primary operating system already installed, and that you have some free space on that hard drive you are willing to "sacrifice" to use for Ubuntu Server. I suggest at least 10 GB, but if you plan on installing a lot of heavy programs, you will want more. 50 GB should be more than enough for all the programs you want.

I suggest storing files on your primary OS. You can still access these partitions in Ubuntu and use them like a separate hard drive. While Linux can read Windows filesystems (`NTFS`), Windows *cannot* read Linux filesystems (`ext4`).

## Partitioning Your Hard Drive
Ubuntu Server needs, it's own partitions, the simplest setup is as follows:
- The root folder (`/`), an `ext4` filesystem.
  - The main drive, required.
- A swap partition ("virtual RAM"), a `swap` filesystem.
  - Not required but highly recommended, particularly on systems with low RAM.

TODO