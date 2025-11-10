# Pacmund - An Edinburgh MUN-themed Pacman Clone
![Build](https://github.com/bobbylight/PacmanJS/actions/workflows/build.yml/badge.svg)
![CodeQL](https://github.com/bobbylight/PacmanJS/actions/workflows/codeql-analysis.yml/badge.svg)
[![codecov](https://codecov.io/gh/bobbylight/PacmanJS/branch/master/graph/badge.svg?token=1AzwBREy4R)](https://codecov.io/gh/bobbylight/PacmanJS)

A custom fork of PacmanJS featuring Edinburgh Model United Nations mascot and themed sprites. The game mechanics remain authentic to the original Pacman while presenting a unique EdMUN visual style.

Licensed under [an MIT license](LICENSE.txt).

## Hacking
To install, compile, and run locally:

```bash
git clone https://github.com/UnneededHere/Pacmund.git
cd Pacmund
npm install
npm run dev  # Start dev server at localhost:5173, hot deploy changes
npm run build  # Production build into dist/
```

## Electron Support
*Note: This was removed and needs to be re-added, see https://github.com/bobbylight/PacmanJS/issues/17.*

Besides browser support, a native version of the game can be built using
electron.  See the `build:electron`, `dist:electron` and other related tasks below.


## npm scripts

* `clean`: Deletes prior build artifacts
* `dev`:   Runs a dev server on http://localhost:5173 and hot-deploys changes
* `build`: Builds production artifact into `dist/`
* `serve`: Runs the built app on http://localhost:4173
* `lint`: Lints the project
* `test`: Runs unit tests and generates coverage report in `coverage/`


## What's unimplemented/buggy
Relatively in the order in which I want to fix things:

* Sound effects don't always stop/restart properly when the game is paused
* Intermissions are not yet implemented
* Ghost AI is approximate to, but not exactly, the actual algorithms
* Custom sprite animations may need refinement
* Blinky does not turn into Cruise Elroy, or increase in speed, as a level
  goes on
