PORTNAME=	vte3
PORTVERSION=	4.0.3
CATEGORIES=	x11-toolkits rubygems
MASTER_SITES=	RG

MAINTAINER=	sunpoet@FreeBSD.org
COMMENT=	Ruby binding of VTE for GTK+ 3
WWW=		https://ruby-gnome.github.io/

LICENSE=	LGPL21+
LICENSE_FILE=	${WRKSRC}/COPYING.LIB

BUILD_DEPENDS=	rubygem-rake>=0:devel/rubygem-rake
RUN_DEPENDS=	rubygem-gtk3>=${PORTVERSION}:x11-toolkits/rubygem-gtk3

USES=		gem gnome
USE_GNOME=	vte3
USE_RUBY=	yes

NO_ARCH=	yes

.include <bsd.port.mk>
