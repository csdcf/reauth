#-----------------------------------------------------------------------------
# Install afsutil shell scripts into AFSland for cs.stanford.edu
#
# $Id$
# $Source$
#-----------------------------------------------------------------------------


BASEDIR=/afs/.cs/package/reauth
SYSNAME=`fs sysname | cut -d " " -f 4 | sed -e "s/'//g"`

INSTALL_COMMON_BINDIR=${BASEDIR}/common/bin
INSTALL_COMMON_SBINDIR=${BASEDIR}/common/sbin

INSTALL_ARCH_BINDIR=${BASEDIR}/${SYSNAME}/bin
INSTALL_ARCH_SBINDIR=${BASEDIR}/${SYSNAME}/sbin

COMMON_BIN = reauth

install-bin: ${COMMON_BIN}
	@cp -v ${COMMON_BIN} ${INSTALL_COMMON_BINDIR}

install: install-bin

