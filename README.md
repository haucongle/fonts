# Visual Studio Code

### settings.json

```
{
   "editor.fontFamily": "'Operator Mono Lig', FiraCode-Retina, 'SourceCodePro+Powerline+Awesome Regular', Menlo, Monaco, 'Courier New', monospace",
    "editor.fontLigatures": true,
    "editor.tokenColorCustomizations": {
        "textMateRules": [
          {
            "scope": [
              //following will be in italic (=FlottFlott)
              "comment",
              "entity.name.type.class", //class names
              "keyword", //import, export, return…
              "constant", //String, Number, Boolean…, this, super
              "storage.modifier", //static keyword
              "storage.type.class.js", //class keyword
            ],
            "settings": {
              "fontStyle": "italic"
            }
          },
          {
            "scope": [
              //following will be excluded from italics (VSCode has some defaults for italics)
              "invalid",
              "keyword.operator",
              "constant.numeric.css",
              "keyword.other.unit.px.css",
              "constant.numeric.decimal.js",
              "constant.numeric.json"
            ],
            "settings": {
              "fontStyle": ""
            }
          }
        ]
    }
}
```
