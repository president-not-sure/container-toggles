# container-toggles

It's a bash script wrapper on the podman command line. It enables easy toggling of common podman arguments.
It does so by accumulating arguments in 2 arrays, then combines them with the default ones and finally inserts them in the final command and executes it.
It lives in your `~/bashrc.d`.

> [!WARNING]
> Fully functional, just need to add documentation and maybe a nice demo gif.

## Requirements

- linux
- a relatively recent version of bash
- podman

## Installation

```bash
git clone https://github.com/president-not-sure/container-toggles.git
mkdir --parents ~/.bashrc.d
cp --recursive --force container-toggles/ct container-toggles/ct-launcher ~/.bashrc.d/
rm --recursive --force container-toggles
```

## Usage

```bash
ct [ct|toggle|option]... container|command [container_command_line]
```
