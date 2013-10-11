cg2sandbox
=======




Assimp Modifications

assimp/CMakeLists.txt
- ENABLE_BOOST_WORKAROUND was set to ON by default
- disabled the uninstall capability
assimp/code/CMakeLists.txt
- COMPILE_FLAGS "-D_CRT_SECURE_NO_WARNINGS" was added to avoid secure warnings in msvc  
- COMPILE_FLAGS "-D_SCL_SECURE_NO_WARNINGS" was added to avoid secure warnings in msvc  
assimp/code/LWOAnimation.cpp
- #include <functional> was added in order to compile in windows


Qt 5.1.1 Compiling for Visual Studio 2013 RC

- http://qt-project.org/forums/viewthread/32508

set CL=/MP
set QMAKEPATH=C:/Qt/5.1.1.12/qtbase/bin
configure -opensource -confirm-license -nomake examples -nomake tests -opengl desktop -platform win32-msvc2013