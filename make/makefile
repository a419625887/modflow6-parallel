# makefile created on 2019-03-13 12:37:04.099529
# by pymake (version 1.1.0)
# using the gfortran fortran and gcc c/c++ compilers.

# Define the directories for the object and module files,
# the executable, and the executable name and path.
OBJDIR = ./obj_temp
BINDIR = .
PROGRAM = mf6

SOURCEDIR1=../src
SOURCEDIR2=../src/Exchange
SOURCEDIR3=../src/Model
SOURCEDIR4=../src/Model/Geometry
SOURCEDIR5=../src/Model/GroundWaterFlow
SOURCEDIR6=../src/Model/ModelUtilities
SOURCEDIR7=../src/Solution
SOURCEDIR8=../src/Solution/SparseMatrixSolver
SOURCEDIR9=../src/Timing
SOURCEDIR10=../src/Utilities
SOURCEDIR11=../src/Utilities/Memory
SOURCEDIR12=../src/Utilities/Observation
SOURCEDIR13=../src/Utilities/OutputControl
SOURCEDIR14=../src/Utilities/TimeSeries

VPATH = \
${SOURCEDIR1} \
${SOURCEDIR2} \
${SOURCEDIR3} \
${SOURCEDIR4} \
${SOURCEDIR5} \
${SOURCEDIR6} \
${SOURCEDIR7} \
${SOURCEDIR8} \
${SOURCEDIR9} \
${SOURCEDIR10} \
${SOURCEDIR11} \
${SOURCEDIR12} \
${SOURCEDIR13} \
${SOURCEDIR14} 

.SUFFIXES: .c .cpp .f .f90 .F90 .fpp .o

# Define the Fortran compile flags
FC = gfortran
FFLAGS = -O2 -fbacktrace 

# Define the C compile flags
CC = gcc
CFLAGS = -O3 -D_UF 

# Define the libraries
SYSLIBS = 

OBJECTS = \
$(OBJDIR)/kind.o \
$(OBJDIR)/OpenSpec.o \
$(OBJDIR)/HashTable.o \
$(OBJDIR)/version.o \
$(OBJDIR)/ims8reordering.o \
$(OBJDIR)/List.o \
$(OBJDIR)/BaseGeometry.o \
$(OBJDIR)/Xt3dAlgorithm.o \
$(OBJDIR)/Constants.o \
$(OBJDIR)/SimVariables.o \
$(OBJDIR)/genericutils.o \
$(OBJDIR)/ObsOutput.o \
$(OBJDIR)/mf6lists.o \
$(OBJDIR)/Sparse.o \
$(OBJDIR)/SmoothingFunctions.o \
$(OBJDIR)/compilerversion.o \
$(OBJDIR)/Memory.o \
$(OBJDIR)/ArrayHandlers.o \
$(OBJDIR)/TimeSeriesRecord.o \
$(OBJDIR)/MemoryList.o \
$(OBJDIR)/StringList.o \
$(OBJDIR)/Timer.o \
$(OBJDIR)/Sim.o \
$(OBJDIR)/Budget.o \
$(OBJDIR)/InputOutput.o \
$(OBJDIR)/ArrayReaders.o \
$(OBJDIR)/comarg.o \
$(OBJDIR)/RectangularGeometry.o \
$(OBJDIR)/BlockParser.o \
$(OBJDIR)/MemoryManager.o \
$(OBJDIR)/ListReader.o \
$(OBJDIR)/Iunit.o \
$(OBJDIR)/RectangularChGeometry.o \
$(OBJDIR)/CircularGeometry.o \
$(OBJDIR)/ims8linear.o \
$(OBJDIR)/ObsOutputList.o \
$(OBJDIR)/BaseModel.o \
$(OBJDIR)/TimeSeries.o \
$(OBJDIR)/DisvGeom.o \
$(OBJDIR)/NameFile.o \
$(OBJDIR)/PackageMover.o \
$(OBJDIR)/TimeSeriesFileList.o \
$(OBJDIR)/PrintSaveManager.o \
$(OBJDIR)/Connections.o \
$(OBJDIR)/BaseSolution.o \
$(OBJDIR)/Mover.o \
$(OBJDIR)/tdis.o \
$(OBJDIR)/sort.o \
$(OBJDIR)/TimeSeriesLink.o \
$(OBJDIR)/SolutionGroup.o \
$(OBJDIR)/BaseExchange.o \
$(OBJDIR)/BndUzfKinematic.o \
$(OBJDIR)/TimeSeriesManager.o \
$(OBJDIR)/DiscretizationBase.o \
$(OBJDIR)/NumericalPackage.o \
$(OBJDIR)/gwf3dis8.o \
$(OBJDIR)/gwf3disu8.o \
$(OBJDIR)/gwf3mvr8.o \
$(OBJDIR)/TimeArray.o \
$(OBJDIR)/TimeArraySeries.o \
$(OBJDIR)/gwf3ic8.o \
$(OBJDIR)/gwf3sto8.o \
$(OBJDIR)/Xt3dInterface.o \
$(OBJDIR)/gwf3disv8.o \
$(OBJDIR)/Observe.o \
$(OBJDIR)/gwf3hfb8.o \
$(OBJDIR)/OutputControlData.o \
$(OBJDIR)/ObsUtility.o \
$(OBJDIR)/TimeArraySeriesLink.o \
$(OBJDIR)/TimeArraySeriesManager.o \
$(OBJDIR)/ObsContainer.o \
$(OBJDIR)/gwf3npf8.o \
$(OBJDIR)/OutputControl.o \
$(OBJDIR)/Obs3.o \
$(OBJDIR)/gwf3oc8.o \
$(OBJDIR)/gwf3obs8.o \
$(OBJDIR)/BoundaryPackage.o \
$(OBJDIR)/gwf3riv8.o \
$(OBJDIR)/gwf3rch8.o \
$(OBJDIR)/gwf3maw8.o \
$(OBJDIR)/gwf3ghb8.o \
$(OBJDIR)/gwf3evt8.o \
$(OBJDIR)/gwf3sfr8.o \
$(OBJDIR)/NumericalModel.o \
$(OBJDIR)/gwf3lak8.o \
$(OBJDIR)/gwf3uzf8.o \
$(OBJDIR)/gwf3drn8.o \
$(OBJDIR)/gwf3wel8.o \
$(OBJDIR)/gwf3chd8.o \
$(OBJDIR)/NumericalExchange.o \
$(OBJDIR)/GhostNode.o \
$(OBJDIR)/NumericalSolution.o \
$(OBJDIR)/gwf3.o \
$(OBJDIR)/GwfGwfExchange.o \
$(OBJDIR)/SimulationCreate.o \
$(OBJDIR)/mf6.o 

# Define task functions

# Create the bin directory and compile and link the program
all: makebin | $(PROGRAM)

# Make the bin directory for the executable
makebin :
	mkdir -p $(BINDIR)

# Define the objects that make up the program
$(PROGRAM) : $(OBJECTS)
	-$(FC) $(FFLAGS) -o $@ $(OBJECTS) $(SYSLIBS) -I$(OBJDIR) -J$(OBJDIR) 

$(OBJDIR)/%.o : %.f
	@mkdir -p $(@D)
	$(FC) $(FFLAGS) -c $< -o $@ -I$(OBJDIR) -J$(OBJDIR) 

$(OBJDIR)/%.o : %.f90
	@mkdir -p $(@D)
	$(FC) $(FFLAGS) -c $< -o $@ -I$(OBJDIR) -J$(OBJDIR) 

$(OBJDIR)/%.o : %.F90
	@mkdir -p $(@D)
	$(FC) $(FFLAGS) -c $< -o $@ -I$(OBJDIR) -J$(OBJDIR) 

$(OBJDIR)/%.o : %.fpp
	@mkdir -p $(@D)
	$(FC) $(FFLAGS) -c $< -o $@ -I$(OBJDIR) -J$(OBJDIR) 

$(OBJDIR)/%.o : %.c
	@mkdir -p $(@D)
	$(CC) $(CFLAGS) -c $< -o $@

$(OBJDIR)/%.o : %.cpp
	@mkdir -p $(@D)
	$(CC) $(CFLAGS) -c $< -o $@

# Clean the object and module files and the executable
.PHONY : clean
clean : 
	-rm -rf $(OBJDIR)
	-rm -rf $(PROGRAM)

# Clean the object and module files
.PHONY : cleanobj
cleanobj : 
	-rm -rf $(OBJDIR)

