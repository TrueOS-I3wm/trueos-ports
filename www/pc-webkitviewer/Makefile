# Created by: Joe Maloney <jmaloney@ixsystems.com>
# $FreeBSD$

PORTNAME=	pc-webkitviewer
PORTVERSION=	201706210943
PORTREVISION= 1
CATEGORIES=	www

MAINTAINER=	jmaloney@ixsystems.com
COMMENT=	TrueOS QT5 Utilities

LICENSE=	BSD2CLAUSE

WRKSRC_SUBDIR=  src-qt5
MAKE_ARGS=      PREFIX=${STAGEDIR}${PREFIX}

CONFLICTS=      pcbsd-utils-[0-9]*

MAKE_JOBS_UNSAFE=yes
ONLY_FOR_ARCHS= amd64
USES=           qmake shebangfix tar:xz qt:5
USE_LDCONFIG=   yes
USE_QT=        core gui network svg linguist_build \
		buildtools_build x11extras widgets multimedia webkit
USE_GL+=	gl

WRKSRC_SUBDIR=  src-qt5

QMAKE_ARGS=     CONFIG+="configure"

USE_GITHUB=	yes
GH_ACCOUNT=	trueos
GH_PROJECT=	pc-webkitviewer
GH_TAGNAME=	8fda9baa40c5e0e870e5cad383bab9f9e130a690

.include <bsd.port.mk>
