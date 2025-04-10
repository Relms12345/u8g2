AC_INIT([otf2bdf], [3.1], [your-email@example.com])
AM_INIT_AUTOMAKE([-Wall -Werror foreign])
AC_CONFIG_SRCDIR([otf2bdf.c])
AC_PROG_CC

# Check for freetype2 via pkg-config (requires version 2.0 or higher)
PKG_CHECK_MODULES([FREETYPE2], [freetype2 >= 2.0],
  [
    AC_SUBST(FREETYPE2_CFLAGS)
    AC_SUBST(FREETYPE2_LIBS)
  ],
  [
    AC_MSG_ERROR([freetype2 library not found; please install freetype2])
  ]
)

AC_CONFIG_FILES([Makefile])
AC_OUTPUT
