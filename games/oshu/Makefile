# $OpenBSD: Makefile$

COMMENT =	Fast osu! port

V =	2.0.1
DISTNAME =	${V}
PKGNAME =	oshu-${V}

CATEGORIES =	games

MAINTAINER =	Paul Valencia <reivyr@enmadechi.com>

#GPLv3+
PERMIT_PACKAGE =	Yes

WANTLIB += ${COMPILER_LIBCXX} c m
WANTLIB += SDL2 SDL2_image
WANTLIB += cairo glib-2.0 gobject-2.0 harfbuzz
WANTLIB += intl pango-1.0 pangocairo-1.0
WANTLIB += avcodec avformat avutil swresample

MASTER_SITES =	https://github.com/fmang/oshu/archive/

COMPILER =	base-clang ports-gcc

MODULES =	devel/cmake

RUN_DEPENDS =	devel/desktop-file-utils \
		misc/shared-mime-info

LIB_DEPENDS =	devel/sdl2-image \
		graphics/cairo \
		devel/glib2 \
		devel/pango \
		graphics/ffmpeg

WRKDIST =	${WRKDIR}/${PKGNAME}

.include <bsd.port.mk>
