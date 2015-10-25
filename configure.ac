#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.

AC_PREREQ([2.69])
AC_INIT([tacc], [1.7], [tacc-bug-reports@kravietz.industries])
AM_INIT_AUTOMAKE([1.8 gnu])

AC_LANG([C])
AC_PROG_CC
AC_PROG_INSTALL
AC_PROG_MAKE_SET
AC_PROG_RANLIB

AC_SEARCH_LIBS([OPENSSL_secure_malloc], [crypto], [], [])
AC_SEARCH_LIBS([RAND_bytes], [crypto], [], [])
AC_SEARCH_LIBS([logwtmp], [util], [], [])

AC_CHECK_HEADERS([arpa/inet.h fcntl.h malloc.h netdb.h netinet/in.h stdlib.h string.h sys/file.h sys/param.h sys/socket.h sys/time.h syslog.h unistd.h utmp.h])

AC_TYPE_PID_T
AC_TYPE_SIZE_T

AC_FUNC_FORK
AC_FUNC_REALLOC
AC_CHECK_FUNCS([alarm bzero gethostbyname getpass gettimeofday inet_ntoa memset socket])

AX_PRINTF_SIZE_T

AC_CONFIG_FILES([Makefile libtacc/Makefile])
AC_CONFIG_SRCDIR([tacc.c])
AC_CONFIG_HEADERS([config.h])

AC_OUTPUT
