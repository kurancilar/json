# Kur'an-ı Kerîm JSON

Sure, ayet ve sesleri JSON dosyası olarak barındırın.

```
.
├── LICENSE
├── README.md
├── audio
|   └── <SURE_NUMARASI:001-114>
|       ├── <AYET NUMARASI:001-n>.mp3
|       └── index.json
└── sure
    └── <SURE_NUMARASI>.json
```

#### Adresler

`https://kurancilar.github.io/json/sure/<SURE_NUMARASI>.json`

`https://kurancilar.github.io/json/audio/<SURE_NUMARASI:001-114>.json`

#### Örnek Kullanım

**Vanilla JavaScript:**

```js
    fetch("https://kurancilar.github.io/json/sure/1.json")
        .then(dat => dat.json())
        .then(json => {
            json.verses.forEach(ayet => {
                document.write(ayet.arabic);
                document.write("<br>");
            })
        })
```

#### Lisans

[MIT Lisansı](/LICENSE)