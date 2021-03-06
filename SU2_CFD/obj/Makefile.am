# SU2 Makefile.am for SU2_CFD
# SU2 v3.2.7 "eagle"
#
# SU2 Lead Developers: Dr. Francisco Palacios (Francisco.D.Palacios@boeing.com).
#                      Dr. Thomas D. Economon (economon@stanford.edu).
#
# SU2 Developers: Prof. Juan J. Alonso's group at Stanford University.
#                 Prof. Piero Colonna's group at Delft University of Technology.
#                 Prof. Nicolas R. Gauger's group at Kaiserslautern University of Technology.
#                 Prof. Alberto Guardone's group at Polytechnic University of Milan.
#                 Prof. Rafael Palacios' group at Imperial College London.
#
# Copyright (C) 2012-2015 SU2, the open-source CFD code.
#
# SU2 is free software; you can redistribute it and/or
# modify it under the terms of the GNU Lesser General Public
# License as published by the Free Software Foundation; either
# version 2.1 of the License, or (at your option) any later version.
#
# SU2 is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
# Lesser General Public License for more details.
#
# You should have received a copy of the GNU Lesser General Public
# License along with SU2. If not, see <http://www.gnu.org/licenses/>.
#
# Created: 		10/26/12
# Last updated: 	3/11/13
#
# Created by: 		M. Colonno
# Updated by: 		M. Colonno
#
######################################################################################

# AUTOMAKE_OPTIONS = subdir-objects
ACLOCAL_AMFLAGS = ${ACLOCAL_FLAGS}

bin_PROGRAMS = ../bin/SU2_CFD

___bin_SU2_CFD_SOURCES = ../include/definition_structure.hpp \
    ../include/fluid_model.hpp \
    ../include/fluid_model.inl \
		../include/integration_structure.hpp \
		../include/integration_structure.inl \
		../include/iteration_structure.hpp \
		../include/numerics_structure.hpp \
   	../include/numerics_machine_learning.hpp \
		../include/numerics_machine_learning.inl \
		../include/numerics_machine_learning_turbulent.hpp \
		../include/numerics_structure.inl \
		../include/output_structure.hpp \
		../include/solver_structure.hpp \
		../include/solver_structure.inl \
		../include/SU2_CFD.hpp \
    ../include/transport_model.hpp \
    ../include/transport_model.inl \
		../include/variable_structure.hpp \
		../include/variable_structure.inl \
		../src/definition_structure.cpp \
		../src/fluid_model.cpp \
    ../src/fluid_model_pig.cpp \
    ../src/fluid_model_pvdw.cpp \
    ../src/fluid_model_ppr.cpp \
		../src/integration_structure.cpp \
		../src/integration_time.cpp \
		../src/iteration_structure.cpp \
		../src/numerics_adjoint_levelset.cpp \
		../src/numerics_adjoint_mean.cpp \
		../src/numerics_adjoint_tne2.cpp \
		../src/numerics_adjoint_turbulent.cpp \
		../src/numerics_direct_poisson.cpp \
		../src/numerics_direct_elasticity.cpp \
		../src/numerics_direct_heat.cpp \
		../src/numerics_direct_mean.cpp \
		../src/numerics_direct_tne2.cpp \
		../src/numerics_direct_transition.cpp \
		../src/numerics_direct_turbulent.cpp \
		../src/numerics_direct_wave.cpp \
		../src/numerics_machine_learning.cpp \
		../src/numerics_linearized_mean.cpp \
		../src/numerics_linearized_turbulent.cpp \
		../src/numerics_structure.cpp \
		../src/numerics_machine_learning_turbulent.cpp \
		../src/numerics_template.cpp \
		../src/output_cgns.cpp \
		../src/output_structure.cpp \
		../src/output_tecplot.cpp \
    ../src/output_fieldview.cpp \
    ../src/output_su2.cpp \
    ../src/output_paraview.cpp \
		../src/solver_adjoint_levelset.cpp \
		../src/solver_adjoint_mean.cpp \
		../src/solver_adjoint_tne2.cpp \
		../src/solver_adjoint_turbulent.cpp \
		../src/solver_direct_poisson.cpp \
		../src/solver_direct_elasticity.cpp \
		../src/solver_direct_heat.cpp \
		../src/solver_direct_mean.cpp \
		../src/solver_direct_tne2.cpp \
		../src/solver_direct_transition.cpp \
		../src/solver_direct_turbulent.cpp \
		../src/solver_direct_wave.cpp \
		../src/solver_linearized_mean.cpp \
		../src/solver_linearized_turbulent.cpp \
		../src/solver_structure.cpp \
		../src/solver_template.cpp \
		../src/SU2_CFD.cpp \
    ../src/transport_model.cpp \
		../src/variable_adjoint_levelset.cpp \
		../src/variable_adjoint_mean.cpp \
		../src/variable_adjoint_tne2.cpp \
		../src/variable_adjoint_turbulent.cpp \
		../src/variable_direct_poisson.cpp \
		../src/variable_direct_elasticity.cpp \
		../src/variable_direct_heat.cpp \
		../src/variable_direct_mean.cpp \
		../src/variable_direct_tne2.cpp \
		../src/variable_direct_transition.cpp \
		../src/variable_direct_turbulent.cpp \
		../src/variable_direct_wave.cpp \
		../src/variable_linearized_mean.cpp \
		../src/variable_linearized_turbulent.cpp \
		../src/variable_structure.cpp \
		../src/variable_template.cpp

___bin_SU2_CFD_CXXFLAGS =
___bin_SU2_CFD_LDADD = ../../Common/lib/libSU2.a

# always link to built dependencies from ./externals
___bin_SU2_CFD_CXXFLAGS += @su2_externals_INCLUDES@
___bin_SU2_CFD_LDADD += @su2_externals_LIBS@

# if BUILD_CGNS
___bin_SU2_CFD_CXXFLAGS += @CGNS_CXX@
___bin_SU2_CFD_LDADD += @CGNS_LD@
# endif

# if BUILD_MUTATIONPP
___bin_SU2_CFD_CXXFLAGS += @MUTATIONPP_CXX@
___bin_SU2_CFD_LDADD += @MUTATIONPP_LD@
# endif

# if BUILD_JSONCPP
___bin_SU2_CFD_CXXFLAGS += @JSONCPP_CXX@
___bin_SU2_CFD_LDADD += @JSONCPP_LD@
# endif
