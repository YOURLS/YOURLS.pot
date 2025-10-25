# YOURLS `.POT` [![Listed in Awesome YOURLS!](https://img.shields.io/badge/Awesome-YOURLS-C5A3BE)](https://github.com/YOURLS/awesome-yourls/)

[<img src="https://github.com/YOURLS/YOURLS/raw/master/images/yourls-logo.svg" alt="YOURLS Logo" height="120">](https://github.com/YOURLS/YOURLS.pot)

This is the official YOURLS `.pot` file to generate and maintain your own translations.

> [!NOTE]
> Check the [release archives](https://github.com/YOURLS/YOURLS.pot/releases) for older versions.

## Awesome! How do I create my own translation?

1. Download the translation file template `YOURLS.pot`
2. Rename it to `[your-locale].po`, where `[your-locale]` is typically `language code, underscore, country code` (for instance in Portugal that would be `pt_PT`, while in Brazil it’d be `pt_BR`). You'll find a complete list [here](https://simplelocalize.io/data/locales/).  
3. Install a translation tool: it’s nothing more than a text editor capable of reading `.po` files, showing you the untranslated string and a text box where you type in the translation, and saving a `.mo` file which is what PHP needs.\
   There are downloadable offline tools, such as [poEdit](https://poedit.net/), or online tools like [TranslatePOT](https://translatepot.app) which can even (attempt to) translate automatically.
4. Translate all the strings and save your work; you'll end up with a fully translated `pt_BR.po` and the generated `pt_BR.mo`

## Awesome! How do I test my translation in YOURLS?

1. Install the latest [YOURLS release](https://github.com/YOURLS/YOURLS/releases)
2. Drop your `pt_BR.po` and `pt_BR.mo` files in `user/languages`
3. Add `define( 'YOURLS_LANG', 'pt_BR' )` to your `config.php`
4. That’s it! Play with YOURLS to check everything is fine

## Awesome! How do I make my translation available to all?

When your translation file is all fine, make sure others can benefit from your hard work!

1. Upload your two `PO` and `MO` files somewhere on the interweb.\
   It's best to use a *source control service*, such as Github or GitLab: this will make your changes easy to track, your files easy to maintain, and others' contributions easy to implement.  
2. Make it clear for users: a directory with clearly labelled files (`yourls-1.6-pt_BR.zip` for instance) so they know what to pick.  
3. Open a pull request on https://github.com/YOURLS/awesome-yourls and get your translation listed!   

## What languages are already available?

See https://github.com/YOURLS/awesome#translations

## Credits and license

Thanks to [LeoColomb](https://github.com/LeoColomb) - L10n was a low priority feature but he threw his patch at my face :)

License is "Do whatever the hell you want with it".
