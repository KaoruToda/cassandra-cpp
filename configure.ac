#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.

AC_PREREQ([2.69])
AC_INIT([cassandracpp], [1.2.1], [BUG-REPORT-ADDRESS])
AM_INIT_AUTOMAKE
AC_CONFIG_SRCDIR([lib/Cassandra.cpp])
AC_CONFIG_HEADERS([config.h])

AC_PROG_LIBTOOL
AC_CONFIG_MACRO_DIR([m4])


# Checks for programs.
AC_PROG_CXX
#AC_PROG_CC

AC_PROG_AWK
#AC_PROG_CC
AC_PROG_CPP
AC_PROG_INSTALL
AC_PROG_LN_S
AC_PROG_MAKE_SET
AC_PROG_RANLIB


# Checks for libraries.

# Checks for header files.
AC_CHECK_HEADERS([stdint.h])

# Install /usr/local/include/cassandracpp
AC_SUBST(includedir, $includedir/cassandra/cpp)

# Checks for typedefs, structures, and compiler characteristics.
AC_CHECK_HEADER_STDBOOL
AC_TYPE_INT16_T
AC_TYPE_INT32_T
AC_TYPE_INT64_T
AC_TYPE_SIZE_T
AC_TYPE_UINT32_T
AC_TYPE_UINT8_T

# Checks for library functions.

CPPFLAGS="$CPPFLAGS -I/usr/local/include/ -I/usr/local/include/thrift -I/usr/local/include/glib-2.0/ -L/usr/local/lib"

AC_LANG_PUSH([C++])
AC_CHECK_LIB([thrift])
AC_CHECK_HEADERS([thrift/thrift.h])
AC_LANG_POP([C++])

AC_CONFIG_FILES([Makefile
                 include/Makefile
                 lib/Makefile])
AC_OUTPUT
