# Created by: Thomas Dreibholz <dreibh@iem.uni-due.de>
# $FreeBSD: head/benchmarks/netperfmeter/Makefile 510673 2019-09-01 01:46:45Z yuri $

PORTNAME=	netperfmeter
PORTVERSION=	1.8.7
CATEGORIES=	benchmarks
MASTER_SITES=	https://www.uni-due.de/~be0001/netperfmeter/download/

MAINTAINER=	dreibh@iem.uni-due.de
COMMENT=	Network Performance Meter

LICENSE=	GPLv3+
LICENSE_FILE=	${WRKSRC}/COPYING

USES=		cmake shebangfix tar:xz

SHEBANG_FILES=	src/pdfembedfonts src/setpdfmetadata src/plot-netperfmeter-results

CMAKE_ARGS=	-DCMAKE_INSTALL_MANDIR=${PREFIX}/man
CMAKE_OFF=	WITH_NEAT BUILD_TEST_PROGRAMS
CMAKE_ON=	BUILD_PLOT_PROGRAMS

.include <bsd.port.mk>
