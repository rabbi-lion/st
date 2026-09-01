# st

My customized build of [st](https://st.suckless.org/).

This build is used by my Arch Linux and Debian dwm setup and includes the terminal features and keybindings I use daily.

## Installation

Clone the repository:

```sh
git clone https://github.com/rabbi-lion/st.git
cd st
```

Build and install:

```sh
make
sudo make install
```

On a fresh system, the recommended method is to use my post-install script:

```text
https://github.com/rabbi-lion/dwm-install
```

## Features

This build includes:

- scrollback
- mouse scrolling
- keyboard scrollback
- URL opening
- URL copying
- terminal output copying

## Keybindings

```text
Alt+l       open URL
Alt+y       copy URL
Alt+o       copy terminal output
Shift+PgUp  scroll up
Shift+PgDn  scroll down
```

The URL and output actions use helper scripts provided by my dotfiles repository.

## Scrollback

Terminal history can be navigated using the keyboard or mouse.

Keyboard scrolling:

```text
Shift+PgUp  scroll up
Shift+PgDn  scroll down
```

Mouse scrolling is also supported.

## URL handling

URLs displayed in the terminal can be opened or copied using:

```text
Alt+l  open URL
Alt+y  copy URL
```

The helper script is provided by:

```text
https://github.com/rabbi-lion/dotfiles
```

## Output copying

Terminal output can be selected and copied using:

```text
Alt+o
```

The corresponding helper is also provided by the dotfiles repository.

## Configuration

st is configured directly in:

```text
config.h
```

After changing the configuration, rebuild and reinstall:

```sh
sudo make clean install
```

Restart the terminal to use the new build.

## Related repositories

```text
https://github.com/rabbi-lion/dwm-install
https://github.com/rabbi-lion/dotfiles
https://github.com/rabbi-lion/dwm
https://github.com/rabbi-lion/dwmblocks
https://github.com/rabbi-lion/nsxiv
```

## License

This repository retains the original st MIT/X Consortium license.

See `LICENSE` for the full license text.
