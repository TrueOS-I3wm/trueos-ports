# $FreeBSD$

PORTNAME=	icingaweb2-module-graphite
DISTVERSIONPREFIX=	v
DISTVERSION=	1.1.0
PORTREVISION=	2
CATEGORIES=	net-mgmt www

MAINTAINER=	lme@FreeBSD.org
COMMENT=	Graphite integration into Icinga Web 2

LICENSE=	GPLv2
LICENSE_FILE=	${WRKSRC}/COPYING

RUN_DEPENDS=	icingaweb2>=2.5.0:net-mgmt/icingaweb2

USE_GITHUB=	yes
GH_ACCOUNT=	icinga

NO_BUILD=	yes
NO_ARCH=	yes

WWWDIR?=	${PREFIX}/www/icingaweb2/modules/${PORTNAME:C/^.*-//}

do-install:
	@${MKDIR} ${STAGEDIR}${WWWDIR}
	(cd ${WRKSRC} && \
		${COPYTREE_SHARE} . ${STAGEDIR}${WWWDIR})

.include <bsd.port.mk>
