PORTNAME=	grape
PORTVERSION=	1.6.2
CATEGORIES=	devel rubygems
MASTER_SITES=	RG

MAINTAINER=	sunpoet@FreeBSD.org
COMMENT=	Framework for rapid API development with great conventions
WWW=		https://github.com/ruby-grape/grape

LICENSE=	MIT
LICENSE_FILE=	${WRKSRC}/LICENSE

RUN_DEPENDS=	rubygem-activesupport60>=0:devel/rubygem-activesupport60 \
		rubygem-builder>=0:devel/rubygem-builder \
		rubygem-dry-types>=1.1:devel/rubygem-dry-types \
		rubygem-mustermann-grape>=1.0.0<1.1:devel/rubygem-mustermann-grape \
		rubygem-rack>=1.3.0,3:www/rubygem-rack \
		rubygem-rack-accept>=0:www/rubygem-rack-accept \
		rubygem-virtus>=1.0.0:devel/rubygem-virtus

USES=		cpe gem
USE_RUBY=	yes

NO_ARCH=	yes

CPE_VENDOR=	ruby-grape

.include <bsd.port.mk>
