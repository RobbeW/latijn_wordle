# Vue Griekse Wordle

[Live demo](https://latijnwordle.netlify.app)

Een Griekse Vue-implementatie van het [Wordle-spel](https://www.powerlanguage.co.uk/wordle/). Dit is gewoon voor de lol en is niet bedoeld om het origineel 100% na te maken.

Je kunt je eigen Wordle maken en naar vrienden sturen door een woord te base64-encoderen en het als URL-query op te nemen, bijv. [https://latijnwordle.netlify.app?zpvOn86Tzp/Oow==](https://latijnwordle.netlify.app/?zpvOn86Tzp/Oow==) (dit laat ook woorden toe die niet in het woordenboek staan).

## Woordenlijst configureren

De woordenlijst kan extern geladen worden door de omgevingsvariabele `VITE_WORD_LIST_URL` te zetten naar een raw bestand met een object als:

```
const words = {
  ΕΙΝΑΙ: true,
  ΕΣΤΙΝ: true
}
```

Voorbeeld:

```
VITE_WORD_LIST_URL=https://raw.githubusercontent.com/jouw-account/jouw-repo/main/src/data/words.js
```

Dit archief is alleen open source voor leerdoeleinden - de originele maker(s) van Wordle bezitten alle toepasselijke rechten op het spel zelf.
