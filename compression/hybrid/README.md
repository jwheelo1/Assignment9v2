# Hybrid Compression

Hybrid compression combines the Burrows-Wheeler Transform with RLE encoding.

## Getting Started Steps

- running "make clean" will clean the project by removing all "pycache" folders and files
- running "make format will run autopep8 and docformatter to auto format the code
- running "make style" will run a lint checker on your code
- running "make test" or "make" will run all unit tests that have been created
- running "make coverage" will run all unit tests and give you a code coverage report

## Hybrid Compression

### Requirements

- You must implement a class that handles the below interfaces for hybrid compression.
- The class name must be called "Hybrid".
- You must implement at least 14 unit tests.
- Must get a 10/10 when running "make style"
- Your unit tests must reach 100% code coverage

### Interface

- The function hybrid_encode(self, data) performs the BWT and then RLE encoding, returning the final encoding.

Example: 'Test input. Test input. Test input.' -> '2.6t^2 |3T3 3i3n3e3s3u3p.'

- The function hybrid_decode(self, encoding) performs RLE decoding and then the inverse BWT, returning the final decoding

### Tests

- Perform encoding and decoding on data
- Perform an encoding and decoding, ensuring the result is the same as the original.

### Corner Cases

- Encoding an empty string

## Library

You can only use basic python libraries (no special imports).
