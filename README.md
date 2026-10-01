# Inventory Manager — downloads

Pre-built binaries for **Inventory Manager**, a desktop app for tracking
inventory: sections and subsections, people, check in/out, repair and
write-off, history, multiple organizations and Excel export.

This repository holds **releases only — no source code**. The code lives
in the private repository
[`thatmechguy/inventory_manager_source`](https://github.com/thatmechguy/inventory_manager_source).

## Installing

Grab the archive for your platform from the
[latest release](https://github.com/thatmechguy/inventory_manager/releases/latest):

| Platform | Asset |
| --- | --- |
| Linux | `inventory_manager-<version>-linux-x64.tar.gz` |
| Windows | `inventory_manager-<version>-win64.zip` |

* **Linux** — extract the tarball and run `inventory_manager`, or extract
  it over an existing install; the desktop entry keeps working.
* **Windows** — in the zip's *Properties* tick **Unblock** first, then
  close the app and extract over the previous folder.

Program data lives apart from the executable, so replacing the program
never touches sections, people or organizations:

* Linux — `~/.local/share/com.tmg.inventory_manager/inventory_manager/organizations/`
* Windows — `%APPDATA%\com.tmg\inventory_manager\inventory_manager\organizations\`

An installed build silently checks **this** repository's latest release
and shows an update badge as soon as a newer version appears. The badge
only notifies: the app never replaces its own files.

## For developers

Build instructions, the release procedure and the full feature list live
in the source repository — see `README.md` and `BUILD_WINDOWS.md` there.
