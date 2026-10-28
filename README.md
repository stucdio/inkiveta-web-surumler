# inkiveta web sürüm kaydı

web.inkiveta.com'un yayımlanan her sürümünün parmak izi (manifest, importmap, WASM sha256) bu depoda, **yalnız ekleme** ile ve
inkiveta'nın çevrimdışı tutulan Ed25519 anahtarıyla **imzalı** olarak tutulur. `web.json` dosyası, çalışan sayfayı ve "inkiveta Doğrula"
eklentisini bağımsız bir kayıtla karşılaştırmak içindir.

- Dosya: `web.json` = `{ "surumler": [...], "imza": "<b64>", "anahtarKimligi": "ed25519:<16 hex>" }`
- İmzalanan bayt: `surumler` dizisinin kanonik JSON'u (anahtarlar alfabetik, boşluksuz, ASCII).
- Açık anahtar (ham 32 bayt, base64): `s+R5RtttvQFbKtambAOKCbEWAjYYDJXW+GM7NJCIxDE=`
- Anahtar kimliği: `ed25519:d3bc08c290001feb`

Kayıt silinmez, değiştirilmez; yeni sürüm listenin başına eklenir. Geçmiş git geçmişi ve yansılarla korunur.

Tüm hakları saklıdır.
