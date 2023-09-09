# JUCE CMake Plugin Template

Configurable base template for a JUCE audio plugin using CMake

## Requirements

- git 2.13+
- cmake 3.15+

## Getting Started

#### 1. Recursively clone this repo
`git clone --recurse-submodules https://github.com/tadashibashi/juce-cmake-plugin-template`

#### 2. Run customary mkdir build && cd build && cmake .. && cmake --build

## Project Structure

```
/
├─ lib/                    # Submodule dependencies
│  └─ JUCE/
├─ src/                    # Plugin boilerplate code
│  ├─ PluginEditor.cpp
│  ├─ PluginEditor.h
│  ├─ PluginProcessor.cpp
│  └─ PluginProcessor.h
├─ CMakeLists.txt          # Build configurations
└─ ReadMe.md               # This file
```

## How to Use

- CMakeLists.txt is where you can configure the project --
project name, manufacturer, plugin type, compile defs etc.
- When adding, removing, or renaming source files, please make sure to 
update them in CMakeLists.txt `target_sources` command (file glob not used)
