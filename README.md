# aes_cwc
This library does AES CWC decryption and encryption.

## Changes
- It makes a few changes to the endianness of the algorithm by FromSoftware.  
- Additional platform detection macro changes were added just in case targets like ARM64 were to ever be used.  
- CMake is used instead of a Visual Studio solution directly for cross-platform portability.

## Acknowledgements
- This library is based on [modes](https://github.com/BrianGladman/modes) by [Brian Gladman](https://github.com/BrianGladman).  
- The endianness changes are discovered from [ds3os](https://github.com/TLeonardUK/ds3os) by [Tim Leonard](https://github.com/TLeonardUK).

## License
The code files are subject to the original copyright and permissions granted by Brian Gladman.  
See [LICENSE.txt](LICENSE.txt) for details.