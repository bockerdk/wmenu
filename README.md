# About

This is a fork of [wmenu](https://codeberg.org/adnano/wmenu) with a broader scope than just feature parity with dmenu.

Changes from upstream:

- EditorConfig support
- Option to center the menu
- Option to set the menu width

# wmenu

wmenu is an efficient dynamic menu for Sway and wlroots based Wayland
compositors. It provides a Wayland-native dmenu replacement which maintains the
look and feel of dmenu.

## Installation

Dependencies:

- cairo
- pango
- wayland
- xkbcommon
- scdoc (optional)

```
$ meson setup build
$ ninja -C build
# ninja -C build install
```

## Usage

See wmenu(1)

To use wmenu with Sway, you can add the following to your configuration file:

```
set $menu wmenu-run
bindsym $mod+d exec $menu
```
