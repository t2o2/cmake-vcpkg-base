# CMake VCPKG initial project for Mac
Base project to use CMake and VCPKG

Able to use in vscode

# Prerequisites

```bash
brew install ninja
```

# Usage

Setup Environment Variables

```bash
# Adding to bashrc / zshrc
export VCPKG_ROOT=/path/to/vcpkg
export PATH=$VCPKG_ROOT:$PATH
```

Configure & Build

```bash
cmake --preset=default
cmake --build build
```

Run Application

```bash
./build/HelloWorld

Hello World!
```

# New Environment

## Setup from scratch

Please refer official Micro$oft [vcpkg docs](https://learn.microsoft.com/en-gb/vcpkg/get_started/get-started?pivots=shell-bash)

```bash
git clone https://github.com/microsoft/vcpkg.git
cd vcpkg && ./bootstrap-vcpkg.sh
```

## Basic package usage

```bash
# Setup vcpkg at the project root
vcpkg new --application

vcpkg add port fmt
```