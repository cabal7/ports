PORTNAME=	portupgrade
PORTVERSION=	2.4.16
PORTREVISION=	0
PORTEPOCH=	2
CATEGORIES=	ports-mgmt
MASTER_SITES=	LOCAL/bdrewery/${PORTNAME}/ \
		http://mirror.shatow.net/freebsd/${PORTNAME}/ \
		GH

MAINTAINER=	bdrewery@FreeBSD.org
COMMENT=	FreeBSD ports/packages administration and management tool suite
WWW=		https://wiki.freebsd.org/portupgrade

LICENSE=	BSD3CLAUSE

OPTIONS_DEFINE=	DOCS

CONFLICTS_INSTALL=	portupgrade-devel

USE_GITHUB=	yes
GH_ACCOUNT=	freebsd

DIST_SUBDIR=	${PORTNAME}
USES=		uidfix
USE_RUBY=	yes

USE_LDCONFIG=	${PREFIX}/lib/compat/pkg

MAKE_ARGS=	PREFIX="${PREFIX}" RUBY="${RUBY}" \
		RUBY_SITELIBDIR="${RUBY_SITELIBDIR}" MKDIR="${MKDIR}"

EXAMPLESDIR=	${PREFIX}/share/examples/pkgtools
DOCSDIR=	${PREFIX}/share/doc/pkgtools

.include <bsd.port.pre.mk>

INSTALL_TARGET=		install
.if ${PORT_OPTIONS:MDOCS}
INSTALL_TARGET+=	install-doc
.endif

.if ${RUBY_VER} >= 3.2
# databases/ruby-bdb is BROKEN with Ruby 3.2
RUN_DEPENDS+=	rubygem-dbm>0:databases/rubygem-dbm
.else
# For PKG_DBDRIVER={bdb_btree,bdb_hash}
RUN_DEPENDS+=	${RUBY_SITEARCHLIBDIR}/bdb.so:databases/ruby-bdb
.endif

post-install:
	${MKDIR} ${STAGEDIR}${PREFIX}/lib/compat/pkg

.include <bsd.port.post.mk>
