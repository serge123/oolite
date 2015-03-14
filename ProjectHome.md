# Patching Oolite source code in Gentoo #

  * **Install packages (tested)**

> >=gnustep-base/gnustep-make-2.6.6

> >gnustep-base/gnustep-gui-0.22.0

> >gnustep-base/gnustep-back-cairo-0.22.0

> >virtual/gnustep-back-0.22.0

> sys-devel/gcc +objc

> gnustep-base/gnustep-make +native-exceptions


  * **Get Oolite source with**

> git clone https://github.com/OoliteProject/oolite.git

> cd oolite

> git submodule update --init

  * **Download patch and unpack it.**

> cd ../

> wget https://oolite.googlecode.com/git/oolite-gentoo-patch-2014-12-24.tar.bz2

> tar xvjf oolite-gentoo-patch-2014-12-24.tar.bz2

> cp oolite-gentoo-patch-2014-12-24/oolite-gentoo.patch oolite

> cp oolite-gentoo-patch-2014-12-24/oolite-gentoo-patch.sh oolite

> cd oolite

  * **Apply patch with**

> sh oolite-gentoo-patch.sh

  * **Compile**

> . /usr/share/GNUstep/Makefiles/GNUstep.sh

> make -fMakefile release-snapshot

**Details how to compile on** http://www.aegidian.org/bb/viewtopic.php?f=9&t=4595&start=165