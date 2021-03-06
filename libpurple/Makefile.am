EXTRA_DIST = \
		dbus-analyze-functions.py \
		dbus-analyze-signals.py \
		dbus-analyze-types.py \
		enums.c.in \
		enums.h.in \
		glibcompat.h \
		purple-notifications-example \
		purple-remote \
		purple-send \
		purple-send-async \
		purple-url-handler \
		purple.h.in \
		tag.sh \
		version.h.in \
		Makefile.mingw \
		data/purple-3.pc.in \
		data/purple-3-uninstalled.pc.in \
		data/purple-url-handler.desktop.in \
		win32/global.mak \
		win32/libc_interface.c \
		win32/libc_interface.h \
		win32/libc_internal.h \
		win32/libpurplerc.rc.in \
		win32/rules.mak \
		win32/targets.mak \
		win32/wpurpleerror.h \
		win32/win32dep.c \
		win32/win32dep.h

SUBDIRS = . plugins protocols tests example

purple_coresources = \
	account.c \
	accounts.c \
	accountopt.c \
	blistnode.c \
	buddy.c \
	buddylist.c \
	buddyicon.c \
	chat.c \
	ciphers/aescipher.c \
	ciphers/descipher.c \
	ciphers/des3cipher.c \
	ciphers/md4hash.c \
	ciphers/pbkdf2cipher.c \
	ciphers/rc4cipher.c \
	cipher.c \
	circularbuffer.c \
	cmds.c \
	connection.c \
	contact.c \
	conversation.c \
	conversationtypes.c \
	conversations.c \
	core.c \
	countingnode.c \
	debug.c \
	e2ee.c \
	eventloop.c \
	group.c \
	http.c \
	idle.c \
	image.c \
	image-store.c \
	keyring.c \
	log.c \
	media/backend-fs2.c \
	media/backend-iface.c \
	media/candidate.c \
	media/codec.c \
	media/enum-types.c \
	media.c \
	mediamanager.c \
	memorypool.c \
	message.c \
	mime.c \
	nat-pmp.c \
	network.c \
	notify.c \
	plugins.c \
	pluginpref.c \
	pounce.c \
	prefs.c \
	presence.c \
	proxy.c \
	protocol.c \
	protocols.c \
	purple-gio.c \
	queuedoutputstream.c \
	request.c \
	request-datasheet.c \
	roomlist.c \
	savedstatuses.c \
	server.c \
	signals.c \
	smiley-custom.c \
	smiley-list.c \
	smiley-parser.c \
	smiley-theme.c \
	smiley.c \
	status.c \
	stringref.c \
	stun.c \
	sound.c \
	sound-theme.c \
	sound-theme-loader.c \
	sslconn.c \
	theme.c \
	theme-loader.c \
	theme-manager.c \
	tls-certificate.c \
	tls-certificate-info.c \
	trie.c \
	upnp.c \
	util.c \
	version.c \
	whiteboard.c \
	xfer.c \
	xmlnode.c

purple_builtsources = \
	enums.c

purple_coreheaders = \
	account.h \
	accounts.h \
	accountopt.h \
	blistnode.h \
	buddy.h \
	buddylist.h \
	buddyicon.h \
	chat.h \
	cipher.h \
	circularbuffer.h \
	cmds.h \
	connection.h \
	contact.h \
	conversation.h \
	conversationtypes.h \
	conversations.h \
	core.h \
	countingnode.h \
	dbus-maybe.h \
	debug.h \
	e2ee.h \
	eventloop.h \
	group.h \
	http.h \
	idle.h \
	image.h \
	image-store.h \
	keyring.h \
	log.h \
	media.h \
	mediamanager.h \
	memorypool.h \
	message.h \
	mime.h \
	nat-pmp.h \
	network.h \
	notify.h \
	plugins.h \
	pluginpref.h \
	pounce.h \
	prefs.h \
	presence.h \
	proxy.h \
	protocol.h \
	protocols.h \
	purple-gio.h \
	queuedoutputstream.h \
	request.h \
	request-datasheet.h \
	roomlist.h \
	savedstatuses.h \
	server.h \
	signals.h \
	smiley-custom.h \
	smiley-list.h \
	smiley-parser.h \
	smiley-theme.h \
	smiley.h \
	status.h \
	stringref.h \
	stun.h \
	sound.h \
	sound-theme.h \
	sound-theme-loader.h \
	sslconn.h \
	tests.h \
	theme.h \
	theme-loader.h \
	theme-manager.h \
	tls-certificate.h \
	tls-certificate-info.h \
	trie.h \
	upnp.h \
	util.h \
	whiteboard.h \
	xfer.h \
	xmlnode.h

if USE_VV
purple_coreheaders += media-gst.h
else
EXTRA_DIST += media-gst.h
endif

if IS_WIN32
purple_coresources += \
	win32/libc_interface.c \
	win32/win32dep.c

purple_coreheaders += \
	win32/libc_interface.h \
	win32/libc_internal.h \
	win32/win32dep.h \
	win32/wpurpleerror.h

.rc.o: %.rc
	$(AM_V_GEN)$(WINDRES) -i $< -o $@

LIBPURPLE_WIN32RES = win32/libpurplerc.o
LIBPURPLE_WIN32RES_LDFLAGS = -Wl,$(LIBPURPLE_WIN32RES)
endif

purple_mediaheaders = \
	backend-iface.h \
	candidate.h \
	codec.h \
	enum-types.h

purple_cipherheaders = \
	aescipher.h \
	descipher.h \
	des3cipher.h \
	md4hash.h \
	pbkdf2cipher.h \
	rc4cipher.h

purple_builtheaders = purple.h version.h enums.h

purple_enumheaders = \
	$(srcdir)/account.h \
	$(srcdir)/buddyicon.h \
	$(srcdir)/cipher.h \
	$(srcdir)/connection.h \
	$(srcdir)/conversation.h \
	$(srcdir)/conversationtypes.h \
	$(srcdir)/debug.h \
	$(srcdir)/eventloop.h \
	$(srcdir)/notify.h \
	$(srcdir)/plugins.h \
	$(srcdir)/protocol.h \
	$(srcdir)/protocols.h \
	$(srcdir)/roomlist.h \
	$(srcdir)/status.h \
	$(srcdir)/sound.h \
	$(srcdir)/xfer.h \
	$(srcdir)/xmlnode.h


# glib-mkenums doesn't handle VPATHs well, sed is used here to fix the
# include paths and documentation.
# Escaping possible . in $(srcdir) to \. for sed pattern.
enums.h: $(srcdir)/enums.h.in $(purple_enumheaders)
	$(AM_V_GEN)$(GLIB_MKENUMS) --template $(srcdir)/enums.h.in $(purple_enumheaders) > $@
	sed -i 's,$(subst .,\.,$(srcdir))/,,g' $@

enums.c: $(srcdir)/enums.c.in $(purple_enumheaders)
	$(AM_V_GEN)$(GLIB_MKENUMS) --template $(srcdir)/enums.c.in $(purple_enumheaders) > $@
	sed -i 's,$(subst .,\.,$(srcdir))/,,g' $@

CLEANFILES = \
	enums.c \
	enums.h

DISTCLEANFILES = \
	data/purple-url-handler.desktop

if ENABLE_DBUS

CLEANFILES += \
	dbus-bindings.c \
	dbus-client-binding.c \
	dbus-client-binding.h \
	dbus-signals.c \
	dbus-types.c \
	dbus-types.h \
	purple-client-bindings.c \
	purple-client-bindings.h \
	purple.service

# purple dbus server

dbus_sources  = dbus-server.c dbus-useful.c
dbus_headers  = dbus-server.h dbus-bindings.h dbus-purple.h dbus-useful.h dbus-define-api.h dbus-types.h

dbus_exported = dbus-useful.h dbus-define-api.h account.h accounts.h blistnode.h \
                buddy.h buddylist.h buddyicon.h connection.h conversation.h \
                conversationtypes.h conversations.h core.h xfer.h log.h notify.h \
                prefs.h presence.h roomlist.h savedstatuses.h smiley.h smiley-list.h \
				status.h server.h util.h xmlnode.h protocol.h protocols.h

# Filter out enums.h as it doesn't actually generate anything.
# This way making from a VPATH and distcheck doesn't fail due
# to not being able to find the enums.h file if it's already
# been generated in the $(srcdir).
purple_build_coreheaders = $(addprefix $(srcdir)/, $(purple_coreheaders)) \
		$(addprefix $(srcdir)/ciphers/, $(purple_cipherheaders)) \
		$(addprefix $(srcdir)/media/, $(purple_mediaheaders)) \
		$(filter-out: enums.h, $(purple_builtheaders))
dbus_build_exported = $(addprefix $(srcdir)/, $(dbus_exported))
# We should probably make this better
dbus_signals = $(addprefix $(srcdir)/, $(purple_coresources)) \
	$(srcdir)/protocols/irc/irc.c \
	$(srcdir)/protocols/jabber/jabber.c

dbus-types.c: dbus-analyze-types.py $(purple_build_coreheaders)
	$(AM_V_GEN) $(PYTHON) $(srcdir)/dbus-analyze-types.py --pattern=PURPLE_DBUS_DEFINE_TYPE\(%s\) -o $@ $(purple_build_coreheaders)

dbus-types.h: dbus-analyze-types.py $(purple_build_coreheaders)
	$(AM_V_GEN) $(PYTHON) $(srcdir)/dbus-analyze-types.py --pattern=PURPLE_DBUS_DECLARE_TYPE\(%s\) -o $@ $(purple_build_coreheaders)

dbus-bindings.c: dbus-analyze-functions.py $(dbus_exported)
	$(AM_V_GEN)$(PYTHON) $(srcdir)/dbus-analyze-functions.py -o $@ $(dbus_build_exported)

dbus-signals.c: dbus-analyze-signals.py $(dbus_signals)
	$(AM_V_GEN) $(PYTHON) $(srcdir)/dbus-analyze-signals.py -o $@ $(dbus_signals)

dbus-server.$(OBJEXT): dbus-bindings.c dbus-signals.c dbus-types.c dbus-types.h
dbus-server.lo: dbus-bindings.c dbus-signals.c dbus-types.c dbus-types.h

# Declare these as dependencies so they're built even if `make distcheck`
# is run immediately after configuring.
$(libpurple_la_OBJECTS): dbus-types.h enums.h

# libpurple-client

libpurple_client_lib = libpurple-client.la

libpurple_client_la_SOURCES = purple-client.c purple-client.h
libpurple_client_la_LDFLAGS = -version-info $(PURPLE_LT_VERSION_INFO) -no-undefined
libpurple_client_la_LIBADD = $(DBUS_LIBS)

purple-client-bindings.c: dbus-analyze-functions.py $(dbus_exported)
	$(AM_V_GEN) $(PYTHON) $(srcdir)/dbus-analyze-functions.py --client -o $@ $(dbus_build_exported)

purple-client-bindings.h: dbus-analyze-types.py dbus-analyze-functions.py $(purple_coreheaders) $(addprefix ciphers/, $(purple_cipherheaders)) $(addprefix media/, $(purple_mediaheaders)) $(purple_builtheaders) $(dbus_exported)
	$(AM_V_GEN) $(PYTHON) $(srcdir)/dbus-analyze-types.py --keyword=enum --verbatim -o $@ $(purple_build_coreheaders)
	$(AM_V_at) $(PYTHON) $(srcdir)/dbus-analyze-functions.py --client --headers --append -o $@ $(dbus_build_exported)

$(libpurple_client_la_OBJECTS): purple-client-bindings.h purple-client-bindings.c

# purple-client-example

purple_client_example_SOURCES = purple-client-example.c

purple_client_example_DEPENDENCIES = libpurple-client.la

purple_client_example_LDADD = \
	libpurple-client.la \
	$(GLIB_LIBS) \
	$(DBUS_LIBS)

bin_PROGRAMS = purple-client-example

purple-client-example.$(OBJEXT): purple-client-bindings.h

# scripts

bin_SCRIPTS = purple-remote purple-send purple-send-async purple-url-handler

BUILT_SOURCES = $(purple_builtheaders) \
	$(purple_builtsources) \
	dbus-bindings.c \
	dbus-signals.c \
	dbus-types.c \
	dbus-types.h \
	purple-client-bindings.c \
	purple-client-bindings.h

else

BUILT_SOURCES = $(purple_builtheaders) $(purple_builtsources)

# Declare these as dependencies so they're built even if `make distcheck`
# is run immediately after configuring.
$(libpurple_la_OBJECTS): enums.h

endif

lib_LTLIBRARIES = libpurple.la $(libpurple_client_lib)

libpurple_la_SOURCES = \
	$(purple_coresources) \
	$(purple_builtsources) \
	$(dbus_sources)

noinst_HEADERS= \
	internal.h \
	media/backend-fs2.h \
	valgrind.h

libpurpleincludedir=$(includedir)/libpurple
libpurpleinclude_HEADERS = \
	$(purple_coreheaders) \
	$(purple_builtheaders) \
	$(dbus_headers)

cipherincludedir=$(includedir)/libpurple/ciphers
cipherinclude_HEADERS = \
	$(addprefix $(srcdir)/ciphers/, $(purple_cipherheaders))

mediaincludedir=$(includedir)/libpurple/media
mediainclude_HEADERS = \
	$(addprefix $(srcdir)/media/, $(purple_mediaheaders))

pkgconfigdir = $(libdir)/pkgconfig
pkgconfig_DATA = data/purple-3.pc

if INSTALL_I18N
DESKTOP_FILE=data/purple-url-handler.desktop

appsdir = $(datadir)/applications
apps_in_files = data/purple-url-handler.desktop.in
apps_DATA = $(apps_in_files:.desktop.in=.desktop)

# silenced INTLTOOL_DESKTOP_RULE
%.desktop: %.desktop.in $(INTLTOOL_MERGE) $(wildcard $(top_srcdir)/po/*.po)
	$(AM_V_GEN) LC_ALL=C $(INTLTOOL_MERGE) -d -u -c $(top_builddir)/po/.intltool-merge-cache $(top_srcdir)/po $< $@ > /dev/null

@INTLTOOL_XML_RULE@

endif # INSTALL_I18N

libpurple_la_DEPENDENCIES = \
	$(STATIC_LINK_LIBS) $(LIBPURPLE_WIN32RES)

libpurple_la_LDFLAGS = -export-dynamic -version-info $(PURPLE_LT_VERSION_INFO) \
	-no-undefined $(LIBPURPLE_WIN32RES_LDFLAGS)
libpurple_la_LIBADD = \
	$(STATIC_LINK_LIBS) \
	$(DBUS_LIBS) \
	$(DNSAPI_LIBS) \
	$(GLIB_LIBS) \
	$(GPLUGIN_LIBS) \
	$(LIBXML_LIBS) \
	$(NETWORKMANAGER_LIBS) \
	$(INTLLIBS) \
	$(FARSTREAM_LIBS) \
	$(GSTREAMER_LIBS) \
	$(GSTVIDEO_LIBS) \
	$(GSTAPP_LIBS) \
	$(GSTINTERFACES_LIBS) \
	$(IDN_LIBS) \
	$(JSON_LIBS) \
	$(GNUTLS_LIBS) \
	$(NSS_LIBS) \
	$(ZLIB_LIBS) \
	$(INTROSPECTION_LIBS) \
	-lm

AM_CPPFLAGS = \
	$(GLIB_CFLAGS) \
	$(GPLUGIN_CFLAGS) \
	$(DEBUG_CFLAGS) \
	$(DBUS_CFLAGS) \
	$(LIBXML_CFLAGS) \
	$(FARSTREAM_CFLAGS) \
	$(GSTREAMER_CFLAGS) \
	$(GSTVIDEO_CFLAGS) \
	$(GSTAPP_CFLAGS) \
	$(GSTINTERFACES_CFLAGS) \
	$(IDN_CFLAGS) \
	$(NETWORKMANAGER_CFLAGS) \
	$(JSON_CFLAGS) \
	$(GNUTLS_CFLAGS) \
	$(NSS_CFLAGS) \
	$(ZLIB_CFLAGS) \
	$(INTROSPECTION_CFLAGS)

-include $(INTROSPECTION_MAKEFILE)
INTROSPECTION_GIRS =
INTROSPECTION_SCANNER_ARGS = --add-include-path=$(prefix)/share/gir-1.0 --warn-all --pkg-export=purple-$(PURPLE_MAJOR_VERSION)
INTROSPECTION_COMPILER_ARGS = --includedir=$(prefix)/share/gir-1.0

if HAVE_INTROSPECTION
introspection_sources = \
	$(libpurpleinclude_HEADERS) \
	$(addprefix ciphers/, $(purple_cipherheaders)) \
	$(addprefix media/, $(purple_mediaheaders))

Purple-$(PURPLE_MAJOR_VERSION).$(PURPLE_MINOR_VERSION).gir: $(builddir)/libpurple.la
Purple_3_0_gir_INCLUDES = Gio-2.0 GObject-2.0
if PLUGINS
Purple_3_0_gir_INCLUDES += GPlugin-0.0
endif
if ENABLE_DBUS
Purple_3_0_gir_INCLUDES += DBus-1.0 DBusGLib-1.0
endif

Purple_3_0_gir_CFLAGS = \
	-I$(srcdir) \
	$(INCLUDES) \
	-DDATADIR=\"$(datadir)\" \
	-DLIBDIR=\"$(libdir)/purple-$(PURPLE_MAJOR_VERSION)/\" \
	-DLOCALEDIR=\"$(datadir)/locale\" \
	-DSYSCONFDIR=\"$(sysconfdir)\" \
	$(GLIB_CFLAGS) \
	$(GPLUGIN_CFLAGS) \
	$(DBUS_CFLAGS) \
	$(LIBXML_CFLAGS) \
	$(FARSTREAM_CFLAGS) \
	$(GSTREAMER_CFLAGS) \
	$(GSTVIDEO_CFLAGS) \
	$(GSTINTERFACES_CFLAGS) \
	$(IDN_CFLAGS) \
	$(NETWORKMANAGER_CFLAGS) \
	$(JSON_CFLAGS) \
	$(GNUTLS_CFLAGS) \
	$(NSS_CFLAGS) \
	$(ZLIB_CFLAGS) \
	$(INTROSPECTION_CFLAGS)

Purple_3_0_gir_LIBS = $(builddir)/libpurple.la
Purple_3_0_gir_FILES = $(introspection_sources)
INTROSPECTION_GIRS += Purple-$(PURPLE_MAJOR_VERSION).$(PURPLE_MINOR_VERSION).gir

girdir = $(prefix)/share/gir-1.0 $(INTROSPECTION_GIRDIR)
gir_DATA = $(INTROSPECTION_GIRS)

typelibdir = $(prefix)/share/gir-1.0 $(INTROSPECTION_TYPELIBDIR)
typelib_DATA = $(INTROSPECTION_GIRS:.gir=.typelib)

CLEANFILES += $(gir_DATA) $(typelib_DATA)
endif
