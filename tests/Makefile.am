NULL =

AM_CPPFLAGS = \
	-DLOCALE_DIR=\""$(datadir)/locale"\" \
	-I$(top_srcdir)/src/ \
	-I$(top_srcdir)/tests/ \
	$(GLIB2_CFLAGS) \
	$(GTK_CFLAGS) \
	$(WARN_CFLAGS) \
	$(NULL)

LDADD= \
	$(top_builddir)/src/libvirt-viewer-util.la \
	$(GLIB2_LIBS) \
	$(GTK_LIBS) \
	$(LIBXML2_LIBS) \
	$(NULL)

TESTS = test-version-compare test-monitor-mapping
check_PROGRAMS = $(TESTS)
test_version_compare_SOURCES = \
	test-version-compare.c \
	$(NULL)

test_monitor_mapping_SOURCES = \
	test-monitor-mapping.c \
	$(NULL)

-include $(top_srcdir)/git.mk
