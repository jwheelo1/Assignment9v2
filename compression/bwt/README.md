# BWT

## Getting Started Steps

- running "make clean" will clean the project by removing all "pycache" folders and files
- running "make format will run autopep8 and docformatter to auto format the code
- running "make style" will run a lint checker on your code
- running "make test" or "make" will run all unit tests that have been created
- running "make coverage" will run all unit tests and give you a code coverage report

## Burrows-Wheeler Transform

### Requirements

- You must implement a class that handles the below interfaces for a Burrows-Wheeler Transform.
- The class name must be called "BWT".
- You must implement at least 14 unit tests.
- Must get a 10/10 when running "make style"
- Your unit tests must reach 100% code coverage

### Interface

- The function bw_transform(self, data) performs the Burrows-Wheeler transform on data, and returns the result. The encoding should first be modified to contain the start of data marker "^" and the end of data marker "|". After this, the transform should be done.
Data should be a string and a string should be returned.

Example: 'Test input. Test input. Test input.' -> '..tttttt^  |TTT   iiinnneeesssuuuppp.'

- The function bw_inv_transform(self, encoding) returns the decoding of encoding using the inverse Burrows-Wheeler transform. The decoding should not contain the previous markers.
Encoding should be a string and a string should be returned.

Example: '.tteett^ |ssvvtt  iiIInneerreessuu  ppnn.' -> 'Inverse test input. Inverse test input.'

### Tests

- Perform the BWT and inverse BWT on data.
- Perform an encoding and decoding, ensuring the result is the same as the original.

### Corner Cases

- BWT on an empty string

## Library

You can only use basic python libraries (no special imports).