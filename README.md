# inputstream.adaptive v2.0.20 compiled for ODROID-C2 (ARM aarch64) Kodi 17.6

Addon file [inputstream.adaptive-2.0.20.zip](https://github.com/circulosmeos/inputstream.adaptive/releases/download/v2.0.20/inputstream.adaptive-2.0.20.zip) has been compiled for **Kodi 17.6** on platform **ODROID-C2** (ARM aarch64).

**DO NOT INSTALL IF YOU ARE NOT RUNNING BOTH ODROID-C2 AND KODI 17.6**

## compilation steps

	# git clone https://github.com/xbmc/xbmc.git
	# cd xbmc
	# git checkout tags/17.6-Krypton
	# cd ..
	# git clone  https://github.com/peak3d/inputstream.adaptive.git
	# cd inputstream.adaptive
	# git checkout -b Krypton origin/Krypton
	# mkdir build && cd build
	# cmake -DADDONS_TO_BUILD=inputstream.adaptive -DADDON_SRC_PREFIX=../.. -DCMAKE_BUILD_TYPE=Debug -DCMAKE_INSTALL_PREFIX=../../xbmc/addons -DPACKAGE_ZIP=1 ../../xbmc/project/cmake/addons
	# make

In case this error appears after make:
	
	checking build system type... conftools/config.guess: unable to guess system type

Do:

	# wget 'http://git.savannah.gnu.org/gitweb/?p=config.git;a=blob_plain;f=config.sub;hb=HEAD' -O ./build/expat/src/expat/conftools/config.sub
	# wget 'http://git.savannah.gnu.org/gitweb/?p=config.git;a=blob_plain;f=config.guess;hb=HEAD' -O ./build/expat/src/expat/conftools/config.guess

And repeat previous cmake and make commands.

## This is the original README of this project: [README.ORIGINAL.md](https://github.com/circulosmeos/inputstream.adaptive/blob/Krypton/README.ORIGINAL.md)