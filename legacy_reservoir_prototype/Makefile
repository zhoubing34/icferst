#    Copyright (C) 2006 Imperial College London and others.
#
#    Please see the AUTHORS file in the main source directory for a full list
#    of copyright holders.
#
#    Prof. C Pain
#    Applied Modelling and Computation Group
#    Department of Earth Science and Engineering
#    Imperial College London
#
#    amcgsoftware@imperial.ac.uk
#
#    This library is free software; you can redistribute it and/or
#    modify it under the terms of the GNU Lesser General Public
#    License as published by the Free Software Foundation,
#    version 2.1 of the License.
#
#    This library is distributed in the hope that it will be useful,
#    but WITHOUT ANY WARRANTY; without even the implied warranty of
#    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
#    Lesser General Public License for more details.
#
#    You should have received a copy of the GNU Lesser General Public
#    License along with this library; if not, write to the Free Software
#    Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307
#    USA
SHELL = /bin/bash
PACKAGE_NAME = fluidity

FLUIDITY = $(PACKAGE_NAME)
FC      = mpif90
FCFLAGS = -I../include -I/usr/include/python2.7 -DHAVE_NUMPY -I/usr/lib/python2.7/dist-packages/numpy/core/include -I/usr/lib/petscdir/3.6.3/include -I/usr/lib/petscdir/3.6.3/linux-gnu-c-opt/include -I/usr/include -I/usr/include/hdf5/openmpi -I/usr/lib/openmpi/include -I/usr/lib/openmpi/include/openmpi/opal/mca/event/libevent2021/libevent -I/usr/lib/openmpi/include/openmpi/opal/mca/event/libevent2021/libevent/include -I/usr/lib/openmpi/include/openmpi -Iinclude/ -DHAVE_PETSC  -I/usr/include/vtk-6.2 -I/usr/include -I/usr/include/jsoncpp -I/usr/include/python2.7 -I/usr/include/freetype2 -I/usr/include/x86_64-linux-gnu/freetype2 -I/usr/include/x86_64-linux-gnu -I/usr/include/hdf5/serial -I/usr/lib/openmpi/include/openmpi/opal/mca/event/libevent2021/libevent -I/usr/lib/openmpi/include/openmpi/opal/mca/event/libevent2021/libevent/include -I/usr/lib/openmpi/include -I/usr/lib/openmpi/include/openmpi -I/usr/include/libxml2 -I/usr/include/tcl   -DHAVE_VTK -fbounds-check -Wall -Wimplicit-interface -Wno-surprising -g -O0 -frecord-marker=4 -DHAVE_NUMPY -I/usr/lib/python2.7/dist-packages/numpy/core/include -fno-realloc-lhs -ffree-line-length-none -ffixed-line-length-none -finit-integer=-66666 -finit-real=nan -I/usr/lib/petscdir/3.6.3/include -I/usr/lib/petscdir/3.6.3/linux-gnu-c-opt/include -I/usr/include -I/usr/include/hdf5/openmpi -I/usr/lib/openmpi/include -I/usr/lib/openmpi/include/openmpi/opal/mca/event/libevent2021/libevent -I/usr/lib/openmpi/include/openmpi/opal/mca/event/libevent2021/libevent/include -I/usr/lib/openmpi/include/openmpi -Iinclude/ -fdefault-real-8 -fdefault-double-8 -I/usr/local/include -I./

MPIF90  = mpif90

CC      = mpicc
CFLAGS  = -I/usr/include/python2.7 -DHAVE_NUMPY -I/usr/lib/python2.7/dist-packages/numpy/core/include -I/usr/lib/petscdir/3.6.3/include -I/usr/lib/petscdir/3.6.3/linux-gnu-c-opt/include -I/usr/include -I/usr/include/hdf5/openmpi -I/usr/lib/openmpi/include -I/usr/lib/openmpi/include/openmpi/opal/mca/event/libevent2021/libevent -I/usr/lib/openmpi/include/openmpi/opal/mca/event/libevent2021/libevent/include -I/usr/lib/openmpi/include/openmpi -Iinclude/ -DHAVE_PETSC  -I/usr/include/vtk-6.2 -I/usr/include -I/usr/include/jsoncpp -I/usr/include/python2.7 -I/usr/include/freetype2 -I/usr/include/x86_64-linux-gnu/freetype2 -I/usr/include/x86_64-linux-gnu -I/usr/include/hdf5/serial -I/usr/lib/openmpi/include/openmpi/opal/mca/event/libevent2021/libevent -I/usr/lib/openmpi/include/openmpi/opal/mca/event/libevent2021/libevent/include -I/usr/lib/openmpi/include -I/usr/lib/openmpi/include/openmpi -I/usr/include/libxml2 -I/usr/include/tcl   -DHAVE_VTK -fbounds-check -Wall -g -O0 -I/usr/include/python2.7 -DHAVE_NUMPY -I/usr/lib/python2.7/dist-packages/numpy/core/include  -I../include -I/usr/local/include

CXX     = mpicxx
CXXFLAGS= -I/usr/include/python2.7 -DHAVE_NUMPY -I/usr/lib/python2.7/dist-packages/numpy/core/include -I/usr/lib/petscdir/3.6.3/include -I/usr/lib/petscdir/3.6.3/linux-gnu-c-opt/include -I/usr/include -I/usr/include/hdf5/openmpi -I/usr/lib/openmpi/include -I/usr/lib/openmpi/include/openmpi/opal/mca/event/libevent2021/libevent -I/usr/lib/openmpi/include/openmpi/opal/mca/event/libevent2021/libevent/include -I/usr/lib/openmpi/include/openmpi -Iinclude/ -DHAVE_PETSC  -I/usr/include/vtk-6.2 -I/usr/include -I/usr/include/jsoncpp -I/usr/include/python2.7 -I/usr/include/freetype2 -I/usr/include/x86_64-linux-gnu/freetype2 -I/usr/include/x86_64-linux-gnu -I/usr/include/hdf5/serial -I/usr/lib/openmpi/include/openmpi/opal/mca/event/libevent2021/libevent -I/usr/lib/openmpi/include/openmpi/opal/mca/event/libevent2021/libevent/include -I/usr/lib/openmpi/include -I/usr/lib/openmpi/include/openmpi -I/usr/include/libxml2 -I/usr/include/tcl   -DHAVE_VTK -fbounds-check -Wall -g -O0 -I/usr/include/python2.7 -DHAVE_NUMPY -I/usr/lib/python2.7/dist-packages/numpy/core/include  -I../include -I/usr/local/include

LINKER  = mpicxx -rdynamic   

FLLINKER = mpif90 @FLFLAGS@

MAKE    = make
AR  = ar
ARFLAGS = cr

OBJS = $(shell find . -mindepth 2 -maxdepth 2 -name '*.c' -o -name '*.cpp' -o -name '*.[fF]' -o -name '*.F90' | grep -v ^./lib | xargs)

.SUFFIXES: .f90 .F90 .c .cpp .o .a

.f90.o:
	@echo "        FC $<"
	$(FC) $(FCFLAGS) -c $<
.F90.o:
	@echo "        FC $<"
	$(FC) $(FCFLAGS) -c $<
.c.o:
	@echo "        CC $<"
	$(CC) $(CFLAGS) -c $<
.cpp.o:
	@echo "        CXX $<"
	$(CXX) $(CXXFLAGS) -c $<

default: lib/libmphase.a  main.o

# cancel implicit rule that tries to make .o from .mod with m2c:
%.o: %.mod

lib/libmphase.a: $(OBJS)
	@echo "BUILD libmphase"
	@echo "    MKDIR lib"
	@mkdir -p lib
	@echo "    MAKE src pre_diagnostics"
	@cd src; 	 $(MAKE) pre_diagnostics
	@echo "    MAKE diagnostics"
	@cd diagnostics; $(MAKE)
	@echo "    MAKE src post_diagnostics"
	@cd src; 	 $(MAKE) post_diagnostics
	@$(AR) $(ARFLAGS) lib/libmphase.a src/*.o diagnostics/*.o

clean:
	@rm -f *.o *.d include/*.mod $(PROG_EXEC) lib/*.a 
	@rm -rf bin/
	@cd src;   make clean
	@cd diagnostics; make clean
	@cd tests; PYTHONPATH=../python ../tools/testharness_MultiphasePrototype.py --clean >/dev/null
	@cd unittest; make clean


build_unittest: lib/libmphase.a
	@cd unittest; $(MAKE)

unittest: build_unittest
	@echo "RUN bin/tests"
	@../bin/unittestharness bin/tests
