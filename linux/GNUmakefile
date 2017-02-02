# Linux Makefile for RPFITS (grus, Debian etch).

# The RPFITS root directory.
RPFITSROOT := ..

# Only used for locating architecture-specific code in
# $(RPFITSROOT)/code/$(RPARCH).
RPARCH := linux

# Select Fortran compiler flags based on the value of FC, gfortran or g77.
# FC defaults to gfortran but can be overridden on the command line, i.e.
# 'make FC=g77'.
FFLAGS_gfortran := -g -O -fimplicit-none -Wall
FFLAGS_g77      := -g -O -fno-automatic -Wall -Wimplicit -Wno-globals

# GNU Fortran and C compiler flags.
FC     := gfortran
FFLAGS := $(FFLAGS_$(FC))
CFLAGS := -g -O -Wall
RANLIB := ranlib

LDFLAGS :=

# Where to install stuff.
PREFIX := /usr/local

#-----------------------------------------------------------------------------
# Include generic RPFITS makefile.
-include $(RPFITSROOT)/GNUmakefile
