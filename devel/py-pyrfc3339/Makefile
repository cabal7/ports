PORTNAME=	pyrfc3339
PORTVERSION=	1.1
CATEGORIES=	devel python
MASTER_SITES=	PYPI
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}
DISTNAME=	pyRFC3339-${PORTVERSION}

MAINTAINER=	sunpoet@FreeBSD.org
COMMENT=	Generate and parse RFC 3339 timestamps
WWW=		https://pypi.org/project/pyRFC3339/

LICENSE=	MIT
LICENSE_FILE=	${WRKSRC}/LICENSE.txt

RUN_DEPENDS=	${PYTHON_PKGNAMEPREFIX}pytz>=0,1:devel/py-pytz@${PY_FLAVOR}

USES=		python:3.6+
USE_PYTHON=	autoplist concurrent distutils nose

NO_ARCH=	yes

.include <bsd.port.mk>
