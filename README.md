

![Demo](https://raw.githubusercontent.com/camccar/RustTetris/master/src/assets/demo.jpg)

# Rust Tetris

This app aims to be a complete low level Tetris clone written in Rust and SDL2. It should have
Scoring and game play similar to the NES version of the game. The code is based off of the 
typescript Tetris prototype I've previously written.Only with better game logic more consistent with the nes version of the game. You can see that version here [TypeScript Tetris](https://camccar.github.io/tetris/) 

## Download for Windows

Version 1.0 is now available for windows 10 64bit. You can download it [here](https://github.com/camccar/RustTetris/releases/download/1.02/rust-tetris-release-1.zip). or find it in the [release section](https://github.com/camccar/RustTetris/releases).
Unzip the file rust-tetris-release-1.zip click into the folder and double click on rusttetris.exe

## Getting Started

Currently Ubuntu 18.04 and Windows are supported. Because thats what I'm testing on.

### Prerequisites

You will need the latest stable version of rust. You will also need sdl2 and sdl2-ttf development libraries  if you are on ubuntu. which you can install with.

```
sudo apt-get install libsdl2-dev
```

```
sudo apt-get install libsdl2-ttf-dev
```

```
sudo apt-get install libsdl2-image-dev

```

Windows users may use the build.rs script in the main directory and the included sdl libraries.


### Installing

To build and run the project, cd into the root directory and type 

```
cargo run
```

Cargo will go out and gather the needed dependencies, build and launch tetris.

## Controlls

### Keyboard

Use the left, right, and down arrow keys for navigation.
The up key rotates the piece. The space bar lands the piece at the bottom.
The r key resets the board. Press enter to pause the game. Esc exits the game.

### Gamepad
SDL Gamepad support. Most gamepads should work. The xbox buttons should be the following,
a,b,up are change piece state.
x and y are drop piece.
up, down, left, right behave exactly as the keyboard does.
Sholder buttons should move the piece either one space to the left or one space to the right.

## Resolution and fullscreen

The default resolution is set to 720 windowed; However you may change this along with the fps in the src/assets/jata.json file.

### Built With

* [Rust](https://www.rust-lang.org/en-US/) - Programming Language
* [Rust SDL](https://github.com/Rust-SDL2/rust-sdl2) - The Graphics Library wrapper written in rust
* [SDL2](https://www.libsdl.org/download-2.0.php) - C library rust wrapper uses



### Authors

* **Caleb McCarthy** - [Web Site](http://calebmccarthy.io)
.

### Acknowledgments

* [Colin Fahey's great Tetris documentation](https://www.colinfahey.com/tetris/tetris.html)
* [The Tetris Wiki](http://tetris.wikia.com/wiki/Tetris_Wiki)

