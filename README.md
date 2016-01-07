# org.qtmob.material.wrapper
A wrapper to use [qml-material](https://github.com/papyros/qml-material) as a qrc file.

## Usage

1. create a git repo for your app:  
`git init`
2. in your app's repo, add qml-material-qrc as a git submodule:  
`git submodule add https://github.com/maply/org.qtmob.material.wrapper lib/org/qtmob/material/wrapper`
3. navigate to the submodule's folder  
`cd lib/org/qtmob/material/wrapper`
4. download qml-material:  
`git submodule init; git submodule update`
5. in your app's .pro file, add  
`include(lib/org/qtmob/material/wrapper/org_qtmob_material_wrapper.pri)`
7. in your app's main.cpp file, add  
`engine.addImportPath("qrc:/qml-material/modules");`

You can customize the org_qtmob_material_wrapper.qrc file to add/remove components and resources as needed.
For example, for mobile deployment you might want to omit unused fonts and icons.
