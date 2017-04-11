
AC_PREREQ([2.67])
AC_INIT([libsmartchain], [0.1], [n.schaetti@gmail.com])
AM_INIT_AUTOMAKE([1.10 -Wall no-define])
AC_CONFIG_MACRO_DIR([m4])
m4_ifdef([AM_PROG_AR], [AM_PROG_AR])

# Check for programs
AC_PROG_CXX
LT_INIT([disable-static])
AC_ENABLE_SHARED
AC_DISABLE_STATIC

AC_CHECK_LIB([crypto], [MD5_Init], [PTHREAD_LIBS="-lcrypto" LIBS="$LIBS -lcrypto"],[AC_MSG_ERROR([libssl library is missing])])

# Config files
AC_CONFIG_FILES([Makefile src/Makefile])

AC_OUTPUT
