# Call of Duty UO Extended

CoDUOExtended is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

====

Call of Duty UO Extended is a modification for Call of Duty UO 1.51, which does what it says it extends CoD UO with new features, increasing limits and fixing bugs.

# Usage

Your startup commandline for your Call of Duty dedicated server would look something like this.
LD_LIBRARY_PATH=$LD_LIBRARY_PATH:. LD_PRELOAD=/path/to/coduoextended.so ./coduo_lnxded

# Dependencies / libraries

sudo apt-get install build-essential
sudo apt-get install nasm
sudo apt-get install libz-dev:i386
sudo apt-get install libssl-dev:i386

[ If you're on x86_64 then you would add :i386 after the library package names ]

# Building

Clone this repo
git clone https://github.com/riicchhaarrd/codextended
cd codextended
cd src
./build.sh

You should now have a coduoextended.so file in your ../bin folder.

# MySQL / MariaDB

If you want to compile with MySQL support you have to install the libmysqlclient or libmariadbclient libraries.

Example for Debian/Ubuntu, find the respective install command for your distro e.g yum for CentOS.

sudo apt install libmariadbclient-dev:i386

# Optional

If you want to use these features, then you have to download the dependencies and place them listed under here in the respective directories.
SteamSDK, Duktape

To compile with these options you can use arguments passed to the build script.

# Questions

If you have any question add me on Discord: Prawy#3490

====

Thanks to kung foo man (http://killtube.org) and his libcod project (CoD 2 memory modification) (https://github.com/kungfooman/libcod), php (http://xtnded.org)  and his codextended project (https://github.com/riicchhaarrd/CoDExtended/)
