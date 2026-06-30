# aes_cwc
This library does AES CWC decryption and encryption.

## Changes
- It makes a few changes to the endianness of the algorithm by FromSoftware.  
- Additional platform detection macro changes were added just in case targets like ARM64 were to ever be used.  
- CMake is used instead of a Visual Studio solution directly for cross-platform portability.  
- A macro was added to portably get the alignment of a struct.  
- A function was added to get the size of the cwc context struct for native interop.  
- A function was added to get the alignment of the cwc context struct for native interop.

## Building
This project has been built using CMake 4.4.0-rc2 for Windows x64 on Windows 10.  
CMake would generate a solution for Visual Studio 2026, and Visual Studio could compile it.  

To build under these conditions:  
1. Download and install CMake, ensuring it gets added to PATH  
2. Download and install Visual Studio 2026 with C++ desktop support  
3. Run generate.bat, only continuing after if it was successful  
4. Go into the `generated` folder and open the `.slnx` of the project in Visual Studio 2026  
5. Build the solution as debug or release  

Other conditions will likely work just fine.  
These are currently the only tested build conditions.

## Acknowledgements
- This library is based on [modes](https://github.com/BrianGladman/modes) by [Brian Gladman](https://github.com/BrianGladman).  
- The endianness changes are discovered from [ds3os](https://github.com/TLeonardUK/ds3os) by [Tim Leonard](https://github.com/TLeonardUK).

## License
See [LICENSE.txt](LICENSE.txt) for details.