# YOURLS .POT FILE FOR TRANSLATIONS

This is the official YOURLS .pot file to generate and maintain your own translations.

### Awesome! How do I create my own translations?

To create translation files:

1. Download the translation file template YOURLS.pot  
2. Rename it to `[your-locale].po`, where `[your-locale]` is typically `language code, underscore, country code` (for instance in Portugal that would be `pt_PT`, while in Brazil it’d be `pt_BR`).  
3. Install a translation software: it’s nothing more than a text editor capable of reading `.po` files, showing you the untranslated string and a text box where you type in the translation, and saving a `.mo` file which is what PHP needs. A cross platform, simple yet complete editor is [Poedit](http://www.poedit.net/).  
4. Once you have your fully translated `pt_BR.po` and the generated `pt_BR.mo`, host them somewhere (preferably on a source control enabled environment such as Github or Google Code to make contributions easier) and ping me! I’ll maintain a list of available translations.  

To check your translation file and load it in YOURLS:

1. Download a nightly build or update via SVN. [Read this](http://code.google.com/p/yourls/wiki/InstallFromSVN)
2. Drop your `pt_BR.po` and `pt_BR.mo` files in `user/languages`
3. Add `define( 'YOURLS_LANG', 'pt_BR' )` to your `config.php`
4. That’s it! Play with YOURLS

See the [related blog post](http://blog.yourls.org/2013/02/yourls-1-6-translators-wanted/)

## How to generate a .po/.pot file ?

You mostly don't need to do that.

If you want to generate a `.pot` file for YOURLS, you'll need to configure your software (eg PoEdit) with these strings, which are the functions used in YOURLS translation API

* `yourls__`
* `yourls_e`
* `yourls_s`
* `yourls_se`
* `yourls_esc_attr__`
* `yourls_esc_html__`
* `yourls_x`
* `yourls_ex`
* `yourls_esc_attr_x`
* `yourls_esc_html_x`
* `yourls_n:1,2`
* `yourls_nx:1,2`
* `yourls_n_noop:1,2`
* `yourls_nx_noop:1,2`

![poedit keywords](https://raw.github.com/yourls/yourls.pot/screenshots/poedit-strings.png)

Configure also the parser to include comments for translators. In Poedit: File, Preferences, Parsers, PHP : edit and in the `Parser command` add parameter `--add-comments=/`


#### Thanks to
[LeoColomb](https://github.com/LeoColomb) - L10n was a low priority feature but he threw his patch at my face :)


#### License
Do whatever the hell you want with it.

[![githalytics.com alpha](https://cruel-carlota.pagodabox.com/51e281a952f55ec59467afad65496246 "githalytics.com")](http://githalytics.com/YOURLS/YOURLS.pot)
