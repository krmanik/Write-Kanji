# Add writing component to existing deck

Features
- Support Kanji and Kana
- Night mode
- Character and grid height
- Show and hide outline
- Show stroke with animation
- Skip to next character

# Add to existing deck with Kanji

1. Download zip files which contains necessary files<br>
[Download - Add Kanji writer v2.0](https://github.com/infinyte7/Write-Kanji/releases/download/v2.0/Add.Kanji.writer.to.existing.deck.version.2.0.zip)

```
_hanzi_writer_style.css
_hanzi_writer_xiehanzi_kanji.js
_Material-Icons.woff2
```

2. Extract zip file and copy all three files to `Anki/User 1/collection.media` folder

3. Open card template editor or note editor for current deck and add the following to back or front side of card template.

Note: 1. Change `{{Expression}}` to fields in your Anki Kanji decks<br>
      2. **To hide the add this to the div of Expression**, `style="display:none;"`<br>
      `<div id='ch_kanji' class="text-color4" style="display:hidden">{{Expression}}</div>`

```html
<div id='ch_kanji' class="text-color4">{{Expression}}</div>
<div id="character-target-div"></div>
<div id="bottom-Button"></div>

<script>
    var show_outline = true;     // default show outline, put false for hiding
    var charHW = 70;             // default grid size on screen on scale of 0-100
    var strokeWidth = 10;        // default brush size

    var url_hanzi = "https://cdn.jsdelivr.net/gh/infinyte7/hanzi-writer-data-jp@master/data/";
    // var url_hanzi = "http://127.0.0.1:8080/data/";
</script>


<script>
    // https://forums.ankiweb.net/t/linking-to-external-javascript/1713/4
    var injectScript = (src) => {
        return new Promise((resolve, reject) => {
            const script = document.createElement('script');
            script.src = src;
            script.async = true;
            script.onload = resolve;
            script.onerror = reject;
            document.head.appendChild(script);
        });
    };

    (async () => {
        if (typeof keyman === 'undefined') {
            await injectScript('_hanzi_writer_xiehanzi_kanji.js');
        }
    })();
</script>
```

4. Add following to Styling of card template.
```css
@import "_hanzi_writer_style.css";
```



