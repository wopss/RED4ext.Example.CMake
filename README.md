# RED4ext.Example using CMake

An example of a RED4ext plugin using CMake.

## Build instructions

### Requirements

- **[CMake 3.12+](https://cmake.org/)**.

### Steps

1. Download and install
   **[Visual Studio 2022 Community Edition](https://www.visualstudio.com/)** or
   a higher version.
2. Download and install the **[Requirements](#requirements)**.
3. Clone this repository.
4. Create a directory named `build` and generate **[CMake](https://cmake.org/)**
   files in it.
5. Open the solution (**RED4ext.Example.CMake.sln**) located in the `build`
   directory.
6. Build the project (the artifacts are located in `build/src/{debug|release}`
   directory).

**Notes**:

- The plugin has to be a 64-bit library. That means all required libraries have
  to be compiled in 64-bit and the compiler has to support 64-bit.
- Make sure you are using the latest SDK by updating `GIT_TAG` in
  [cmake/deps/RED4extSdk.cmake](cmake/deps/RED4extSdk.cmake).
- You can also generate the project from the command line, see
  [.github/workflows/build.yml](.github/workflows/build.yml).
