**InsertESV is an Emacs package for inserting ESV Bible passages.**

## Installation

insert-esv is available from [MELPA](https://melpa.org/#/getting-started).

1. Run `M-x package-install RET insert-esv RET` to install the package.
2. Grab an API key from [Crossway](https://api.esv.org/docs/).
3. Add the API key to your init file:
   `(setq insert-esv-crossway-api-key "<token>")`.

If you don't wish to use MELPA, you can clone this repo and
run `M-x package-install-file RET </path/to/insert-esv.el> RET`.

## Usage

1. Set a keybind in your init file:
   `(global-set-key (kbd "C-x C-e") #'insert-esv-passage)`.
2. Alternatively, run it from the minibuffer:
   `M-x insert-esv-passage RET`.
3. Enter a Bible reference (e.g. "Matthew 6:33") and hit `RET`
   to insert it at cursor point.

## Options

* InsertESV contains support for the optional parameters in
  Crossway's [Passage Text API](https://api.esv.org/docs/passage-text/).
* You can customise these parameters in your init file.
* Make sure to prefix the parameter with "insert-esv", like this:
  `(setq insert-esv-include-headings 'true)`.

## Disclaimer

* InsertESV is licensed under
  [GPLv3](https://github.com/sam030820/insert-esv/blob/master/COPYING).
* Scripture quotations are from the ESV® Bible, copyright © 2001
  by Crossway, a publishing ministry of Good News Publishers.

## Changelog

### [0.1.0] - 2020-08-07
#### Added
* Initial release
