# Sun Solaris Makefile for RPFITS (lynx, SunOS 5.9).

# The RPFITS root directory.
RPFITSROOT := ..

# Only used for locating architecture-specific code in
# $(RPFITSROOT)/code/$(RPARCH).
RPARCH := sun4sol

ifndef USEGNU
  # Sun Fortran and C compiler flags...
  FFLAGS := -O -u -xs
  CFLAGS := -O -xs
else
  # ...or if you want to use the GNU compilers.
  FC     := gfortran
  FFLAGS := -g -O -fno-automatic -Wall
  CC     := gcc
  CFLAGS := -g -O -Wall -Wno-parentheses
endif

RANLIB := ranlib

LDFLAGS :=

# Where to install stuff.
PREFIX := /usr/local

#-----------------------------------------------------------------------------
# Include generic RPFITS makefile.
-include $(RPFITSROOT)/GNUmakefile
