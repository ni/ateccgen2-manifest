# smartrack-manifest

Written based on the [Toradex manifest](https://git.toradex.com/cgit/toradex-manifest.git/) for building Yocto BSPs, smartrack-manifest.xml will include the meta-smartrack layer for building the NI Smart Rack RCU Image.

To use this manifest, follow these instructions on [building a reference image](https://developer.toradex.com/knowledge-base/board-support-package/openembedded-core#Building_a_Reference_Image_with_Yocto_Project). Instead of the original repo init command, run this:

> `repo init -u https://github.com/ni/smartrack-manifest.git -b $GITBRANCH -m smartrack-manifest.xml`
