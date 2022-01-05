mmm-jinja2 for Emacs
====================

[![License GPL 3][badge-license]][copying]

Add [Jinja2][] tag support into other major modes with [mmm-mode][] in [GNU Emacs][] 24.

This mode has only been tested in GNU Emacs 24. It may **not** work with GNU Emacs 23 and below,
or with other flavors of Emacs (e.g. XEmacs).

Installation
------------

**Manual**

You'll need the following packages:

* python-mode
* [mmm-mode][]

In your .emacs, load the .el:

```el
(load "~/mmm-jinja2.el")
```

Then specify the extensions to use with mmm-jinja2 mode:

```el
(add-to-list 'auto-mode-alist '("\\.jinja2\\'" . html-mode))
(mmm-add-mode-ext-class 'html-mode "\\.jinja2\\'" 'jinja2)
```

**Automatic**

From [MELPA][] or [MELPA Stable][] with <kbd>M-x package-install RET
mmm-jinja2</kbd>.

Usage
-----

Available MMM Mode Insertion Commands:

|   Key     |      Inserts     |
|-----------|:----------------:|
| `C-c % {` |   `mako-{{-}}`   |
| `C-c % #` |   `mako-comment` |
| `C-c % %` |   `mako-{%-%}`   |

(Use `C-c % h` to show this help message when in mmm-jinja2 mode)

Support
-------

Feel free to ask question or make suggestions in the [issue tracker][].

This package was originally authored by Ben Hayden; the current maintainer is Glynn Forrest.

Contribute
----------

- [Issue tracker][]
- [Github][]

Contributors
------------

- [Ben Hayden](https://github.com/deybhayden)
- [Glynn Forrest](https://github.com/glynnforrest)
- [Mandar Vaze](https://github.com/mandarvaze)

License
-------

mmm-jinja2 is free software: you can redistribute it and/or modify it under the
terms of the GNU General Public License as published by the Free Software
Foundation, either version 3 of the License, or (at your option) any later
version.

mmm-jinja2 is distributed in the hope that it will be useful, but WITHOUT ANY
WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
PARTICULAR PURPOSE.  See the GNU General Public License for more details.

See [`COPYING`][copying] for the complete license.

[badge-license]: https://img.shields.io/badge/license-GPL_3-green.svg
[COPYING]: https://github.com/glynnforrest/mmm-jinja2/blob/master/COPYING
[GNU Emacs]: https://www.gnu.org/software/emacs/
[MELPA]: https://melpa.org/
[MELPA Stable]: https://stable.melpa.org/
[Issue tracker]: https://github.com/glynnforrest/mmm-jinja2/issues
[Github]: https://github.com/glynnforrest/mmm-jinja2
[Jinja2]: http://jinja.pocoo.org/
[mmm-mode]: https://github.com/purcell/mmm-mode
