# 🔐 Secrets

## Certificate
- RSA Key: `-----BEGIN RSA PRIVATE KEY-----|-----END RSA PRIVATE KEY-----`
- Private Key: `-----BEGIN PRIVATE KEY-----|-----END PRIVATE KEY-----`

## Sessions
- Typical Session: `session=(.*?).*`
- Tomcat: `JSESSIONID=(.*?).*`
- Rails: `([a-zA-Z0-9_]*)_session=(.*?).*`
- PHP: `PHPSESSID=(.*?).*`
- Django: `sessionid=(.*?).*`

## API Keys and Tokens
- AWS Access Key: `AKIA[0-9A-Z]{16}`
- AWS Appsync GraphQL: `da2-[a-z0-9]{26}`
- Amazon MWS Auth Token: `amzn\\.mws\\.[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}`
- Google oauth ID: `[0-9(+-[0-9A-Za-z_]{32}.apps.qooqleusercontent.com`
- Google API: `AIza[0-9A-Za-z-_]{35}`
- Google oauth: `ya29\\.[0-9A-Za-z\\-_]+`
- Facebook Access Token: `EAACEdEose0cBA[0-9A-Za-z]+`
- Github Access Token: `[a-zA-Z0-9_-]*:[a-zA-Z0-9_\\-]+@github\\.com*`
- Telegram Bot API Key: `[0-9]+:AA[0-9A-Za-z\\-_]{33}`
- Square Access Token: `sq0atp-[0-9A-Za-z\\-_]{22}`
- Square Oauth Secret: `sq0csp-[0-9A-Za-z\\-_]{43}`
- Twitter Access Token: `[tT][wW][iI][tT][tT][eE][rR].*[1-9][0-9]+-[0-9a-zA-Z]{40}`
- Twilio API Key: `SK[0-9a-fA-F]{32}`
- Braintree Token: `access_token\\$production\\$[0-9a-z]{16}\\$[0-9a-f]{32}`
- Stripe API Key: `sk_live_[0-9a-zA-Z]{24}`
- Stripe Restricted Key: `rk_live_[0-9a-zA-Z]{24}`
- Slack Token: `(xox[p|b|o|a]-[0-9]{12}-[0-9]{12}-[0-9]{12}-[a-z0-9]{32})`
- Facebook Oauth: `[f|F][a|A][c|C][e|E][b|B][o|O][o|O][k|K].{0,30}['\"\\s][0-9a-f]{32}['\"\\s]`
- Twitter Oauth: `[t|T][w|W][i|I][t|T][t|T][e|E][r|R].{0,30}['\"\\s][0-9a-zA-Z]{35,44}['\"\\s]`
- Heroku API: `[h|H][e|E][r|R][o|O][k|K][u|U].{0,30}[0-9A-F]{8}-[0-9A-F]{4}-[0-9A-F]{4}-[0-9A-F]{4}-[0-9A-F]{12}`
- Mailgun API: `key-[0-9a-zA-Z]{32}`
- Mailchamp API: `[0-9a-f]{32}-us[0-9]{1,2}`
- Picatic API: `sk_live_[0-9a-z]{32}"`

## Hooks
- Slack hook: `https://hooks.slack.com/services/T[a-zA-Z0-9_]{8}/B[a-zA-Z0-9_]{8}/[a-zA-Z0-9_]{24}`
- Slack hook: `https://hooks.slack.com/services/T[a-zA-Z0-9_]{8,10}/B[a-zA-Z0-9_]{8,10}/[a-zA-Z0-9_]{24}`
