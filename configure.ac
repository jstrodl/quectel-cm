AC_INIT([quectel-cm], [1.6.0.12-js0.1], [johannes.strodl@gmail.com])
AC_CONFIG_AUX_DIR(config)
AC_CONFIG_SRCDIR(src/quectel_cm.c)

AM_INIT_AUTOMAKE

AC_PROG_CC

AC_CHECK_HEADERS([linux/un.h linux/if.h linux/usbdevice_fs.h linux/types.h linux/if_ether.h],
        [],
        [missing_linux_headers="yes"])
AS_IF([test "x$missing_linux_headers" = "xyes"],
        [AC_MSG_ERROR([Missing linux headers.])])

AC_OUTPUT(Makefile src/Makefile)

