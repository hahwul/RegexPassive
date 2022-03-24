# Informational

## Internal IP Address
- `((172\.\d{1,3}\.\d{1,3}\.\d{1,3})|(192\.168\.\d{1,3}\.\d{1,3})|(10\.\d{1,3}\.\d{1,3}\.\d{1,3})|([fF][eE][89aAbBcCdDeEfF]::))`

## Email
- `([a-zA-Z0-9_.+-]+@[a-zA-Z0-9]+[a-zA-Z0-9-]*\.[a-zA-Z0-9-.]*[a-zA-Z0-9]{2,})`

## Encoding
- Base64: `([A-Za-z0-9+\/]{15,}=+)`

## Hashes
- SHA512: `(\$6\$\w{8}\S{86})`
- MD4/MD5: `([a-f0-9]{32})`
- Blowfish: `(\$2a\$8\$(.){75})`
- Vbulletin: `(([0-9a-zA-Z]{32}):(\S{3,32}))`

## Comments
- HTML: `(\<![\s]*--[\-!@#$%^&*:;ºª.,"'(){}\w\s\/\\[\]]*--[\s]*\>)`
