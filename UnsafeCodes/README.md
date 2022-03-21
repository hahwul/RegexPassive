# Unsafe Codes
## DOM XSS
- `eval\(`

## DOM Clobbering
- `(location|\.href|\.innerHTML|\.outerHTML|document.URL|\.srcdoc)(|\s)=(|\s)window\..*`
- `(eval\(|html\(|constructor\(|setInterval\(|setTimeout\(|document.write\(|document.execCommand\()(|\s)window\..*`
