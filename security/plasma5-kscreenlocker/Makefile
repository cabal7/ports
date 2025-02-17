PORTNAME=	kscreenlocker
DISTVERSION=	${KDE_PLASMA_VERSION}
CATEGORIES=	security kde kde-plasma

MAINTAINER=	kde@FreeBSD.org
COMMENT=	Plasma5 secure lock screen architecture
WWW=		https://www.kde.org/plasma-desktop

BUILD_DEPENDS=	ck-list-sessions:sysutils/consolekit2
LIB_DEPENDS=	libwayland-client.so:graphics/wayland \
		libxcb-keysyms.so:x11/xcb-util-keysyms
RUN_DEPENDS=	ck-list-sessions:sysutils/consolekit2\
		dbus-send:devel/dbus

USES=		cmake compiler:c++11-lib cpe gettext kde:5 pkgconfig qt:5 \
		shebangfix tar:xz xorg
USE_KDE=	auth codecs config configwidgets coreaddons crash emoticons \
		globalaccel i18n idletime init itemmodels kcmutils \
		kdeclarative layer-shell-qt notifications package \
		plasma-framework service sonnet textwidgets wayland \
		widgetsaddons windowsystem xmlgui \
		ecm:build
USE_QT=		core dbus declarative gui network qdbus widgets x11extras xml \
		buildtools:build qmake:build testlib:build
USE_XORG=	ice sm x11 xcb xcursor xext xi

CPE_VENDOR=	kde

SHEBANG_FILES=	updaters/ksreenlocker_5_3_separate_autologin.pl

.include <bsd.port.mk>
