# 💣 Unsafe Codes
## DOM XSS
- `/((src|href|data|location|code|value|action)\s*["'\]]*\s*\+?\s*=)|((replace|assign|navigate|getResponseHeader|open(Dialog)?|showModalDialog|eval|evaluate|execCommand|execScript|setTimeout|setInterval)\s*["'\]]*\s*\()/`
- `/(location\s*[\[.])|([.\[]\s*["']?\s*(arguments|dialogArguments|innerHTML|write(ln)?|open(Dialog)?|showModalDialog|cookie|URL|documentURI|baseURI|referrer|name|opener|parent|top|content|self|frames)\W)|(localStorage|sessionStorage|Database)/`

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

## Prototype Pollution
- CanJS deparam [1]: `(\/\(\[\^\[\]\]\+\)\`
- MooTools More [1]: `(\.substr\(0,\s*\w+\s*-\s*1\)\.match\(\/\(\[\^\]\?\[\]\+\`
- Purl [1]: `(String\(\w+\)\.split\(\/&\`
- Segment analytics.js [1]: `(\w+\s*=\s*\/\(\w\+\)\[\(\d\+\)\]\/)`
- Segment analytics.js [2]: `(\(\w+\s*=\s*\w+\.exec\(\w+\)\)\s*\?\s*\(\s*\w+\[\w+\[1\]\]\s*=\s*\w+\[\w+\[1\]\]\s*\`
- Unknown Lib [1]: `(\w+\.replace\(\s*[\'"]\[\][\'"]\s*,\s*[\'"]\[[\'"]\.concat\()`
- Unknown Lib [2]: `(\w+\s*=\s*\w+\.slice\(0,\s*\w+\.indexOf\([\'"]?0?0[\'"]\)\))`
- Unknown Lib [3]: `([]\s*===\s*\w+\.substring\(\w+\.length\s*-\s*2\)[\s\?\)\(]*(?:\w+\[)?\w+\s*=\s*\w+\.substring\(0,\s*\w+\.length\s*-\s*2\))`
- Unknown Lib [4]: `(\w+\.match\(\/\(\^\[\^\[\]\+\)\(\[\.\*\]$\)\?\/\))`
- Unknown Lib [5]: `(\(\[\^\\[\^\\]\]\+\)\(\(\\[\(\^\\[\^\\]\)\\]\)\*\))`
- Unknown Lib [6]: `([\'"]-1[\'"]\s*==\s*\w+\[1\]\.indexOf\([\'"]\[[\'"]\))`
- Unknown Lib [7]: `/([^&=]+)=?([^&]*)/g`
- Unknown Lib [8]: `toeStrFirstUp`
- Unknown Lib [9][1]: `queryParamsToObject`
- Unknown Lib [9][2]: `/^[\{\[].*[\}\]]$/`
- V4Fire Core [1]: `(\w+\s*=\s*\/\[\(\[\^\]\]\*\)\]\/g)`
- YUI 3 querystring-parse [1]: `(\/\(\.\*\)\[\(\[\^\]\]\*\)\]$\/\.exec\(\w+\))`
- backbone-query-parameters [2]: `(\s*(\w+)\s*=\s*\2\[(\w+)\]\s*=\s*\2\[\3\]\s*\`
- cdn.fera.ai [1]: `(\?\s*decodeURIComponent\(\s*\w+\.substr\(\s*\w+\s*\+\s*1\)\)\s*:\s*[\'"][\'"])`
- cdn.fera.ai [2]: `getFeraActionParams`
- cdn.fera.ai [3]: `cdn.fera.ai/js/fera.js`
- deparam [1]: `(\s*\/\[\/\.test\(\s*\w+\[0\]\s*\)\s*&&\s*\/\]$\/\.test\(\s*\w+\[\s*\w+\s*\]\s*\)\s*)`
- deparam [2]: `([\'"]\[\][\'"]\s*===\s*\w+\s*\?\s*\w+\.push\(\w+\)\s*:\s*\w+\[\w+\]\s*=\s*\w+)`
- flow.io [1]: `(\w+\s*=\s*\/\[\?\(\[\^\]\[\]\+\)\]\?\/g)`
- jQuery BBQ [1]: `($\.each\(\s*\w+\.replace\(\s*\/\+\/g\s*,\s*[\'"] [\'"]\s*\)\.split\(\s*[\'"]&[\'"]\s*\))`
- jQuery BBQ [2]: `jQuery BBQ`
- jQuery Query-Object [1]: `(\/\^\(\[\^\[\]\+\)\(\[\.\*\]\)\?$\/\.exec\(\s*\w+\s*\))`
- jQuery Query-Object [2]: `/* jQuery querystring plugin */`
- jQuery Query-Object [3]: `/^([^[]+?)(\[.*\])?$/.exec(`
- jQuery Sparkle [1]: `(\w+\s*=\s*\w+\.split\(\/\&\(amp\;\)\?\/\))`
- jQuery.parseParams.js [1]: `(\w+\s*=\s*\w+\.split\(\/\.\(\.\+\)\?\/\)\[1\])`
- queryToObject [1]: `(\.match\(\/\(\^\[\^\[\]\+\)\(\[\.\*\]$\)\?\/\))`
- wishpond [1]: `(\w+\s*=\s*\w+\(\w+\[1\]\.slice\(\w+\s*\+\s*1,\s*\w+\[1\]\.indexOf\([\'"]\][\'"],\s*\w+\)\)\))`
