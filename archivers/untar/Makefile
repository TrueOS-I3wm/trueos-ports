# Created by: KIMURA Shigekazu <rikimura@a011.broada.jp>
# $FreeBSD$

PORTNAME=	untar
PORTVERSION=	1.4
PORTREVISION=	1
CATEGORIES=	archivers
MASTER_SITES=	http://www.the-little-red-haired-girl.org/pub/elvis/
DISTNAME=	${PORTNAME}
EXTRACT_SUFX=	.c
EXTRACT_ONLY=

MAINTAINER=	ports@FreeBSD.org
COMMENT=	Lists/Extracts files from a "*.tgz" or "*.gz" archive

BROKEN=		unfetchable

MAKEFILE=	/usr/share/mk/bsd.prog.mk
NO_WRKSUBDIR=	yes
PLIST_FILES=	bin/untar

MAKE_ENV+=	PROG=untar NO_MAN=yes
MAKE_ARGS+=	CFLAGS="${CFLAGS} -D_POSIX_SOURCE" \
		LDFLAGS="${LDFLAGS} -static"

post-extract:
	@${CP} ${DISTDIR}/untar.c ${WRKSRC}

do-install:
	${INSTALL_PROGRAM} ${WRKSRC}/${PORTNAME} ${STAGEDIR}${PREFIX}/bin

.include <bsd.port.mk>
