# Write Kanji
 Learn, read, write and practice Kanji by drawing strokes with Onyomi, Kunyomi and Meaning in English.

# Demo
<img src="/Images/write-kanji-demo.gif" height="560" width="263"></img>

# Quick Start
**Download from AnkiWeb**
<br>[Write Kanji](https://ankiweb.net/shared/info/1546710114)

**Download from GitHub**
<br>Download lated deck from release page
<br>[Release](https://github.com/infinyte7/Write-Kanji/releases)

# Features
- Night mode
- Change size of characters
- Change drawing stroke width
- Kanji with Onyomi, Kunyomi and Meaning in English.
- Characters listed at https://www.mext.go.jp/a_menu/shotou/new-cs/youryou/syo/koku/001.htm 
- Indicator at bottom for showing if character loaded or not (green - loaded, red - not loaded or some error)

Note: Some changes will get reflect from next card.

# Turn off default settings
If below lines not present in write kanji deck then deck can be updated by two methods.
1. Download latest deck from [release page.](https://github.com/infinyte7/Write-Kanji/releases)
or
2. Copy the [back.html](https://github.com/infinyte7/Write-Kanji/blob/master/Versions/Version%201.1/back.html) to Back Template of deck.
View [this](https://github.com/infinyte7/Anki-xiehanzi/wiki/Update-xiehanzi-deck-on-AnkiDesktop) to copy [back.html](https://github.com/infinyte7/Write-Kanji/blob/master/Versions/Version%201.1/back.html) to existing deck.

Now,
Open template editor.
In ``` Back Template ``` at top will be following lines
```html
<script>
    var default_show_kanji = true;
    var default_show_onyomi = true;
    var default_show_Kunyomi = true;
    var default_show_outline = true;
    var default_show_meaning = true;
</script>
```
Change true to false for not showing the respective fields.
For ex:- To stop by default showing Kanji at beginning of review.
```javascript
var default_show_kanji = false;
```

 # Data
 Character's stroke data
 <br>https://github.com/chanind/hanzi-writer-data-jp

 Kanji list taken from
 <br>https://www.mext.go.jp/a_menu/shotou/new-cs/youryou/syo/koku/001.htm

 Onyomi, Kunyomi and Meaning extracted from 
 <br>https://github.com/davidluzgouveia/kanji-data

# Faq?
**Are all kanji supported?**
<br>No, Currently [hanzi-writer-data-jp](https://github.com/chanind/hanzi-writer-data-jp) limited number of kanji data json.

**Are kana characters supported?**
<br>No, View this. [https://github.com/chanind/hanzi-writer-data-jp/issues/3](https://github.com/chanind/hanzi-writer-data-jp/issues/3)

**Can I add my own words?**
<br>Yes, See [Anki Manual](https://docs.ankiweb.net/#/editing?id=addingediting).

# Add to existing deck
![](https://github.com/infinyte7/Write-Kanji/blob/master/Images/add_to_existing_deck.gif)

# View xiehanzi Wiki
[Wiki](https://github.com/infinyte7/Anki-xiehanzi/wiki) 

# Bug, feature request or have any questions?
https://github.com/infinyte7/Write-Kanji/issues

<a href='https://ko-fi.com/L3L820U7D' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://cdn.ko-fi.com/cdn/kofi3.png?v=2' border='0' alt='Buy Me a Coffee at ko-fi.com' /></a>

# License
**Write Kanji**
MIT License<br>
Copyright (c) 2020 infinyte7

### Other Third party licenses
Read [License](License)
