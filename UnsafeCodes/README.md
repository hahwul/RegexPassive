# Unsafe Codes
## DOM XSS
- `eval\(`

## DOM Clobbering
- `(location|\.href|\.innerHTML|\.outerHTML|document.URL|\.srcdoc)(|\s)=(|\s)window\..*`
- `(eval\(|html\(|constructor\(|setInterval\(|setTimeout\(|document.write\(|document.execCommand\()(|\s)window\..*`

## Relative Path Overwrite
- `(href\=\"((?!\/|http|www)).*\.css\")`

## ReDOS
- `^([a-zA-Z0-9])(([\-.]|[_]+)?([a-zA-Z0-9]+))*(@){1}[a-z0-9]+[.]{1}(([a-z]{2,3})|([a-z]{2,3}[.]{1}[a-z]{2,3}))$`
  - Attack: aaaaaaaaaaaaaaaaaaaaaaaa!
- `^(([a-z])+.)+[A-Z]([a-z])+$`
  - Attack: aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa!
