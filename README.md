Simple Monitor for Plasma
=========================

A simple monitor for plasma, completely written in QML and Javascript.

Installation using CMake
========================

Having root permission:

````Shell
git clone https://github.com/dhabyx/plasma-simpleMonitor.git plasma-simpleMonitor
mkdir build
cd build
cmake -DCMAKE_INSTALL_PREFIX=`kde4-config --prefix` -DCMAKE_BUILD_TYPE=Release  -DKDE_INSTALL_USE_QT_SYS_PATHS=ON ../
make
make install
````

Having non-root permission:

````Shell
git clone https://github.com/dhabyx/plasma-simpleMonitor.git plasma-simpleMonitor
mkdir build
cd build
cmake -DCMAKE_INSTALL_PREFIX=`kde4-config --localprefix` -DCMAKE_BUILD_TYPE=Release  -DKDE_INSTALL_USE_QT_SYS_PATHS=ON ../
make
make install
````

Packaging
=========

Simple way for make plasmoid package:

````Shell
$ git clone https://github.com/dhabyx/plasma-simpleMonitor.git plasma-simpleMonitor
$ cd plasma-simpleMonitor/plasmoid
$ zip -r plasma-simpleMonitor.plasmoid contents metadata.desktop
````

Installation
------------

In KDE you can use asistant for installation.

In a terminal you can use plasmapkg command:
````Shell
$ plasmapkg2 -i plasma-simpleMonitor.plasmoid
````

If you want update:
````Shell
$ plasmapkg2 -u plasma-simpleMonitor.plasmoid
````

Development
===========

Use launch.sh script to launch and debug plasma-simpleMonitor plasmoid without install it.

If you love QtCreator IDE visit the [wiki](https://github.com/dhabyx/plasma-simpleMonitor/wiki) for more details.

License
=======
Simple Monitor for Plasma is licensed under the GNU General Public License Version 3 or later.

You can modify or/and distribute it under the conditions of this license.
