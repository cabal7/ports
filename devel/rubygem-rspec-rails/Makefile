PORTNAME=	rspec-rails
PORTVERSION=	6.0.1
CATEGORIES=	devel rubygems
MASTER_SITES=	RG

MAINTAINER=	sunpoet@FreeBSD.org
COMMENT=	Testing framework for Rails
WWW=		https://github.com/rspec/rspec-rails

LICENSE=	MIT
LICENSE_FILE=	${WRKSRC}/LICENSE.md

RUN_DEPENDS=	rubygem-actionpack61>=6.1:www/rubygem-actionpack61 \
		rubygem-activesupport61>=6.1:devel/rubygem-activesupport61 \
		rubygem-railties61>=6.1:www/rubygem-railties61 \
		rubygem-rspec-core>=3.11<4:devel/rubygem-rspec-core \
		rubygem-rspec-expectations>=3.11<4:devel/rubygem-rspec-expectations \
		rubygem-rspec-mocks>=3.11<4:devel/rubygem-rspec-mocks \
		rubygem-rspec-support>=3.11<4:devel/rubygem-rspec-support

USES=		gem
USE_RUBY=	yes

NO_ARCH=	yes

.include <bsd.port.mk>
