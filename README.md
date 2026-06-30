# aes_cwc
This library does AES CWC decryption and encryption.

## Changes
- It makes a few changes to the endianness of the algorithm by FromSoftware.  
- Additional platform detection macro changes were added just in case targets like ARM64 were to ever be used.  
- CMake is used instead of a Visual Studio solution directly for cross-platform portability.  
- A macro was added to portably get the alignment of a struct.  
- A function was added to get the size of the cwc context struct for native interop.  
- A function was added to get the alignment of the cwc context struct for native interop.

## Acknowledgements
- This library is based on [modes](https://github.com/BrianGladman/modes) by [Brian Gladman](https://github.com/BrianGladman).  
- The endianness changes are discovered from [ds3os](https://github.com/TLeonardUK/ds3os) by [Tim Leonard](https://github.com/TLeonardUK).

## License
See [LICENSE.txt](LICENSE.txt) for details.