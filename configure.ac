#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.
AC_PREREQ([2.65])
AC_INIT([alvar], [0.0.1], [ntd@rice.edu])

AM_INIT_AUTOMAKE([subdir-objects])
m4_ifdef([AM_SILENT_RULES], [AM_SILENT_RULES([no])])

AC_CONFIG_SRCDIR([src/Alvar.cpp])
AC_CONFIG_HEADERS([config.h])

AC_CONFIG_MACRO_DIR([m4])

# Checks for programs.
AC_USE_SYSTEM_EXTENSIONS
AC_PROG_CXX
AM_PROG_CC_C_O
AC_PROG_LIBTOOL


PKG_CHECK_MODULES([OPENCV], [opencv])
PKG_CHECK_MODULES([EIGEN3], [eigen3])

CFLAGS="$CFLAGS $OPENCV_CFLAGS $EIGEN3_CFLAGS"
CXXFLAGS="$CXXFLAGS $OPENCV_CFLAGS $EIGEN3_CFLAGS"
LDFLAGS="$LDFLAGS $OPENCV_LIBS $EIGEN3_LDFLAGS"

dnl If

## OUTPUT @@
AC_CONFIG_FILES([Makefile])
AC_OUTPUT
