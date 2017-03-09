# $Id: Makefile,v 1.5 2009/09/25 02:00:43 wsw Exp $
#
# Copyright (C) 2012 HighPoint Technologies, Inc.
# All Rights Reserved.
#

HPT_ROOT := ../../..

C_DEFINES := -DSUPPORT_ARRAY

TARGETNAME := rr2680
TARGETTYPE := KMOD
TARGETMODS := him_rr2680.o ldm_raid50.o partition.o raid0.o raid1.o jbod.o raid5.o
TARGETOBJS := os_linux.o osm_linux.o div64.o hptinfo.o config.o

TRASH := ./spp ./update_revision.sh

include $(HPT_ROOT)/inc/linux_32mpa/Makefile.def

$(TARGETOBJS): osm_linux.h
