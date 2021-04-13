# contentful-html-to-rich-text

A library to convert basic HTML to Contentful Rich Text.

## Installation

Using [composer](https://getcomposer.org/):

```sh
composer require ppito/contentful-html-to-rich-text
```

## Usage

### Basic

```php
<?php
// composer require contentful/contentful-management
require __DIR__ . '/vendor/autoload.php';


$content = \Contentful\HtmlToRichText\Tool::parse("<p>Hello</p><p>Another with <strong>bold maybe?</strong></p>");
```

### Supported

The library will convert automatically the following HTML tags :

- `h1`
- `h2`
- `h3`
- `h4`
- `h5`
- `h6`
- `div`
- `p`
- `ul`
- `ol`
- `li`
- `blockquote`
- `br`
- `hr`
- `a`
- `span`
- `strong`
- `b`
- `u`
- `em`
- `i`
- `code`
- `section`
- `footer`
- `header`
- `nav`
- `aside`

### Unsupported
The attribute HTML are not supported (`id=""`, `class=""`, `style=""`, etc.)
