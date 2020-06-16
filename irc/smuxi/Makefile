# $FreeBSD$

PORTNAME=	smuxi
PORTVERSION=	1.0.8
CATEGORIES=	irc
MASTER_SITES=	http://www.smuxi.org/jaws/data/files/

MAINTAINER=	fox@FreeBSD.org
COMMENT=	Smart MUltipleXed Irc

LICENSE=	LGPL21
LICENSE_FILE=	${WRKSRC}/LICENSE

BUILD_DEPENDS=	${LOCALBASE}/libdata/pkgconfig/mono-addins.pc:devel/mono-addins \
		intltool-update:textproc/intltool \
		bash:shells/bash
LIB_DEPENDS=	libstfl.so:devel/stfl
RUN_DEPENDS=	mono-addins>0:devel/mono-addins

GNU_CONFIGURE=	yes
USES=		desktop-file-utils gmake gnome mono pkgconfig gettext-tools:build
USE_GNOME=	gtksharp20
INSTALLS_ICONS=	yes

OPTIONS_DEFINE=	NLS
OPTIONS_SUB=	yes

NLS_USES=		gettext
NLS_CONFIGURE_ENABLE=	nls

CONFIGURE_SHELL="env ${LOCALBASE}/bin/bash"

MAKE_JOBS_UNSAFE=yes

.include <bsd.port.mk>
