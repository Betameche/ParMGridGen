## Source directory

INCLUDES = -I$(top_builddir)/MGridGen/IMlib

pkginclude_HEADERS = defs.h  macros.h  parmgridgen.h  proto.h  rename.h  struct.h
pkgincludedir = $(includedir)/parmgridgen

lib_LTLIBRARIES = libParMGridGen.la
libParMGridGen_la_SOURCES = comm.c  debug.c  grsetup.c  ikeysort.c  memory.c  move.c  parmgridgen.c  setup.c  util.c
libParMGridGen_la_LDFLAGS = -no-undefined -export-dynamic -version-info 1:0:0

libParMGridGen_la_LIBADD = \
	$(top_builddir)/MGridGen/IMlib/libIMlib.la \
	$(top_builddir)/MGridGen/Lib/libMGridGen.la \
	../IMParMetis-2.0/ParMETISLib/libIMparmetis.la
