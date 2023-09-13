# Zeal

Zeal is a simple offline documentation browser inspired by [Dash](https://kapeli.com/dash).

![Screenshot](https://i.imgur.com/qBkZduS.png)

## Download

Get binary builds for Windows and Linux from the [download page](https://zealdocs.org/download.html).

## How to use

After installing Zeal go to `Tools->Docsets`, select the ones you want, and click the `Download` button.

## How to compile

### Build dependencies

* [CMake](https://cmake.org/).
* [Qt](https://www.qt.io/) version 5.9.5 or above. Required module: Qt WebEngine Widgets.
* [libarchive](https://libarchive.org/).
* [SQLite](https://sqlite.org/).
* X11 platforms only: Qt X11 Extras and `xcb-util-keysyms`.

### Build instructions

```sh
cmake -B build
cmake --build build
```

More detailed instructions are available in the [wiki](https://github.com/zealdocs/zeal/wiki).

## Query & Filter docsets

You can limit the search scope by using ':' to indicate the desired docsets:

`java:BaseDAO`

You can also search multiple docsets separating them with a comma:

`python,django:string`

## Command line

If you prefer, you can start Zeal with a query from the command line:

`zeal python:pprint`

## Create your own docsets

Follow instructions in the [Dash docset generation guide](https://kapeli.com/docsets).


## License

This software is licensed under the terms of the GNU General Public License version 3 (GPLv3). Full text of the license is available in the [COPYING](LICENSE.md) file and [online](https://www.gnu.org/licenses/gpl-3.0.html).
