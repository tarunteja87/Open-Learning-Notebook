# CSS stands for Cascading Style Sheet

- Css describes the visual style and presentation of the content written in html
- CSS consists of countless properties that developers use to format the content , properties about font, text, spacing ,layout, etc.


## Typical css code 

```
h1 {
    color : blue;
    text-align :center ;
    font-size :20px;
}
```
- `h1` is called *selector*
- `font-size` - property   `20px` - value 
- property + value = Declaration /Style
- { declaration Block}


## Inline , internal and External CSS

> Inline  `<h1 style="color: aqua;">The Code Bro</h1>`

> Internal css ```<style>
        h1
        {
            color: blueviolet;
        }
    </style>
    ```

> external css `<link rel="stylesheet" href="style.css">`

## Styling Text
```
h1
{
    color: brown;
    font-size: 100px;
    font-family: 'Courier New', Courier, monospace;
    text-transform: uppercase;
    font-style: italic;
}
```
- inherit 
- default font size is 16px

## Combining Selectors
```
h1, h2, h3, h4, p 
{
    font-family : <something>
}
```

## decendent selector

```
footer p {
    font-size :60px;
}
```

## Id 
> attribute id `<p id = 'author'>some paragraph</p>`
  ```
  #author{
    font-style : italic;
  }
  ```

## Vs code to comment 
> `ctrl+/`

## Class
> `<p class='class_author'>some para</p>`
``` .class_author{
    font-weight : bold;
}
```

- difference betwenn Id and class is we are not allowed to repeat id names , but classes we can use 

- using class is a best practice

# Working with colors
## RGB Model
- Each of the 3 base colors can take a value between 0 and 255 , which leads to 16.8 million different colors.
- pure red `255 0 0`
- pure green `0 255 0`
- pure blue `0 0 255`
- white `255 255 255`
- black `0 0 0`

## Defining colors in CSS
- RGB /RGBA notations
> rgb(0,255,255)
- RGB with transprancy
> rgba(0,255,255,0.3)
- Hexadecimal
> #00ffff
-Shades of grey
>rgb(0,0,0)
>#fff
>#000


- background color
`background-color:red;`

- border
`border: 5px solid blue;` shorthand
border width + border type + border color

```
border-top : 5px solid color;
border-buttom :
border-left :
border-right :
```
## pseudo classes
```
li:first-child
li:last-child
li:nth-child(2)
li:nth-child(odd)
```

## Styling Hyperlinks
```
a:link{
    color : #0ff;
    text-decoration: none;
}
```

```
a:visited{
    color: 000;
}
```

```
a:hover
a:active

L  V  H  A - order
```

## Using Chrome Dev tools


