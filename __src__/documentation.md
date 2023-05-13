# ⭕ dank.tool documentation ( for devs ) ⭕

## ⭕ Introduction ⭕

- dank.tool is a collection of tools that I have created to automate / simplify various tasks. I have decided to share them with the world in hopes that they will make your life easier as well.
- dankware is a python package that is used by dank.tool to perform various tasks. It is also available for use in your own projects. You can find it [here](https://github.com/SirDank/dankware).
- dankware is also what I call software made by me. I have decided to use this name because it is a combination of my name and the word software. I think it sounds cool and I hope you do too. (totally not written by github copilot lmfao)

## ⭕ File Structure ⭕

```
📁 dank.tool/
├─📄 dank.tool.exe                       [ direct download to the latest dank.tool installer ]
├─📄 dank.tool.zip                       [ direct download to the latest dank.tool installer inside a zip ]
├─📄 README.md                           [ modules documentation ]
├─📁 __assets__/                         [ assets used by dank.tool's modules ]
│ ├─📁 example_module_1/
│ │ ├─📄 example_file_1.mp3
│ │ └─📄 example_file_2.mp3
│ ├─📁 example_module_2/
│ │ ├─📄 example_file_1.exe
│ │ └─📄 example_file_2.exe
│ └─📁 example_module_3/
│   ├─📄 example_file_1.jar
│   ├─📄 example_file_2.xml
│   └─📄 example_file_3.png
├─📁 __modules__/                        [ src for dank.tool's modules ]
│ ├─📄 example_module_1.py
│ ├─📄 example_module_2.py
│ ├─📄 example_module_3.py
│ └─📁 __wip__/                          [ modules that are still being worked on ]
│   └─📄 example_module_1.py
├─📁 __src__/
│ ├─📄 checksums.txt                     [ checksums for different versions of the dank.tool ( not being used / updated anymore ) ]
│ ├─📄 dank.tool.py                      [ dank.tool's interface + module executor ]
│ ├─📄 documentation.md
│ ├─📄 executor.py                       [ dank.tool's main src ( imports, update checker ( executes updater.py ), discord rpc, online run counter, chatroom user validator, executes dank.tool.py ) ]
│ ├─📄 executor_version.txt              [ dank.tool's latest version ( used for update checks ) ]
│ ├─📄 requirements.txt                  [ python packages required to build dank.tool.exe ]
│ └─📄 updater.py                        [ dank.tool's updater ]
└─📁 __tools__/
  └─📄 package-updater.cmd               [ script I use to quickly update all packages used by the dank.tool before I build the latest version ]
```

## ⭕ Build Process ⭕

- dank.tool is built using [nuitka](https://github.com/Nuitka/Nuitka) and [innosetup](https://jrsoftware.org/isinfo.php) by a custom python executable builder designed by me which is not available to the public. ( It is an advanced tool that automates the entire build process for any executable that I produce )
- in short the dank.init.py script is added on top of the executor.py script and then the entire thing is compiled into a executable with multiple c code source files using nuitka ( standalone mode not onefile mode ), after which the final dank.tool installer is built using innosetup which is a single executable.

## ⭕ dank.init.py ⭕

## ⭕ executor.py ⭕

## ⭕ dank.tool.py ⭕
