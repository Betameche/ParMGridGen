## Source directory

INCLUDES = -I../ParLib -I$(top_builddir)/MGridGen/IMlib

bin_PROGRAMS = parmgridgen
parmgridgen_SOURCES = io.c  main.c  parmgridgen.c
parmgridgen_LDADD = ../IMParMetis-2.0/ParMETISLib/libIMparmetis.la ../ParLib/libParMGridGen.la \
	$(top_builddir)/MGridGen/IMlib/libIMlib.la $(top_builddir)/MGridGen/Lib/libMGridGen.la @MPILIBS@

# AM_CPPFLAGS = -I$(top_srcdir)/ParMETISLib
# LDADD = $(top_builddir)/METISLib/libmetis.la \
# 	$(top_builddir)/ParMETISLib/libparmetis.la

# check_PROGRAMS = parmgridgen
# parmgridgen_SOURCES = io.c  main.c  parmgridgen.c

MPIRUN = mpirun -np 4

check-local: $(check_PROGRAMS)
	$(MPIRUN) parmgridgen $(top_builddir)/Graphs/M6.metis 3 4 6 1 4 128
