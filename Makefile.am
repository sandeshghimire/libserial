SUBDIRS=src doc examples

if PYTHON
SUBDIRS += sip
endif

ACLOCAL_AMFLAGS=-I m4

EXTRA_DIST = doxygen.conf.in Makefile.dist libserial.spec libserial.pc

docs: 
	make dox

dox:
	doxygen doxygen.conf

pkgconfigdir   = $(libdir)/pkgconfig
pkgconfig_DATA = libserial.pc
