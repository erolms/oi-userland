#
# This file and its contents are supplied under the terms of the
# Common Development and Distribution License ("CDDL"), version 1.0.
# You may only use this file in accordance with the terms of version
# 1.0 of the CDDL.
#
# A full copy of the text of the CDDL should have accompanied this
# source.  A copy of the CDDL is also available via the Internet at
# http://www.illumos.org/license/CDDL.
#

#
# Copyright 2013 Andrzej Szeszo.  All rights reserved.
#

include ../../make-rules/shared-macros.mk

COMPONENT_NAME=mpc
COMPONENT_VERSION=1.0.1
COMPONENT_SUMMARY="libmpc - GCC 4.7 private copy"
COMPONENT_SRC= $(COMPONENT_NAME)-$(COMPONENT_VERSION)
COMPONENT_ARCHIVE= $(COMPONENT_SRC).tar.gz
COMPONENT_ARCHIVE_HASH= \
  sha256:ed5a815cfea525dc778df0cb37468b9c1b554aaf30d9328b1431ca705b7400ff
COMPONENT_ARCHIVE_URL= \
  http://multiprecision.org/mpc/download/$(COMPONENT_ARCHIVE)

include ../../make-rules/prep.mk
include ../../make-rules/configure.mk
include ../../make-rules/ips.mk

CONFIGURE_PREFIX= /usr/gcc/4.7

CONFIGURE_OPTIONS+= --with-gmp=/usr/gcc/4.7 --with-mpfr=/usr/gcc/4.7

build:          $(BUILD_32)

install:        $(INSTALL_32)
