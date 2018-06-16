---
layout: post
title:  "OpenSCAD Building on macOS"
permalink: /:title
date:   2018-06-10 00:00:00
author: LI Tao
images:
  - assets/images/OpenSCAD/OpenSCAD.jpg
excerpt:
  "The goal is that it will describe how to set up a functional development environment for OpenSCAD on macOS."

categories: [OpenSCAD]
tags: [OpenSCAD]
---

[//]: # (Image References)
[image1]: assets/images/OpenSCAD/OpenSCAD_Welcome.png "OpenSCAD Welcome"


OpenSCAD is a software for creating solid 3D CAD objects. It is free software and available for Linux/UNIX, MS Windows and Mac OS X.

Unlike most free software for creating 3D models (such as the famous application Blender), OpenSCAD focuses on the CAD aspects rather than the artistic aspects of 3D modeling. Thus this might be the application you are looking for when you are planning to create 3D models of machine parts but probably not the tool for creating computer-animated movies.

OpenSCAD is not an interactive modeler. Instead it is more like a 3D-compiler that reads a script file that describes the object and renders the 3D model from this script file (see examples below). This gives you, the designer, complete control over the modeling process and enables you to easily change any step in the modeling process or make designs that are defined by configurable parameters.

OpenSCAD provides two main modeling techniques: First there is constructive solid geometry (aka CSG) and second there is extrusion of 2D outlines. As the data exchange format for these 2D outlines Autocad DXF files are used. In addition to 2D paths for extrusion it is also possible to read design parameters from DXF files. Besides DXF files OpenSCAD can read and create 3D models in the STL and OFF file formats.

To build OpenSCAD from source, follow the instructions for the platform applicable to you below.

**Getting the source code**  
Install git (http://git-scm.com/) onto your system. Then run a clone:

    git clone git://github.com/openscad/openscad.git

This will download the latest sources into a directory named `openscad`.

To pull the MCAD library (https://github.com/openscad/MCAD), do the following:

    cd openscad
    git submodule update --init

**Prerequisites**  
To build OpenSCAD, you need some libraries and tools. The version
numbers in brackets specify the versions which have been used for
development. Other versions may or may not work as well.

If you're using a newer version of Ubuntu, you can install these 
libraries from aptitude. If you're using Mac, or an older Linux/BSD, there 
are build scripts that download and compile the libraries from source. 
Follow the instructions for the platform you're compiling on below.

* A C++ compiler supporting C++11
* [Qt (4.4 -> 5.x)](http://qt.io/)
* [QScintilla2 (2.7 ->)](http://www.riverbankcomputing.co.uk/software/qscintilla/)
* [CGAL (3.6 ->)](http://www.cgal.org/)
* [GMP (5.x)](http://www.gmplib.org/)
* [MPFR (3.x)](http://www.mpfr.org/)
* [cmake (2.8 ->, required by CGAL and the test framework)](http://www.cmake.org/)
* [boost (1.35 ->)](http://www.boost.org/)
* [OpenCSG (1.3.2 ->)](http://www.opencsg.org/)
* [GLEW (1.5.4 ->)](http://glew.sourceforge.net/)
* [Eigen (3.x)](http://eigen.tuxfamily.org/)
* [glib2 (2.x)](https://developer.gnome.org/glib/)
* [fontconfig (2.10 -> )](http://fontconfig.org/)
* [freetype2 (2.4 -> )](http://freetype.org/)
* [harfbuzz (0.9.19 -> )](http://harfbuzz.org/)
* [Bison (2.4 -> )](http://www.gnu.org/software/bison/)
* [Flex (2.5.35 -> )](http://flex.sourceforge.net/)
* [pkg-config (0.26 -> )](http://www.freedesktop.org/wiki/Software/pkg-config/)

Homebrew (assumes [Homebrew](https://brew.sh/) is already installed)

        ./scripts/macosx-build-homebrew.sh

**Compilation**  
First, run `qmake openscad.pro` from Qt to generate a Makefile.
Then run `make`. Finally you might run `make install` as root or simply copy the
'openscad' binary (`OpenSCAD.app` on Mac OS X) to the bin directory of your choice.

	qmake openscad.pro
	make

If you had problems compiling from source, raise a new issue in the
[issue tracker on the github page](https://github.com/openscad/openscad/issues).
	
ld: library not found for -lqscintilla2
clang: error: linker command failed with exit code 1 (use -v to see invocation)
make: *** [OpenSCAD.app/Contents/MacOS/OpenSCAD] Error 1

change the line -lqscintilla2 to -lqscintilla2_qt5, rerun the command.

![alt text][image1]

prebuilt image: [OpenSCAD.app](assets/uploads/OpenSCAD.zip) 

**reference**  
* [Building OpenSCAD from Sources](http://en.wikibooks.org/wiki/OpenSCAD_User_Manual/Building_OpenSCAD_from_Sources)
