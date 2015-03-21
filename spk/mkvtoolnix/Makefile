SPK_NAME = mkvtoolnix
SPK_VERS = 7.3.0
SPK_REV = 1
SPK_ICON = src/mkvtoolnix.png

DEPENDS = cross/$(SPK_NAME)

MAINTAINER = SynoCommunity
DESCRIPTION = MKVToolNix is a set of tools to create, alter and inspect Matroska files.
DESCRIPTION_GER = MKVToolNix stellt eine Reihe von Werkzeugen bereit, um Dateien im freien Containerformat Matroska zu erzeugen, zu ändern oder zu untersuchen.
STARTABLE = no
RELOAD_UI = no
DISPLAY_NAME = MKVToolNix
CHANGELOG = "initial cross-compile"

HOMEPAGE = http://www.bunkus.org/videotools/mkvtoolnix/
LICENSE  =

INSTALLER_SCRIPT = src/installer.sh
SSS_SCRIPT       = src/dsm-control.sh

INSTALL_PREFIX = /usr/local/$(SPK_NAME)

PRE_COPY_TARGET = myPreCopy

include ../../mk/spksrc.spk.mk

.PHONY: myPreCopy
myPreCopy:
	cp $(WORK_DIR)/../PLIST $(WORK_DIR)/PLIST
	

