# ⚠️ Error Patterns

## Takeovers
- aftership: `Oops.</h2><p class=\"text-muted text-tight\">The page you're looking for doesn't exist.`
- acquia: `The site you are looking for could not be found.`
- agilecrm: `Sorry, this page is no longer available.`
- aha: `There is no portal here ... sending you back to Aha!`
- airee: `Ошибка 402. Сервис Айри.рф не оплачен`
- anima: `If this is your website and you've just created it, try refreshing in a minute`
- announcekit: `Error 404 - AnnounceKit`
- aws-bucket: `The specified bucket does not exist`
- bigcartel: `<h1>Oops! We couldn&#8217;t find that page.</h1>`
- bitbucket: `Repository not found`
- brightcove: `<p class=\"bc-gallery-error-code\">Error Code: 404</p>`
- campaignmonitor: `<strong>Trying to access your account?</strong>`
- canny: `Company Not Found`
- cargocollective: `<div class=\"notfound\">`
- cargo: `If you're moving your domain away from Cargo you must make this configuration through your registrar's DNS control panel.`
- feedpress: `The feed has not been found.`
- flexbe: `Domain isn't configured`
- flywheel: `We're sorry, you've landed on a page that is hosted by Flywheel`
- fastly: `Fastly error: unknown domain`
- frontify: `404 - Page Not Found`
- gemfury: `404: This page could not be found.`
- getresponse: `With GetResponse Landing Pages, lead generation has never been easier`
- ghost: `offline.ghost.org`
- gitbook: `If you need specifics, here's the error`
- github: `There isn't a GitHub Pages site here.`
- hatenablog: `404 Blog is not found`
- helpjuice: `We could not find what you're looking for.`
- helprace: `Alias not configured!`
- helpscout: `No settings were found for this company:`
- heroku: `herokucdn.com/error-pages/no-such-app.html`
- hubspot: `Domain not found`
- intercom: `<h1 class=\"headline\">Uh oh. That page doesn\\’t exist.</h1>`
- jazzhr: `This account no longer active`
- jetbrains: `is not a registered InCloud YouTrack.`
- kinsta: `No Site For Domain`
- launchrock: `It looks like you may have taken a wrong turn somewhere. Don't worry...it happens to all of us.`
- mashery: `Unrecognized domain <strong>`
- netlify: `Not found - Request ID:`
- ngrok: `ngrok.io not found`
- pagewiz: `404 - Page Not Found`
- pantheon: `The gods are wise, but do not know of the site which you seek.`
- pingdom: `Public Report Not Activated`
- proposify: `If you need immediate assistance, please contact <a href=\"mailto:support@proposify.biz`
- readme: `Project doesnt exist... yet!`
- readthedocs: `unknown to Read the Docs`
- shopify: `To finish setting up your new web address, go to your domain settings, click \"Connect existing domain\"`
- short-io: `Link does not exist`
- simplebooklet: `We can't find this <a href=\"https://simplebooklet.com`
- smartjob: `Job Board Is Unavailable`
- smugmug: `{\"text\":\"Page Not Found\"`
- strikingly: `But if you're looking to build your own website`
- surge: `project not found`
- surveygizmo: `data-html-name`
- tave: `<h1>Error 404: Page Not Found</h1>`
- teamwork: `Oops - We didn't find your site.`
- tictail: `Building a brand of your own?`
- tilda: `Please go to the site settings and put the domain name in the Domain tab.`
- tumblr: `Whatever you were looking for doesn't currently exist at this address.`
- uberflip: `Non-hub domain, The URL you've accessed does not provide a hub.`
- uservoice: `This UserVoice subdomain is currently available!`
- vend: `Looks like you've traveled too far into cyberspace.`
- webflow: `<p class=\"description\">The page you are looking for doesn't exist or has been moved.</p>`
- wishpond: `https://www.wishpond.com/404?campaign=true`
- wix: `Error ConnectYourDomain occurred`
- wordpress: `Do you want to register`
- worksites.net: `Hello! Sorry, but the website you&rsquo;re looking for doesn&rsquo;t exist.</p>\n<a href=\"https://worksites.net/\">Learn more about Worksites.net`
- wufoo: `Profile not found`
- zendesk: `this help center no longer exists`

## Databases
### MySQL
- `(SQL syntax.*MySQL|Warning.*mysql_.*|MySqlException \\(0x|valid MySQL result|check the manual that corresponds to your (MySQL|MariaDB) server version|MySqlClient\\.|com\\.mysql\\.jdbc\\.exceptions)`
- `SQL syntax.*?MySQL`
- `Warning.*?mysqli?`
- `MySQLSyntaxErrorException`
- `valid MySQL result`
- `check the manual that (corresponds to|fits) your MySQL server version`
- `check the manual that (corresponds to|fits) your MariaDB server version`
- `check the manual that (corresponds to|fits) your Drizzle server version`
- `Unknown column '[^ ]+' in 'field list'`
- `com\\.mysql\\.jdbc`
- `Zend_Db_(Adapter|Statement)_Mysqli_Exception`
- `MySqlException`
- `Syntax error or access violation`

### PostgreSQL
- `(PostgreSQL.*ERROR|Warning.*\\Wpg_.*|valid PostgreSQL result|Npgsql\\.|PG::SyntaxError:|org\\.postgresql\\.util\\.PSQLException|ERROR:\\s\\ssyntax error at or near)`
- `PostgreSQL.*?ERROR"`
- `Warning.*?\\Wpg_`
- `valid PostgreSQL result`
- `Npgsql\\."`
- `PG::SyntaxError:`
- `org\\.postgresql\\.util\\.PSQLException`
- `ERROR:\\s\\ssyntax error at or near`
- `ERROR: parser: parse error at or near`
- `PostgreSQL query failed`
- `org\\.postgresql\\.jdbc`
- `PSQLException`

### MSSQL
- `(Driver.* SQL[\\-\\_\\ ]*Server|OLE DB.* SQL Server|\bSQL Server.*Driver|Warning.*mssql_.*|\bSQL Server.*[0-9a-fA-F]{8}|[\\s\\S]Exception.*\\WSystem\\.Data\\.SqlClient\\.|[\\s\\S]Exception.*\\WRoadhouse\\.Cms\\.|Microsoft SQL Native Client.*[0-9a-fA-F]{8})`
- `Driver.*? SQL[\\-\\_\\ ]*Server`
- `OLE DB.*? SQL Server`
- `\bSQL Server[^&lt;&quot;]+Driver`
- `Warning.*?\\W(mssql|sqlsrv)_`
- `\bSQL Server[^&lt;&quot;]+[0-9a-fA-F]{8}`
- `System\\.Data\\.SqlClient\\.SqlException`
- `(?s)Exception.*?\bRoadhouse\\.Cms\\.`
- `Microsoft SQL Native Client error '[0-9a-fA-F]{8}`
- `\\[SQL Server\\]`
- `ODBC SQL Server Driver`
- `ODBC Driver \\d+ for SQL Server`
- `SQLServer JDBC Driver"`
- `com\\.jnetdirect\\.jsql`
- `macromedia\\.jdbc\\.sqlserver`
- `Zend_Db_(Adapter|Statement)_Sqlsrv_Exception`
- `com\\.microsoft\\.sqlserver\\.jdbc`
- `SQL(Srv|Server)Exception`

### Oracle
`(\\bORA-\\d{5}|Oracle error|Oracle.*Driver|Warning.*\\Woci_.*|Warning.*\\Wora_.*)`

### IBMDB2
`(CLI Driver.*DB2|DB2 SQL error|\\bdb2_\\w+\\(|SQLSTATE.+SQLCODE)`

### Informix
`(Exception.*Informix)`

### SQLite
`(SQLite\\/JDBCDriver|SQLite.Exception|System.Data.SQLite.SQLiteException|Warning.*sqlite_.*|Warning.*SQLite3::|\\[SQLITE_ERROR\\])`

### SAPDB
`(SQL error.*POS([0-9]+).*|Warning.*maxdb.*)`

### Sybase
`(Warning.*sybase.*|Sybase message|Sybase.*Server message.*|SybSQLException|com\\.sybase\\.jdbc)`

### Ingress
`(Warning.*ingres_|Ingres SQLSTATE|Ingres\\W.*Driver)`

### Frontbase
`(Exception (condition )?\\d+. Transaction rollback.)`

### HSQLDB
`(org\\.hsqldb\\.jdbc|Unexpected end of command in statement \\[|Unexpected token.*in statement \\[)`
