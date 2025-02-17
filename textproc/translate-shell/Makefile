PORTNAME=	translate-shell
DISTVERSIONPREFIX=	v
DISTVERSION=	0.9.6.12
PORTREVISION=	2
CATEGORIES=	textproc

MAINTAINER=	nivit@FreeBSD.org
COMMENT=	Command line interface to translation engines
WWW=		https://www.soimort.org/translate-shell/

LICENSE=	UNLICENSE
LICENSE_FILE=	${WRKSRC}/LICENSE

BUILD_DEPENDS=	gawk:lang/gawk
RUN_DEPENDS=	bash:shells/bash \
		gawk:lang/gawk \
		gbase64:sysutils/coreutils
TEST_DEPENDS=	curl:ftp/curl \
		emacs:editors/emacs@nox \
		rlwrap:devel/rlwrap

USE_GITHUB=	yes
GH_ACCOUNT=	soimort

ALL_TARGET=	build
TEST_ENV=	LC_ALL=C.UTF-8
TEST_TARGET=	test
NO_ARCH=	yes
PLIST_FILES=	bin/trans \
		man/man1/trans.1.gz

OPTIONS_DEFINE=	FRIBIDI READLINE TEXT2SPEECH

TEXT2SPEECH_DESC=	Enable Text-to-Speech functionality via espeak

FRIBIDI_RUN_DEPENDS=	fribidi:converters/fribidi

READLINE_RUN_DEPENDS=	rlwrap:devel/rlwrap

TEXT2SPEECH_RUN_DEPENDS=	espeak-ng:audio/espeak-ng

do-install:
	${INSTALL_SCRIPT} ${WRKSRC}/build/trans ${STAGEDIR}${PREFIX}/bin/trans
	${INSTALL_MAN} ${WRKSRC}/man/trans.1 ${STAGEDIR}${MANPREFIX}/man/man1/trans.1

.include <bsd.port.mk>
