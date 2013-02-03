# YOURLS .POT FILE FOR TRANSLATIONS

This is the official YOURLS .pot file to generate and maintain your own translations.

## Source keywords

YOURLS uses the following set of functions to translate strings:

* `yourls__`
* `yourls_e`
* `yourls_esc_attr__`
* `yourls_esc_html__`
* `yourls_x`
* `yourls_ex`
* `yourls_esc_attr_x`
* `yourls_esc_html_x`
* `yourls_n`
* `yourls_nx`

If you want to generate a .pot file for YOURLS, you'll need to configure your software (eg PoEdit) with these strings

![poedit keywords](https://raw.github.com/yourls/yourls/screenshots/poedit-strings.png)

### Awesome! How do I create my own translations?

TODO: add info here

### This .POT file is incomplete, I want to contribute!

First, as of 1.6-alpha, YOURLS needs more translatable strings. Basically there are hardcoded English strings all over the place, they need to be replaced with their equivalent translation aware function:

* `echo()` &rarr; `yourls_e()`
* `return()` &rarr; `yourls__()`
* ... and all functions from the above **Source Keyword** list. More info to come.

You can contribute in doing this, check http://code.google.com/p/yourls/

Then, generate a new .pot file and make a pull request to this repo here

#### Thanks to
[LeoColomb](https://github.com/LeoColomb) - L10n was a low priority feature but he threw his patch at my face :)


#### License
Do whatever the hell you want with it.