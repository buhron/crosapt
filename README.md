# crospack
Crospack is an package manager for ChromeOS (but can be installed on Linux and macOS via some script modifications).
## Installation (and removal)
**Installation**<br>
To install crospack, go to VT-2 (Ctrl+Alt+Forward(F2)) and type:
(This doesn't work yet)
```sh
sudo bash <(curl -L https://github.com/buhron/crospack/raw/refs/heads/beta/installers/install-x86_64.sh)
```

Crospack and the packages installed using crospack will be stored at `/usr/share/crospack/` <br>

**Manual Installation (custom)**<br>
Zip archives of crospack will be available in Releases if you want to install crospack to another folder (ex. `/home/chronos/user/.crospack`) Remember that when installing crospack, you will need to set the $CROSPACK_ROOT environment variable to where you installed crospack, or else crospack won't work.<br>
**Removal**
<br>
If you want to remove crospack, simply open a command line and run: `rm -rf $CROSPACK_ROOT` (You may need root previleges based on where you installed crospack, if you installed crospack normally via the command above, you can safely run this command as the script will `chown` the installation directory.
