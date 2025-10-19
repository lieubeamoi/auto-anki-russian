# Auto Anki for Russian
Automatically generate Russian language flashcards for [Anki](https://apps.ankiweb.net/).

# Dependencies
- [Python 3](https://www.python.org/downloads/)
- [Anki](https://apps.ankiweb.net/) and the [AnkiConnect](https://ankiweb.net/shared/info/2055492159) add-on.
- (Optional) To automatically retrieve audio from [Forvo](https://forvo.com/), you will need to purchase your own API key [here](https://api.forvo.com/plans-and-pricing/) and include it in the `.env` file. 

# Description
This program automatically generates Russian language Anki flashcards in the following combinations:
- Translate, "\<Russian word audio\>" to English.
- Translate, "\<Russian word text\>" to English.
- Type, "\<Russian word audio\>" in Russian.
- (Optional) Conjugate, "\<Russian verb text\>".

This program uses the [Wiktionary API](https://en.wiktionary.org/w/api.php) to retrieve audio samples and definitions for new words. You can choose to provide your own audio files and definitions. Sometimes Wiktionary may not have an audio sample for some words, in which case this program will fallback to retrieving the audio sample from [Forvo](https://forvo.com/). To retrieve audio from Forvo, you must purchase a Forvo API key [here](https://api.forvo.com/plans-and-pricing/) and include it in the `.env` file.
