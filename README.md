# qml-material-qrc
A wrapper to use [qml-material](https://github.com/papyros/qml-material) as a qrc file.

## Usage

1. create a git repo for your app:  
`git init`
2. in your app's repo, add qml-material-qrc as a git submodule:  
`git submodule add https://github.com/maply/qml-material-qrc lib/qml-material-qrc`
3. navigate to the submodule's folder  
`cd lib/qml-material-qrc`
4. download qml-material:  
`git submodule init; git submodule update`
5. in your app's .pro file, add  
`include(lib/qml-material-qrc/qml-material-qrc.pri)`
7. in your app's main.cpp file, add  
`engine.addImportPath("qrc:/qml-material/modules");`

You can customize the qml-material-qrc.qrc file to add/remove components and resources as needed.
For example, for mobile deployment you might want to omit unused fonts and icons.
