PORTNAME=	json-jwt
PORTVERSION=	1.15.3
CATEGORIES=	www devel rubygems
MASTER_SITES=	RG
PKGNAMESUFFIX=	115

MAINTAINER=	ruby@FreeBSD.org
COMMENT=	JSON Web Token implementation in Ruby
WWW=		https://github.com/nov/json-jwt

LICENSE=	MIT
LICENSE_FILE=	${WRKSRC}/LICENSE

RUN_DEPENDS=	rubygem-activesupport60>=4.2:devel/rubygem-activesupport60 \
		rubygem-aes_key_wrap>=0:security/rubygem-aes_key_wrap \
		rubygem-bindata>=0:devel/rubygem-bindata \
		rubygem-httpclient>=0:www/rubygem-httpclient

USES=		gem
USE_RUBY=	yes

NO_ARCH=	yes

PORTSCOUT=	limit:^1\.15
.include <bsd.port.mk>
