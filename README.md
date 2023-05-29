# Webster's Dictionary 1844

## Introduction

This is an okay dictionary. If you're interested in a better one, check out the [1828 version](https://codeberg.org/christianlibertyinstitute/webster1828), also released by [Christian Liberty Institute](http://christianlibertyinstitute.org/).

## Installation Instructions

- Apple Mac OS X/macOS: Unzip the archive and copy the .dictionary file to `/Library/Dictionaries/` for all users or `~/Library/Dictionaries/` for the current user. If the Dictionary app isn't working properly, you may need to run this in Terminal: `rm ~/Library/Caches/com.apple.DictionaryServices/DictionaryCache.plist` and restart the app to clear out the cache.
- SWORD module: An archive has been provided for local installations. I did not submit this one to CrossWire because something is wrong with the SWORD export. You should use the 1828 dictionary instead, which is available from the CrossWire repo.
- KOReader: Unzip the StarDict archive and copy the directory to `/.adds/koreader/data/dict/`
- Amazon Kindle: Unzip the archive and copy the .mobi file to `/documents/dictionaries/`. You may need to restart your Kindle before it will work properly.
- Rakuten Kobo: Rename the `webster1844-x.x-kobo.zip` to `dicthtml-pt-en.zip` (which will replace the Portuguese to English dictionary, use another language if you don't want that) and copy it to `/.kobo/dict/`
- Plato: Unzip the StarDict archive and copy the directory to `/.adds/plato/dictionaries/`

This has been tested with:
- The Dictionary.app in Mac OS X Snow Leopard. It may work with earlier versions and should work with whatever garbage OS Apple is putting out now.
- The SWORD module using MacSword and Xiphos.
- KOReader (2023 release) running on a Kobo Aura H2O.

I don't use Kobo's built-in dictionary or Plato, so I cannot vouch for the quality of those and I didn't test the Kindle version because the 1828 is superior.

## Building From Source

I am using [PyGlossary](https://github.com/ilius/pyglossary) to convert the CSV file to the other dictionary formats. The directory `Metadata` contains the files needed to make the title show up correctly on devices.