Introduction
------------
Zipios++ is a small C++ library for reading zip files. The structure
and public interface are based (somewhat loosely) on the java.util.zip
package. The streams created to access the individual entries in a zip
file are based on the standard iostream library.

Zipios++ also provides a way for an application to support files from
multiple sources (e.g. from zip files or from ordinary directories)
transparently.

The source code is released under the GNU Lesser General Public
License.

Dependencies
------------
Requires zlib (http:://www.zlib.org). To run the automatic unit test
suite you need CppUnit (http://cppunit.sourceforge.net)


Installation (Unix)
-------------------
This software package uses autoconf/automake, so the fast installation
procedure is

./configure
make
make install

For details about installation of autoconfiscated packages refer to
the INSTALL file

'make install' installs the Zipios++ header files under
/usr/include/zipios++/ and the library libzipios.a under
/usr/lib/. You can choose another base path than /usr/ by using the
--prefix switch with configure. See the INSTALL file for
details. Running make also builds a number of test programs that
remain in the source directory zipios++/. The built example binaries
and the corresponding source code have names that start with test_ and
example_. These test programs demonstrate the most important features
in Zipios++.

Installation (Windows)
----------------------
Currently, makefiles are only provided for Visual C++, along with a
Developer Studio project. It is also planned to support Inprise and Gnu
compilers in the near future.

Before building, if zlib is not in a standard compiler path, the location of
its headers and .lib file must be defined at the top of win32\Makefile.com

To install, using the appropriate make program and one of the following
makefiles:
	Makefile.vc	- Visual C++ 5, 6 and 7

the procedure (for Visual C++) is
cd win32
nmake -f Makefile.vc

To use the Developer Studio project, run configure.bat from win32 before
compiling. Again, a non-standard location for zlib must be defined in the
project settings before building.

No install options have been defined yet.

Status and Documentation
------------------------
Please refer to the online documentation at
http://zipios.sourceforge.net. A printable version of the online
documentation is also available at the same URL. The documentation can
be automatically generated from the source if you have Doxygen
installed by running

./configure
make doc


Bugs
----
Submit bug reports and patches to thomass@deltadata.dk 

Contributing
------------
If you're interested in helping with Zipios++ then drop me a note at
thomass@deltadata.dk.

