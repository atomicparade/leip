# leip

[![MIT License](https://img.shields.io/badge/license-MIT-blue)](https://choosealicense.com/licenses/mit/)

Lists explicitly installed [pacman](https://wiki.archlinux.org/title/Pacman)
packages that are not dependencies of other packages, along with the install
date and size.

Note that the install date listed is the date that the package was last updated;
it may not be the date that the package was originally instaleld onto the sytem.

Requires [expac](https://github.com/falconindy/expac) (`# pacman -S expac`).

## Usage

```
leip [OPTION]

Options:

  -i, --sort-by-install-date    Sort by install date (default)
  -s, --sort-by-size            Sort by size in MiB
  -n, --sort-by-name            Sort by name
  -h, --help                    Show this help text
      --version                 Show program version
```

## Example output

```
Installed	Size    	Package name
2020-02-23	  0.00 MiB	base
2020-05-30	  0.14 MiB	xfce4-mpc-plugin
2020-05-30	  0.37 MiB	xfce4-pulseaudio-plugin
2020-05-30	  3.43 MiB	xfwm4-themes
2020-05-30	  9.82 MiB	xfce4-artwork
2020-06-04	  0.19 MiB	patch
2020-06-04	  0.95 MiB	flex
2020-06-04	  1.52 MiB	make
2020-06-06	  0.17 MiB	bc
```
