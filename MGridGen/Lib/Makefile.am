## Source directory

INCLUDES = -I../IMlib

pkginclude_HEADERS = defs.h  macros.h  mgridgen.h  proto.h  struct.h
pkgincludedir = $(includedir)/mgridgen

lib_LTLIBRARIES = libMGridGen.la
libMGridGen_la_SOURCES = aratio.c  coarsen.c  kwayfm.c  match.c  merge.c  mgridgen.c  refine.c  setup.c
libMGridGen_la_LDFLAGS = -no-undefined -export-dynamic -version-info 1:0:0

libMGridGen_la_LIBADD = ../IMlib/libIMlib.la
