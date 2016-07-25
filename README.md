See: http://mupuf.org/project/arduide/

Dependencies:

Arduide depends on the following projects:

* [QScintilla2] - Qt port of Scintilla.
* [Grantlee] - A library to separate structure of documents from the data they contain.
* [Libudev] - Allows access to device information.
* [Qt4/Qt5] - Cross-platform application framework.
* [cmake] - Manage build process.
* [Doxygen] - Documentation generator
    
Debian-based (qt4)
```sh
  sudo apt-get install libqscintilla2-dev libudev-dev libgrantlee-dev libgrantlee-core0 qt4-qmake cmake git
```
Debian-based (qt5) - TODO
```sh
  sudo apt-get install libqscintilla2-dev libudev-dev qt5-qmake cmake git
  
  sudo dpkg -i libgrantlee5-dev_5.1.0-1_amd64.deb libgrantlee-templates5_5.1.0-1_amd64.deb libgrantlee-textdocument5_5.1.0-1_amd64.deb
```
Installation
```sh
  $ git clone https://git.gitorious.org/arduide/arduide.git 
  $ cd arduide && mkdir build && cd build
  $ cmake -DCMAKE_INSTALL_PREFIX=/usr -DUSE_FHS_PATHS=ON -DCMAKE_BUILD_TYPE=Release ..
  $ make
  $ make install
```

## Links

[QScintilla2]: http://www.riverbankcomputing.co.uk/software/qscintilla/intro
[Grantlee]: https://github.com/steveire/grantlee
[Libudev]: http://www.freedesktop.org/software/systemd/libudev/
[Qt4/Qt5]: https://qt.digia.com/
[cmake]: http://www.cmake.org/
[Doxygen]: http://www.stack.nl/~dimitri/doxygen/
