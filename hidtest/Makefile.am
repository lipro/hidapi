AM_CPPFLAGS = -I$(top_srcdir)/hidapi/

## Linux
if OS_LINUX
noinst_PROGRAMS = hidtest-libusb

hidtest_libusb_SOURCES = hidtest.cpp
hidtest_libusb_LDADD = $(top_builddir)/libusb/libhidapi-libusb.la
else

# Other OS's
noinst_PROGRAMS = hidtest

hidtest_SOURCES = hidtest.cpp
hidtest_LDADD = $(top_builddir)/$(backend)/libhidapi.la

endif
