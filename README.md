# Hello World VST 3

[![CMake (Linux, macOS, Windows)](https://github.com/dirkarnez/vst3_example_plugin_hello_world/actions/workflows/cmake.yml/badge.svg)](https://github.com/dirkarnez/vst3_example_plugin_hello_world/actions/workflows/cmake.yml)

## Introduction

Hello World VST 3 is a simple FX plug-in which was generated by the VST 3 Project Generator. It shows how to use the VST 3 SDK as an external project by using CMake's ```FetchContent``` module.

The file ```external/vst3sdk/CMakeLists.txt``` defines the content population details as well as the command that performs the actual population of the VST 3 SDK.

## Getting Started

To clone and create the project, open a command prompt and proceed as follows:

### Windows

```sh
git clone https://github.com/steinbergmedia/vst3_example_plugin_hello_world.git
mkdir build
cd build
cmake ../vst3_example_plugin_hello_world
cmake --build .
```

### macOS

```sh
git clone https://github.com/steinbergmedia/vst3_example_plugin_hello_world.git
mkdir build
cd build
cmake -GXcode ../vst3_example_plugin_hello_world
cmake --build .
```

### Linux

```sh
git clone https://github.com/steinbergmedia/vst3_example_plugin_hello_world.git
mkdir build
cd build
cmake -DCMAKE_BUILD_TYPE=Debug ../vst3_example_plugin_hello_world
cmake --build .
```

As soon as the project has been successfully built, you will find the plugin bundle in the build folder: ```Debug/VST3/HelloWorld.vst3```

## Getting Help

* Read through the SDK documentation on the **[VST 3 Developer Portal](https://steinbergmedia.github.io/vst3_dev_portal/pages/index.html)**
* Ask some real people in the official **[VST 3 Developer Forum](https://forums.steinberg.net/c/developer/103)**
* Learn more about **[CMake's ```FetchContent``` module](https://cmake.org/cmake/help/latest/module/FetchContent.html)**

