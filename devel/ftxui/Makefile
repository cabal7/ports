PORTNAME=	ftxui
DISTVERSIONPREFIX=	v
DISTVERSION=	3.0.0-69
DISTVERSIONSUFFIX=	-g90dfcee
CATEGORIES=	devel science

MAINTAINER=	yuri@FreeBSD.org
COMMENT=	C++ Functional Terminal User Interface library
WWW=		https://github.com/ArthurSonzogni/FTXUI

LICENSE=	MIT
LICENSE_FILE=	${WRKSRC}/LICENSE

USES=		cmake:testing compiler:c++17-lang
USE_LDCONFIG=	yes

USE_GITHUB=	yes
GH_ACCOUNT=	ArthurSonzogni
GH_PROJECT=	FTXUI

CMAKE_OFF=	FTXUI_BUILD_DOCS FTXUI_BUILD_EXAMPLES FTXUI_BUILD_TESTS
CMAKE_ON=	BUILD_SHARED_LIBS
CMAKE_TESTING_ON=	FTXUI_BUILD_TESTS

# tests fail to build, see https://github.com/ArthurSonzogni/FTXUI/issues/551

.include <bsd.port.mk>
