PORTNAME=	ldap
DISTVERSION=	3.4.0
CATEGORIES=	net python
MASTER_SITES=	PYPI
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}
DISTNAME=	python-${PORTNAME}-${PORTVERSION}

MAINTAINER=	rm@FreeBSD.org
COMMENT=	LDAP module for python, for OpenLDAP2
WWW=		https://www.python-ldap.org

LICENSE=	PSFL
LICENSE_FILE=	${WRKSRC}/LICENCE

RUN_DEPENDS=	${PYTHON_PKGNAMEPREFIX}pyasn1>0:devel/py-pyasn1@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}pyasn1-modules>0:devel/py-pyasn1-modules@${PY_FLAVOR}

USES=		python:3.6+
USE_PYTHON=	autoplist distutils
USE_OPENLDAP=	yes

post-patch:
	@${REINPLACE_CMD} -e 's|%%LOCALBASE%%|${LOCALBASE}|g' ${WRKSRC}/setup.py

post-install:
	${STRIP_CMD} ${STAGEDIR}${PYTHONPREFIX_SITELIBDIR}/_ldap*.so

.include <bsd.port.mk>
