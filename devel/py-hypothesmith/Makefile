PORTNAME=	hypothesmith
PORTVERSION=	0.2.3
CATEGORIES=	devel
MASTER_SITES=	PYPI
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}

MAINTAINER=	amdmi3@FreeBSD.org
COMMENT=	Hypothesis strategies for generating Python programs
WWW=		https://github.com/Zac-HD/hypothesmith

LICENSE=	MPL20

RUN_DEPENDS=	${PYTHON_PKGNAMEPREFIX}hypothesis>=0:devel/py-hypothesis@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}libcst>=0:devel/py-libcst@${PY_FLAVOR}
TEST_DEPENDS=	${PYTHON_PKGNAMEPREFIX}black>=0:devel/py-black@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}parso>=0:textproc/py-parso@${PY_FLAVOR}

USES=		python:3.7+
USE_PYTHON=	autoplist distutils pytest
NO_ARCH=	yes

.include <bsd.port.mk>
