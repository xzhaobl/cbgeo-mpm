# AGENTS.md

This repository is being audited only as a high-level architectural reference for building a MATLAB research-code MPM framework for geotechnical liquefaction modelling.

Do not modify source code unless explicitly requested.

Do not attempt to translate the C++ code into MATLAB.

Focus only on:

1. overall MPM solver architecture;
2. particle, mesh, material, solver, and IO separation;
3. material model interface and history variable storage;
4. test and benchmark organisation;
5. JSON/input-file design ideas;
6. whether any design is useful for a MATLAB u-p MPM framework with a Liao-type cyclic liquefaction constitutive model;
7. which ideas are too C++/HPC/MPI-specific and should not be copied into MATLAB.

Keep the audit concise and avoid deep CMake, MPI, HDF5, or Docker details unless they affect the MATLAB architecture decision.
