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

* Scripture quotations are from the ESV® Bible, copyright © 2001
  by Crossway, a publishing ministry of Good News Publishers.

## Changelog

### [0.1.0] - 2020-08-07
#### Added
* Initial release

## License

This program is free software; you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.
