# SDL2

## Preparation

```bash
# Install X11 miscellaneous extensions library (development headers)
$ sudo apt-get install libxext-dev
```

## Download and Build SDL2

```bash
# Download SDL2
$ wget https://www.libsdl.org/release/SDL2-2.0.9.tar.gz -O SDL2-2.0.9.tar.gz

# Unpack SDL2-2.0.9.tar.gz file
$ tar -xvzf SDL2-2.0.9.tar.gz

# Go to the SDL directory
$ cd SDL2-2.0.9/

# Create build folder
$ mkdir build

# Go to build folder
$ cd build

# Run configure script from build folder
$ ../configure

# Run make script
$ make
```

### Install

You can install the SDL version you built with the following command from the *build* folder.

```bash
$ sudo make install
```

I have personally never used this option though.

### Notes

The shared object files can be found at *SDL2-2.0.9/build/build/.libs/*. 

The following Stackoverflow explain the interesting file types: https://stackoverflow.com/questions/12237282/whats-the-difference-between-so-la-and-a-library-files

## lala



## Resources

[SDL Projects](https://www.libsdl.org/projects/)

[SDL Image](https://www.libsdl.org/projects/SDL_image/)
