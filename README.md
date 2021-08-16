# Translations

[![Open Issues](https://img.shields.io/github/issues/spamty/translate)](https://github.com/spamty/translate/issues)

[![Twitter Follow](https://img.shields.io/twitter/follow/spamty?style=social)](https://twitter.com/Spamty)
[![GitHub](https://img.shields.io/github/followers/spamty?label=GitHub&style=social)](https://github.com/spamty/)

This is the translation for the spamty.eu website.

Translation is done with .po files located in `/translate/LANG_LANG/LC_MESSAGES/spamty.po`.
The .mo files are generated automatically.


## Languages

Spamty is currently available in:

|Language |Status             |details    |URL |Language Code |System      |
|---      |---                |---        |--- |---           |---         |
|German   |:white_check_mark: |100%       |de  |de_DE         |de_DE.UTF-8 |
|Arabic   |:x:                |TBD        |ar  |              |            |
|English  |:white_check_mark: |primary    |en  |en_US         |en_US.UTF-8 |
|Spanish  |:x:                |Incomplete |es  |es_ES         |es_ES.UTF-8 |
|French   |:white_check_mark: |needs check|fr  |fr_FR         |fr_FR.UTF-8 |
|Chinese  |:x:                |Incomplete |zh  |zh_CN         |zh_CN.UTF-8 |

For URLs we prefer to use *ISO 639-1 codes* <https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes>.



# Server configuration

_Only internal information_

The languages have to be installed on the server. Check which ones are installed with `locale -a`.
In Debian uncomment the required languages in `/etc/locale.gen`. Then run `locale-gen`.

# Website configuration

_Only internal information_

PHP config is in `ws-head.php` file.

The language setting is stored in cookie named *lang*.
Set cookie with chosen language (with Javascript) by clicking on flag icon.
If no cookie is set use browser language or it will be set to currently viewed language.
