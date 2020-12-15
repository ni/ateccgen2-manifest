# smartrack-manifest

Written based on the [Toradex manifest](https://git.toradex.com/cgit/toradex-manifest.git/) for building Dunfell 5.x.y Yocto BSPs, smartrack-manifest.xml will include the meta-smartrack layer for building the NI SmartRack firmware.

To use this manifest, follow these instructions on [building a reference image](https://developer.toradex.com/knowledge-base/board-support-package/openembedded-core#Building_a_Reference_Image_with_Yocto_Project). Instead of the original repo init command, run this:

> `repo init -u https://github.com/NI-SmartRack/smartrack-manifest.git -b main -m smartrack-manifest.xml`
