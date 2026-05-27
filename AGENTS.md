# AGENTS.md

This repository is being audited only at a high architectural level.

Do not modify source code unless explicitly requested.

Do not translate C++ code into MATLAB.

Do not focus on CMake, MPI, Docker, HDF5, or low-level HPC implementation details unless they directly affect the MATLAB architecture decision.

## Project context

The goal is to rebuild a clean MATLAB minimal production MPM host for geotechnical liquefaction modelling. The previous self-developed slope driver failed because of geostatic equilibrium, force-balance, internal-force assembly, low-mass node, and boundary/runout issues.

## Audit focus

Focus only on:

1. overall MPM solver architecture;
2. separation of particles, mesh/nodes, materials, solvers, constraints, and IO;
3. material model interface;
4. particle state/history variable storage;
5. validation and test organisation;
6. input-file or JSON design ideas;
7. force-balance and geostatic-equilibrium testing ideas;
8. boundary and constraint organisation;
9. ideas useful for a MATLAB minimal production MPM host;
10. ideas that are too C++/HPC-specific and should not be copied.

Also identify existing material models and benchmark tests that are useful as pressure tests for a MATLAB clean host, especially elastic, Mohr-Coulomb/Drucker-Prager, Modified Cam Clay, or other stateful geomechanics materials. Do not perform a full constitutive-model survey.

## Expected output

Keep the audit concise. Return a high-level architecture report and a MATLAB design recommendation.
