PORTNAME=	doc
DISTVERSION=	${QT6_VERSION}
PORTREVISION=	1
CATEGORIES=	misc
PKGNAMEPREFIX=	qt6-

MAINTAINER=	kde@FreeBSD.org
COMMENT=	Qt 6 module Documentations
WWW=		https://qt-project.org

BUILD_DEPENDS=	${LOCALBASE}/include/vulkan/vulkan.h:graphics/vulkan-headers

USES=		cmake compiler:c++17-lang \
		qt-dist:6
USE_QT=		base declarative tools

ALL_TARGET=	docs
INSTALL_TARGET=	install_docs

.include <bsd.port.mk>
