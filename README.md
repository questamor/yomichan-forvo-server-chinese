# Yomichan Forvo Server for Anki (Chinese)

Simple server to take advantage of Yomichan's custom audio sources feature. Requires Anki Connect. It web scrapes Forvo's search and word page to get a list of words.

Prerequisites:

- Anki
- Yomichan
- Anki Connect

Install:
1. Navigate to `C:\Users\<user>\AppData\Roaming\Anki2\addons21`, create new folder with any name and copy file `__init__.py` into it
2. Restart Anki
3. Allow network connections (required since this is a local server)
4. In yomichan settings, go to Audio > Configure Audio Playback Sources > Custom Audio Source
5. Select type to `Custom URL (JSON)` and set URL to `http://localhost:8770/?expression={term}&reading={reading}`
6. In your Audio Sources list below, make sure one of them is set to Custom

Now when you scan a word in Yomichan, you should be able to right click the audio icon and the Forvo custom audio sources should appear.

For dialects, edit the code of the add-on. Just change all zh to another language code:
- Min Nan - `nan`
- Wu Chinese - `wuu`
- Hakka - `hak`
