# wf-mod2key

[xcape] style "press modifier on its own to press another key combo" plugin for [Wayfire].
This makes it possible to do the "Control/Escape" and "Shift Parentheses" sections of the legendary blog post, [A Modern Space Cadet].

(Currently only has fixed ctrl-esc and shifts-parens support, TODO: lshift/rshift bindings in wf-config - that would allow flexibility)

[xcape]: https://github.com/alols/xcape
[Wayfire]: https://github.com/WayfireWM/wayfire
[A Modern Space Cadet]: https://stevelosh.com/blog/2012/10/a-modern-space-cadet/

## Alternatives

It is possible to do this on other levels, such as

- in the keyboard itself, with custom firmware like [QMK](https://qmk.fm/)
- on the evdev level, having a daemon write events into a virtual (`uinput`) device, with e.g.:
	- my own [evscript](https://github.com/myfreeweb/evscript)
	- [evdevremapkeys](https://github.com/philipl/evdevremapkeys)
	- [Interception Tools](https://gitlab.com/interception/linux/tools) possibly with [interception-k2k](https://github.com/zsugabubus/interception-k2k)
	- others..

But of course having this in the display server is the least intrusive way.
The only benefit of the other methods is that they can work outside of that display server :)

## License

This is free and unencumbered software released into the public domain.  
For more information, please refer to the `UNLICENSE` file or [unlicense.org](https://unlicense.org).
