# $OpenBSD$
COMMENT =		solitaire card games collection
MODPY_EGG_VERSION =	2.0
DISTNAME =		PySolFC-${MODPY_EGG_VERSION}
PKGNAME =		pysol-${MODPY_EGG_VERSION}
CATEGORIES =		games

HOMEPAGE =		http://pysolfc.sourceforge.net/

MAINTAINER =		Dmitrij D. Czarkoff <czarkoff@gmail.com>

# GPLv3+
PERMIT_PACKAGE_CDROM =	Yes

MASTER_SITES =		${MASTER_SITE_SOURCEFORGE:=pysolfc/}
EXTRACT_SUFX =		.tar.bz2

MODULES =		lang/python \
			x11/gnome
MODPY_VERSION =		${MODPY_DEFAULT_VERSION_2}
MODGNOME_TOOLS =	desktop-file-utils

RUN_DEPENDS =		${MODPY_TKINTER_DEPENDS} \
			devel/pygame \
			graphics/py-Pillow

NO_TEST =		Yes

post-install:
	@mv ${PREFIX}/bin/pysol{.py,}

.include <bsd.port.mk>
