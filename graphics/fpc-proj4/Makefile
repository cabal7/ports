PORTREVISION=	4
CATEGORIES=	graphics lang
PKGNAMESUFFIX=	-proj4

COMMENT=	Free Pascal interface to proj library

USES=		fpc

MASTERDIR=	${.CURDIR}/../../lang/fpc
WRKUNITDIR=	${FPCSRCDIR}/packages/${PKGNAMESUFFIX:S/-//}
EXTRACTUNITDIR=	${WRKUNITDIR}

OPTIONS_DEFINE=	PROJ
PROJ_DESC=	Install proj library
OPTIONS_DEFAULT=	PROJ

PROJ_LIB_DEPENDS=	libproj.so:graphics/proj

.include "${MASTERDIR}/Makefile"
