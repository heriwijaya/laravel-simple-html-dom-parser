laravel-simple-html-dom-parser
==============================

Simple HTML DOM Parser for Laravel

http://simplehtmldom.sourceforge.net/

Requirement
-----------
- PHP Version      : minimum 5.6.0
- PHP Extensions   : iconv, mbstring
- PHP INI Settings : allow_url_fopen = On

Install
-------
```php
composer require heriw/laravel-simple-html-dom-parser
```

Usage
-----
```php
use Heriw\LaravelSimpleHtmlDomParser\HtmlDomParser;

...
$html = HtmlDomParser::file_get_html($file);
or 
$html = HtmlDomParser::str_get_html($str);

$elements = $html->find($element_name);
...

```
