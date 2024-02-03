# Dual Boot Kernel Patcher
> Based On [SurfaceDuoDualBootKernelImagePatcher
](https://github.com/WOA-Project/SurfaceDuoDualBootKernelImagePatcher)  

## Build
  - Preparation
    + A computer with Windows or Linux
    + Clang or GCC as host compiler
    + aarch64 GNU Assembler
    + Git
    + CMake
  - Clone this repo
    ```
        git clone https://github.com/woa-msmnile/DualBootKernelPacther
    ```
  - Setup CMake.
    ```
        cd DualBootKernelPacther
        cmake -B output -S .
    ```
  - Build !
    ```
        cmake --build output -j 12
    ```
## Usage
  - Common usage.
    ```
    DualBootKernelPatcher <Kernel Image to Patch> <UEFI FD Image> <Patched Kernel Image Destination> <Config> <ShellCodeBinary>
    ```
  - Example
    ```
    DualBootKernelPatcher kernel SM8150_EFI.fd PacthedKernel DualBoot.Sm8150.cfg Output/ShellCode/ShellCode.Epsilon.bin
    ```
  - Notice 
    + Shell Code binaries can be find under `output/ShellCode/`
  
## See More
  - You can go to our document page to get more infomation about the Dual Boot Patcher.

## License
  MIT License.