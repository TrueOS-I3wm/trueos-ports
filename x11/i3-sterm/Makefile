# $FreeBSD$


PORTNAME=	i3
DISTVERSION=	2019011200
CATEGORIES=	x11
PKGNAMESUFFIX=	-sterm

MAINTAINER=	miwi@FreeBSD.org
COMMENT=	Simple X terminal

LICENSE=	MIT
LICENSE_FILE=	${WRKSRC}/LICENSE

RUN_DEPENDS=	${LOCALBASE}/share/fonts/powerline-fonts/SpaceMono-Bold.ttf:x11-fonts/powerline-fonts
LIB_DEPENDS=	libfontconfig.so:x11-fonts/fontconfig \
		libfreetype.so:print/freetype2

USES=		pkgconfig
USE_XORG=	x11 xext xft xrender

USE_GITHUB=	yes
GH_ACCOUNT=	trueos-i3wm
GH_PROJECT=	st
GH_TAGNAME=	afdaec8

PLIST_FILES=	bin/st man/man1/st.1.gz

# This way we avoid running tic on st.info which does not work as expected.
BINARY_ALIAS=	tic=true

PORTDATA=	config.h config.mk st.info

post-patch:
	@${REINPLACE_CMD} -e "s|^MANPREFIX = .*|MANPREFIX = ${MANPREFIX}/man|" \
	${WRKSRC}/config.mk

post-install:
	@${STRIP_CMD} ${STAGEDIR}${PREFIX}/bin/st
	@${MKDIR} ${STAGEDIR}${DATADIR}
	cd ${WRKSRC} && ${INSTALL_DATA} ${PORTDATA} ${STAGEDIR}${DATADIR}

.include <bsd.port.mk>
