# lutris-runtime fork
This is a fork of the icons repository for Lutris with a few fixes and changes.

* Several icon names have been fixed to match what Lutris expects them to be.
    * This includes a workaround for a bug with "Game Boy/Game Boy Color". The sidebar in Lutris renders icons using GTK's built-in icon system, and thus expects `gameboy_gameboycolor-symbolic.svg`. The platform badges in the grid view, however, use custom code that does not filter out any characters except spaces, and thus it expects the file to be named `gameboy/gameboycolor-symbolic.svg`. Thus, this repository includes the same icon at both paths.
* The nominal size of several SVG icons has been changed to 128x128. This works around an issue where icons with a large nominal size will be scaled down poorly and appear somewhat pixelated.
* Whitespace has been cropped out of some icons so they appear as large as possible.
* Some missing icons have been added (Xbox, Ryujinx, etc).
* Some icons have been changed out according to my personal preferences. For the symbolic (monochrome) icons, I tend to prefer having it be solid white/black (whereas some of Lutris's default icons have a few shades of gray).

Of the new icons, many of them come from (or are derived from) [Dan Patrick's console logos collection](https://archive.org/details/console-logos-professionally-redrawn-plus-official-versions/9-2%20-%20Logo%20Image%20-%20Various%20Sega.jpg).