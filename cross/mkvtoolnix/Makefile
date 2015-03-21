PKG_NAME = mkvtoolnix
PKG_VERS = 7.7.0
PKG_EXT = tar.xz
PKG_DIST_NAME = $(PKG_NAME)-$(PKG_VERS).$(PKG_EXT)
PKG_DIST_SITE = https://www.bunkus.org/videotools/$(PKG_NAME)/sources
PKG_DIR = $(PKG_NAME)-$(PKG_VERS)

DEPENDS = cross/python cross/curl cross/expat cross/file cross/libogg cross/libvorbis cross/flac cross/zlib cross/boost

HOMEPAGE = http://www.bunkus.org/videotools/mkvtoolnix/
COMMENT  = MKVToolNix is a set of tools to create, alter and inspect Matroska files
LICENSE  =

COMPILE_TARGET = myCompile
INSTALL_TARGET = myInstall

GNU_CONFIGURE = 1

include ../../mk/spksrc.cross-cc.mk

CONFIGURE_ARGS = --with-boost-libdir=$(STAGING_INSTALL_PREFIX)/lib --prefix=$(STAGING_INSTALL_PREFIX) --enable-gui=no

.PHONY: myCompile
myCompile:
	$(RUN) ./drake

.PHONY: myInstall
myInstall:
	$(RUN) ./drake install
