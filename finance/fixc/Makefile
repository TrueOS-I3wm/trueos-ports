# $FreeBSD$

PORTNAME=		fixc
PORTVERSION=		1.2
DISTVERSIONPREFIX=	v
CATEGORIES=		finance

MAINTAINER=		blttll@gmail.com
COMMENT=		Simple Financial Information eXchange (FIX) protocol console client

USES=			go

PLIST_FILES=		bin/fixc
USE_GITHUB=		yes
GH_ACCOUNT=		blttll

do-build:
	@cd ${WRKSRC} && \
		${SETENV} ${MAKE_ENV} go build -o fixc main.go

do-install:
	 ${INSTALL_PROGRAM} ${WRKSRC}/fixc ${STAGEDIR}${PREFIX}/bin

.include <bsd.port.mk>
