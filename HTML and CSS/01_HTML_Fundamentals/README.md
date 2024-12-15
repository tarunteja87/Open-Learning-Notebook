# HTML (Hypert Text Markup Language)

- HTML consists of elements thta describe different types of content : paragraph , links , headings , images , video, etc,


## Anotamy of HTML Element
> `<p> HTML is a markup languege </p>`

 opening tag + content + closing tag

 ## HTML Document structure

 ```
 <!DOCTYPE html>
 <html>
 <head>
    <title> </title>
 <head>
 <body>
    <p>this is a paragarph</p>
 </body>
 </html>
 ```

## comment
> <!-- comment -->

## Bold text in html

> <b>content</b> use strong instead of b `<strong>content</strong>`

## Italic text 

> <i></i>  use em instead of i `<em>content</em>`

## lists 
> ol stands for ordered list which gives numbers 

```
<ol>
    <li>list item one</li>
    <li>list item two</li>
</ol>
```

> ul stands for unordered list

```
<ul>
    <li>list item one</li>
    <li>list item two</li>
</ul>
```

## Images and attributes

> `<img src="/folder/file.format" alt = "about the image" width = "500" height ="200">`

src and alt are called as attributes
- alt stands for alternative text , its very important for SEO

## Specify language  and charset

```
<html lang = 'en'>
<head>
    <meta charset = "UTF-8"/>
</head>
</html>
```

## Hyperlinks

> `<a href="url">click here<a>`

open in newtab

> `<a href='url' target='_blank'>click here</a>`

use `#` for empty href

## Page structuring

> `<nav></nav>`
> `<header></header>`
> `<article></article>`
> `<footer></footer>`
> `<aside></aside>` secondary content or information

## copyright symbol

html entity

> `&copy;` &copy;

## Semantic HTML
represents a meaning - all pages structuring are comes under semantic html



