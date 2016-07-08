#===========================================================================
#
# Build makefile. Builds program or library and supports installation.
#
# License  : GPL (General Public License)
# Author   : Arend Lammertink <lamare AT gmail DOT com>
# Date     : 2016/05/18 (version 0.1)
#
#===========================================================================

#---------------------------------------------------------------------------
# Main variables. At least one of the upper two MUST be set: 
#---------------------------------------------------------------------------
BINARIES  = PRU_memAccessPRUDataRam.bas  user_leds.bas \
            PRU_memAccessPRUDataRam.p user_leds.p PRUSSDRV.dts
# PRU assembler programs are output as a ".bin" file

#LIBNAME  = mylib            # default: None set.

#LIBTYPE  = static           # default: dylib for dynamically linked .so

#---------------------------------------------------------------------------
# Override some default directories
#---------------------------------------------------------------------------
#SRCDIRS  = .                # default: .
INCDIRS  = . ../include       # default: ../include
#BINDIR   = ../../bin        # default: ../bin
#LIBDIR   =                  # default: ../lib
#TESTDIR  =                  # default: ../test
#DOCDIR   =                  # default: ../doc

# Bas include files are in BBB subdir, so override defaults:
INST_FILES_INC.bas  = $(wildcard ../include/BBB/*.bi)
INST_DIR_INC.bas    = $(INST_DIR_INC)/freebasic/BBB
# Don't install example binaries
INST_FILES_BIN.bas  = 

#---------------------------------------------------------------------------
# Add own C flags
#---------------------------------------------------------------------------
#MY_CFLAGS = -D_UNIX_ # Need to define _UNIX_ for this C project


#---------------------------------------------------------------------------
# Include the dirty details aka implementation.
#---------------------------------------------------------------------------
include LaMake/build.mk       # LaMake should be installed in or linked from
                              # /usr[/local]/include 
#===========================================================================
