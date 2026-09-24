# st

My customized build of [st](https://st.suckless.org/).

Used by my Arch Linux and Debian dwm setup. Includes the terminal
features and keybindings I use daily.

## Installation

```sh
git clone https://github.com/rabbi-lion/st.git
cd st
make
sudo make install
```

On a fresh system, use my post-install script instead:

```
https://github.com/rabbi-lion/dwm-install
```

## Features

- scrollback
- mouse scrolling
- keyboard scrollback
- URL opening
- URL copying
- terminal output copying

## Keybindings

```
Alt+l       open URL
Alt+y       copy URL
Alt+o       copy terminal output
Shift+PgUp  scroll up
Shift+PgDn  scroll down
```

Scrollback can be navigated with `Shift+PgUp` / `Shift+PgDn` or with
the mouse. The URL and output actions use helper scripts provided by
my dotfiles repository:

```
https://github.com/rabbi-lion/dotfiles
```

## Configuration

st is configured in `config.h`. After changing the configuration,
rebuild and reinstall:

```sh
sudo make clean install
```

Restart the terminal to use the new build.

## License

This repository retains the original st MIT/X Consortium license.
See `LICENSE` for the full license text.
