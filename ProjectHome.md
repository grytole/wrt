Bla blablabla bla blabla.


---


## lualibusb1 ##
> ### For what? ###
    * To be able to control your connected to router USB devices with Lua scripts

> ### How to build ###
    * Take fresh OpenWRT trunk
    * Add link on this feed into _`feeds.conf`_ file: **`src-svn custom http://wrt.googlecode.com/svn/trunk/package`**
    * Update info about new feed: **`./scripts/feeds update custom`**
    * Add needed package in OpenWRT build system: **`./scripts/feeds install lualibusb1`**
    * Turn on package build: run **`make menuconfig`**, go to _`Languages > Lua`_ and select _`lualibusb1`_ package, then go out from menu
    * Create binaries: **`make`**

> ### How to install ###
    * Flash your router with OpenWRT and set password to make SSH work
    * Upload package to router: **`scp lualibusb1_1.0.1_ar71xx.ipk root@192.168.1.1:/tmp`**
    * Install package from router console: **`root@OpenWrt:/# opkg install /tmp/lualibusb1_1.0.1_ar71xx.ipk`**

> ### Links ###
    * [lualibusb1 project](http://code.google.com/p/lualibusb1/)


---


Bla!