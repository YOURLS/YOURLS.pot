# YOURLS .POT FILE FOR TRANSLATIONS

This is the official YOURLS .pot file to generate and maintain your own translations.

## Awesome! How do I create my own translations?

To create translation files:

1. Download the translation file template `YOURLS.pot`  
2. Rename it to `[your-locale].po`, where `[your-locale]` is typically `language code, underscore, country code` (for instance in Portugal that would be `pt_PT`, while in Brazil it’d be `pt_BR`).  
3. Install a translation software: it’s nothing more than a text editor capable of reading `.po` files, showing you the untranslated string and a text box where you type in the translation, and saving a `.mo` file which is what PHP needs. A cross platform, simple yet complete editor is [Poedit](http://www.poedit.net/).  
4. Translate all the strings. You'll have a fully translated `pt_BR.po` and the generated `pt_BR.mo`

To check your translation file and load it in YOURLS:

1. Download a nightly build or update via SVN. [Read this](http://code.google.com/p/yourls/wiki/InstallFromSVN)
2. Drop your `pt_BR.po` and `pt_BR.mo` files in `user/languages`
3. Add `define( 'YOURLS_LANG', 'pt_BR' )` to your `config.php`
4. That’s it! Play with YOURLS to check everything is fine

For more details, tips and screenshots, see the [related blog post](http://blog.yourls.org/2013/02/workshop-how-to-create-your-own-translation-file-for-yourls/)

## Awesome! How do I update my translation file?

When the `YOURLS.pot` template file is updated with new or modified strings to translate, you don't have to start over your translation file.

1. Download the translation file template `YOURLS.pot`  
2. Put it in the same directory as your translation file, *eg* `pt_BR.po`  
3. In Poedit select **Catalogue** then **Update from POT file**. Now translate only the new strings.

## Awesome! How do I make my translation available to all?

When your translation file is all fine, make sure others can benefit from you hard work!

1. Upload your two `PO` and `MO` files somewhere on the interweb.  
It's best to use a *source control service*, such as Google Code or Github: this will make your changes easy to track, your files easy to maintain, and others' contributions easy to implement. If you don’t want to use SVN or Git, a regular hosting (your blog) will be OK  
2. Make it clear for users: a directory with clearly labelled files (`yourls-1.6-pt_BR.zip` for instance) so they know what to pick.  
3. Ping us! Open a [new issue](https://github.com/YOURLS/YOURLS.pot/issues) here and tell us where your translation lives so we can add it to the [list of available languages](http://yourls.org/translations)   

## What are the available languages already?

See http://yourls.org/translations


#### Thanks to
[LeoColomb](https://github.com/LeoColomb) - L10n was a low priority feature but he threw his patch at my face :)

#### License
Do whatever the hell you want with it.

[![githalytics.com alpha](https://cruel-carlota.pagodabox.com/51e281a952f55ec59467afad65496246 "githalytics.com")](http://githalytics.com/YOURLS/YOURLS.pot)
