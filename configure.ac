AC_PREREQ([2.63])
AC_INIT([csplugin-routewatch], [2.3], [http://www.clearfoundation.com/docs/developer/bug_tracker/])
AC_CONFIG_SRCDIR([csplugin-routewatch.cpp])
AM_INIT_AUTOMAKE
AC_CONFIG_HEADERS([config.h])
AC_CONFIG_MACRO_DIR([m4])
LT_INIT
AC_SUBST([LIBTOOL_DEPS])

# Checks for programs.
AC_PROG_CXX
AC_PROG_INSTALL

# Checks for libraries.

# Checks for header files.
AC_CHECK_HEADERS([sys/socket.h sys/time.h])
AC_LANG_PUSH([C++])
AC_CHECK_HEADERS([clearsync/csplugin.h], [], [AC_MSG_ERROR([clearsync header files not found.])])
AC_LANG_POP([C++])

# Checks for typedefs, structures, and compiler characteristics.
AC_TYPE_SIZE_T
AC_TYPE_SSIZE_T

# Checks for library functions.
AC_CHECK_FUNCS([memset socket strerror])

# Output
AC_CONFIG_FILES([Makefile csplugin-routewatch.spec])
AC_OUTPUT
