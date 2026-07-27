# loungemusik.eu decrypted

`decrypted.html` is the full plaintext of [loungemusik.eu](https://loungemusik.eu).

The site ships its own page as an AES-256-GCM encrypted blob. The key is embedded in the same page, right next to the ciphertext, and an inline script decrypts everything in your browser before showing it.

This repo is the result of running that decryption once and saving the output.

## Music

The audio is deliberately not part of this repo. The page fetches `audio/lounge-city.enc` (encrypted with another hardcoded key) and plays it after in-browser decryption. I dont want to redistributed it here.