# Created by: Steve Wills <swills@FreeBSD.org>
# $FreeBSD$

PORTNAME=	rbtrace
PORTVERSION=	0.4.5
CATEGORIES=	devel rubygems
MASTER_SITES=	RG

MAINTAINER=	ruby@FreeBSD.org
COMMENT=	Shows method calls inside another ruby process in real time

RUN_DEPENDS=	rubygem-ffi>=1.0.6:${PORTSDIR}/devel/rubygem-ffi \
		rubygem-trollop>=1.16.2:${PORTSDIR}/devel/rubygem-trollop \
		rubygem-msgpack>=0.4.3:${PORTSDIR}/devel/rubygem-msgpack

USE_RUBY=	yes
USE_RUBYGEMS=	yes
RUBYGEM_AUTOPLIST=yes

.include <bsd.port.mk>
