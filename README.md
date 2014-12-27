propfont-mixed
==============

Enable use of variable-width fonts for displaying symbols,
in a way that does not conflict with fixed-width-space-based
indentation.

Screenshot
----------

Here is an example: it is a C-file in emacs source, which uses mixed
space/tab indentation. Short words, special symbols, and those words
that are judged to be anchors for other lines' indentation are
displayed with the default font, other words are displayed with the
variable-width font. Note that the indentation looks correct, unlike
what it would be if I enabled the `variable-pitch-mode` instead.

![Screenshot example](screenshot.png?raw=true "Screenshot")

Notes
-----

- Customize `propfont-mixed-inhibit-regexes` to forbid some
  symbols from being shown with proportional fonts. See also
  `propfont-mixed-inhibit-function`, and `propfont-mixed-inhibit-faces`.

- It is probably necessary to adjust the face `variable-pitch`,
  so that the proportional font looks good and is the correct size.
