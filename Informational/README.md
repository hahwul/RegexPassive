# ℹ️ Informational

## URL
- `(https?:\/\/(?:www\.|(?!www))[a-zA-Z0-9][a-zA-Z0-9-]+[a-zA-Z0-9]\.[^\s]{2,}|www\.[a-zA-Z0-9][a-zA-Z0-9-]+[a-zA-Z0-9]\.[^\s]{2,}|https?:\/\/(?:www\.|(?!www))[a-zA-Z0-9]+\.[^\s]{2,}|www\.[a-zA-Z0-9]+\.[^\s]{2,})`

## Internal IP Address
- `((172\.\d{1,3}\.\d{1,3}\.\d{1,3})|(192\.168\.\d{1,3}\.\d{1,3})|(10\.\d{1,3}\.\d{1,3}\.\d{1,3})|([fF][eE][89aAbBcCdDeEfF]::))`

## Email
- `([a-zA-Z0-9_.+-]+@[a-zA-Z0-9]+[a-zA-Z0-9-]*\.[a-zA-Z0-9-.]*[a-zA-Z0-9]{2,})`

## Formats
- JSON: `[^,:{}\[\]0-9.\-+Eaeflnr-u \n\r\t]`

## Encoding
- Base64
  - Basic(loose): `([A-Za-z0-9+\/]{15,}=+)`
  - Encoded JSON: `ey[A-Za-z0-9+\/]{20,}(={0,2})`

## Hashes
- SHA512: `\b[A-Fa-f0-9]{128}\b`
- SHA384: `\b[A-Fa-f0-9]{96}\b`
- SHA256: `\b[A-Fa-f0-9]{64}\b`
- SHA1: `\b[A-Fa-f0-9]{40}\b`
- MD4/MD5: `\b[A-Fa-f0-9]{32}\b`
- Blowfish: `(\$2a\$8\$(.){75})`
- Vbulletin: `(([0-9a-zA-Z]{32}):(\S{3,32}))`

## Comments
- HTML: `(\<![\s]*--[\-!@#$%^&*:;ºª.,"'(){}\w\s\/\\[\]]*--[\s]*\>)`
