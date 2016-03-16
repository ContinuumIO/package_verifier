# package_verifier
Tools for verifying the functionality and integrity of conda packages

This project aims to develop tools that verify Conda packages from an arbitrary 
source against a reference recipe.  Such verification may include:

  - Running package test suites
  - Running downstream test suites to some arbitrary level
  - Perform source and binary matching, to ensure that the package has not been tampered with
  
Another term for this is "reproducible builds."  This effort is essential for establishing trust 
in community packages if they are going to be sourced as the content of Anaconda.
  
Early investigations have pointed at https://diffoscope.org/, which appears to be primarily a Linux tool right now.
