# $FreeBSD$

PORTNAME=	zsh-autosuggestions
DISTVERSIONPREFIX=	v
DISTVERSION=	0.6.3
CATEGORIES=	shells

MAINTAINER=	jrm@FreeBSD.org
COMMENT=	Fish-like autosuggestions for Zsh

LICENSE=	MIT
LICENSE_FILE=	${WRKSRC}/LICENSE

RUN_DEPENDS=	zsh>=4.3:shells/zsh

USE_GITHUB=	yes
GH_ACCOUNT=	zsh-users

NO_ARCH=	yes
NO_BUILD=	yes
PLIST_FILES=	${DATADIR}/${PORTNAME}.zsh
SUB_FILES=	pkg-message

do-install:
	@${MKDIR} ${STAGEDIR}${DATADIR}
	${INSTALL_DATA} ${WRKSRC}/zsh-autosuggestions.zsh ${STAGEDIR}/${DATADIR}

.include <bsd.port.mk>
