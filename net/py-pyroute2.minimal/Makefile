PORTNAME=	pyroute2.minimal
PORTVERSION=	0.7.3
CATEGORIES=	net python
MASTER_SITES=	PYPI
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}

MAINTAINER=	sunpoet@FreeBSD.org
COMMENT=	Python Netlink library: minimal installation
WWW=		https://github.com/svinota/pyroute2/tree/master/pyroute2.minimal

LICENSE=	APACHE20 GPLv2+
LICENSE_COMB=	dual
LICENSE_FILE_APACHE20=	${WRKSRC}/LICENSE.Apache-2.0
LICENSE_FILE_GPLv2+ =	${WRKSRC}/LICENSE.GPL-2.0-or-later

USES=		python:3.6+
USE_PYTHON=	autoplist concurrent distutils

NO_ARCH=	yes

.include <bsd.port.pre.mk>

.if ${PYTHON_REL} < 30800
RUN_DEPENDS+=	${PYTHON_PKGNAMEPREFIX}importlib-metadata>=0:devel/py-importlib-metadata@${PY_FLAVOR}
.endif

post-patch:
	@${CP} ${FILESDIR}/setup.py ${WRKSRC}/

.include <bsd.port.post.mk>
