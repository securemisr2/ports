# $FreeBSD$

PORTNAME=	arcanist
PORTVERSION=	20150423
CATEGORIES=	devel
PKGNAMEPREFIX=	php5-

MAINTAINER=	grembo@FreeBSD.org
COMMENT=	Command line interface for Phabricator

LICENSE=	APACHE20

CONFLICTS=	arc-*

PHP_DESTDIR=	lib/php/arcanist
RUN_DEPENDS=	php5-libphutil>0:${PORTSDIR}/devel/libphutil
USE_PHP=	curl json simplexml
USE_GITHUB=	yes
NO_BUILD=	yes
GH_ACCOUNT=	phacility
GH_TAGNAME=	9ddf37b

do-install:
	@${MKDIR} ${STAGEDIR}${PREFIX}/${PHP_DESTDIR}
	cd ${WRKSRC} ; ${PAX} -rw * ${STAGEDIR}${PREFIX}/${PHP_DESTDIR}
	${LN} -sf ${PREFIX}/${PHP_DESTDIR}/scripts/arcanist.php ${STAGEDIR}${PREFIX}/bin/arc

.include <bsd.port.mk>
