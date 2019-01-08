# Created by: Martin Wilke <miwi@FreeBSD.org>
# $FreeBSD$

PORTNAME=	miwinb
PORTVERSION=	0.13
CATEGORIES=	base misc

MAINTAINER=	miwi@FreeBSD.org
COMMENT=	Desktop Port

RUN_DEPENDS+=	xorg>0:x11/xorg  \
		urxvt:x11/rxvt-unicode \
		urxvt:x11/urxvt-perls \
		vim:editors/vim-console \
		x11-ssh-askpass:security/openssh-askpass \
		porttools>0:ports-mgmt/porttools \
		psearch:ports-mgmt/psearch \
		zsh:shells/zsh \
		git:devel/git \
		firefox:www/firefox \
		neomutt:mail/neomutt \
		bz:ports-mgmt/freebsd-bugzilla-cli \
		mc:misc/mc  \
		svn:devel/subversion \
		rsync:net/rsync \
		python:lang/python \
		openvpn:security/openvpn \
		synergyc:sysutils/synergy \
		/boot/modules/i915kms.ko:graphics/drm-current-kmod \
		slim:x11/slim \
		htop:sysutils/htop \
		${LOCALBASE}/share/fonts/powerline-fonts/SpaceMono-Bold.ttf:x11-fonts/powerline-fonts \
		i3:x11-wm/i3 \
		i3lock:x11/i3lock \
		i3status:x11/i3status \
		dunst:sysutils/dunst \
		rofi:x11/rofi \
		feh:graphics/feh \
		unzip:archivers/unzip \
		powermon:sysutils/powermon \
		powerdxx:sysutils/powerdxx \
		xautolock:x11/xautolock \
		py3status:deskutils/py-py3status \
		networkmgr:net-mgmt/networkmgr \
		lxrandr:x11/lxrandr \
		sysup:sysutils/sysup \
		gcalcli:deskutils/gcalcli \
		neofetch:sysutils/neofetch \
		graphics/scrot

USES=		metaport font
NO_ARCH=	yes

.include <bsd.port.mk>
