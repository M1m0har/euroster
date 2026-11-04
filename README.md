# Euroster

A private Eurovision song timeline game. Scan a card, the song plays on Spotify, guess the year.

## Put it online (GitHub Pages, free)
1. Create a new public repository on github.com, for example `euroster`.
2. Upload every file in this folder (not src.html, which isn't included).
3. Settings > Pages > Deploy from branch > `main` / root. Wait a minute.
4. Open `https://<your-username>.github.io/euroster/`.

## Connect Spotify (once)
Open the site, go to Settings and follow the four steps shown there.

## Optional: no external scripts at all
Phones without a built-in QR reader (mainly iPhones) load the scanner library from unpkg.com.
To serve it yourself, download https://unpkg.com/html5-qrcode@2.3.8/html5-qrcode.min.js
and upload it to the repository next to index.html. The app uses the local copy when present.

## Install on the home screen
iPhone: open the site in Safari > Share > Add to Home Screen.
Android: open in Chrome > menu > Install app.

## Card numbers never change
Every song has a fixed card number (#0001 to #0878, in year and placing order). Each QR code holds
that number plus the Spotify track, for example `https://m1m0har.github.io/euroster/#c=0042&t=<spotify id>`.
Printed cards therefore play on any phone and stay valid even if you reprint. New songs added later
get new numbers at the end (0879 onwards), so existing cards are never renumbered.
