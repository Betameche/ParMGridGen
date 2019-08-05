# -*- Autoconf -*-
AC_PREREQ(2.61)
AC_INIT(parmgridgen, 1.0, moulitsa@cs.umn.edu)
AM_INIT_AUTOMAKE([foreign])
AC_CONFIG_HEADER([config.h])
AC_PROG_INSTALL
AC_PROG_LIBTOOL
AC_CHECK_LIB(m, sqrt)
sinclude(acx_mpi.m4)
AC_LANG_PUSH([C])
ACX_MPI([], AC_MSG_ERROR([could not compile an mpi test program]))
AC_CONFIG_FILES([Makefile 
		 mgridgen.pc
		 parmgridgen.pc
		 MGridGen/Makefile
		 MGridGen/IMlib/Makefile
		 MGridGen/Lib/Makefile
		 MGridGen/Programs/Makefile
		 ParMGridGen/Makefile
		 ParMGridGen/IMParMetis-2.0/Makefile
		 ParMGridGen/IMParMetis-2.0/ParMETISLib/Makefile
		 ParMGridGen/ParLib/Makefile
		 ParMGridGen/Programs/Makefile])
AC_OUTPUT
