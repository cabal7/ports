PORTNAME=	aiortc
PORTVERSION=	1.3.1
CATEGORIES=	devel multimedia python www
MASTER_SITES=	PYPI
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}

MAINTAINER=	swills@FreeBSD.org
COMMENT=	WebRTC and ORTC in Python
WWW=		https://github.com/jlaine/aiortc/

LICENSE=	BSD3CLAUSE
LICENSE_FILE=	${WRKSRC}/LICENSE

LIB_DEPENDS=	libopus.so:audio/opus \
		libvpx.so:multimedia/libvpx
BUILD_DEPENDS=	${PYTHON_PKGNAMEPREFIX}cffi>=1.0.0:devel/py-cffi@${PY_FLAVOR}
RUN_DEPENDS=	${PYTHON_PKGNAMEPREFIX}aioice>=0.7.5:devel/py-aioice@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}attrs>0:devel/py-attrs@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}av>=9.0.0:multimedia/py-av@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}crc32c>=2.1:devel/py-crc32c@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}cryptography>=2.2:security/py-cryptography@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}numpy>0:math/py-numpy@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}openssl>0:security/py-openssl@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}pyee>=9.0.0:devel/py-pyee@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}pylibsrtp>=0.5.6:devel/py-pylibsrtp@${PY_FLAVOR}

USES=		localbase python:3.5+
USE_PYTHON=	autoplist concurrent distutils

.include <bsd.port.mk>
