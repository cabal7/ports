PORTNAME=	bespokesynth
DISTVERSION=	1.1.0-20221006
PORTREVISION=	1
CATEGORIES=	audio

MAINTAINER=	yuri@FreeBSD.org
COMMENT=	Software modular synth
WWW=		https://www.bespokesynth.com/

LICENSE=	GPLv3
LICENSE_FILE=	${WRKSRC}/LICENSE

BROKEN=		incompatible with the latest JUCE (juce-7.0.3), see https://github.com/BespokeSynth/BespokeSynth/issues/1047

BUILD_DEPENDS=	juce>0:devel/juce \
		pybind11>0:devel/pybind11
LIB_DEPENDS=	libasound.so:audio/alsa-lib \
		libfreetype.so:print/freetype2 \
		libjack.so:audio/jack \
		libjsoncpp.so:devel/jsoncpp \
		libpng16.so:graphics/png

USES=		cmake:noninja desktop-file-utils gl localbase:ldflags pkgconfig python
USE_GL=		gl

USE_GITHUB=	yes
GH_ACCOUNT=	BespokeSynth
GH_PROJECT=	BespokeSynth
GH_TAGNAME=	616ad67

DATADIR=	${PREFIX}/share/BespokeSynth

GH_TUPLE=	chriskohlhoff:asio:01b4e87c04abd4daec58e40463bcdc150085b269:chriskohlhoff_asio/libs/link/modules/asio-standalone \
		surge-synthesizer:tuning-library:eb8617be49ac3c2436cf54de6bff94a1b1c94acf:surge_synthesizer_tuning_library/libs/tuning-library \
		ODDSound:MTS-ESP:fcfaa59a043d515d288c9d587bf61a0a7d7571a8:ODDSound_MTS_ESP/libs/oddsound-mts/MTS-ESP \
		Ableton:link:a4e4c2f3e598e28e5bea90002f954b997b8c8c53:Ableton_link/libs/link \
		cameron314:readerwriterqueue:8e7627d:readerwriterqueue/libs/readerwriterqueue

CMAKE_ON=	BESPOKE_SYSTEM_JUCE \
		BESPOKE_SYSTEM_PYBIND11 \
		BESPOKE_SYSTEM_JSONCPP

CXXFLAGS+=	-DJUCE_INCLUDE_PNGLIB_CODE=0
LDFLAGS+=	-lpng

.include <bsd.port.mk>
