# Xcode Template for Raylib Projects

This is a fork of the original [Xcode Template for Raylib](https://github.com/acejacek/raylib_xcode). This fork allows for a more customizable installation.

This is a simple project template for usage within Xcode. It simplifies the steps needed to perform when starting new project. For details, see [Working on macOS](https://github.com/raysan5/raylib/wiki/Working-on-macOS) from official raylib documentation.

## Prerequisite

Install raylib with Homebrew method

- if [Homebrew](https://brew.sh) is not installed, run:

```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

- install raylib:

```
brew install raylib
```

## Instalation of Xcode project template

The easiesst method to install the template is, in this directory, run:

```
chmod +x install.sh
./install.sh
```

From now on, when creating new project, it's possible to select raylib (in macOS platform, scroll down to see it at the bottom of the list). Such created new project will have a link to `libraylib.a` and pre-set search paths to headers and library files. Additionally, it will disable library validations, preventing linking the unsigned raylib.

As mentioned in [Working on macOS](https://github.com/raysan5/raylib/wiki/Working-on-macOS), you may need to add additional frameworks to your project:

- OpenGL.framework
- CoreVideo.framework
- IOKit.framework
- Cocoa.framework
