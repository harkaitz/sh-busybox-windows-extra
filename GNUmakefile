.POSIX:
.SUFFIXES:
.PHONY: all clean install check
all:
PROJECT=busybox-windows-extra
VERSION=1.0.0
PREFIX=/usr/local

all:
clean:
install:
check:
## -- BLOCK:license --
install: install-license
install-license: 
	mkdir -p $(DESTDIR)$(PREFIX)/share/doc/$(PROJECT)
	cp LICENSE $(DESTDIR)$(PREFIX)/share/doc/$(PROJECT)
## -- BLOCK:license --
## -- BLOCK:sh --
install: install-sh
install-sh:
	mkdir -p $(DESTDIR)$(PREFIX)/bin
	cp bin/wsudo            $(DESTDIR)$(PREFIX)/bin
	cp bin/schtasks-boot    $(DESTDIR)$(PREFIX)/bin
	cp bin/schtasks-daily   $(DESTDIR)$(PREFIX)/bin
	cp bin/schtasks-list    $(DESTDIR)$(PREFIX)/bin
	cp bin/cygwin           $(DESTDIR)$(PREFIX)/bin
	cp bin/wcompat          $(DESTDIR)$(PREFIX)/bin
	cp bin/xdg-open         $(DESTDIR)$(PREFIX)/bin
## -- BLOCK:sh --
