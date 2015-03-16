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

MODULES =		lang/python
MODPY_VERSION =		2.7

RUN_DEPENDS =		${MODPY_TKINTER_DEPENDS} \
			devel/pygame \
			graphics/py-Pillow

post-install:
	@mv ${PREFIX}/bin/pysol{.py,}

.include <bsd.port.mk>