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
Link - Visited - Hover - Action
```

## Using Chrome Dev tools
-  Inspect 
- hover

## CSS Theory 1 -CONFLICTS BETWEEN Selectors
- what happen when multiple css rules applied to a element

```
<p id="author-text" class= "author">
    posted by Tarun teja on 16-12-2024
</p>
```

```
.author {
    font-style : italic;
    font-size : 18px;
}

#author-text {
    font-size : 20px;
}

p, li {
    font-family : san-serif;
    color : #444444
    font-size :22px;
}
```
> * There are multiple selectors selecting the same element . Which one of them applies? *
  All of them. All rules and properties are applied !

- ~ Highest priority   to   Lowest priority ~
  ```
  5. Declarations marked !important
  4. Inline style (style attribute in HTML)
  3. ID (#) selector
  2. Class (.) or pseudo-class (:) selector
  1. Element selector (p,div,li,etc.)
  0. Universal selector (*)
  ```
if Multiple - Last selector in code applies

> if you add `!important` for any of the property - then the priority is very high

##  CSS Theory 2 - INHERITANCE and universal Selector

- some properties are inherited from the main element 
  eg: if a color property added to body will apply to all the elements present in the body
- only few properties will inherit (mostly related to text will inherits
)  

## CSS BOX MODEL (IMP)
- **CONTENT** : Text , images,etc.
- **Border** : A line around the element , still inside of the element.
- **Padding** : Invisible space around the content , inside of the element.
- **Margin** : Space outside element , between elements
- **FillArea** : Area that gets filled with background color or background image

### Height and width calculation
- **Final element width** = left border + left padding + width + right padding + right border
- **Final element height** = top border + top padding + height + bottom padding + bottom border
## Margins and padding
```
padding :50px ;
padding-left : 10px;
padding-right : 20px;
padding-top : 20px;
padding-buttom : 30px;
```

- shot hand 

``` padding : 20px; /* applies to all the sides */ 
    
    padding : top&bottom  left&right;
    
    top  right  buttom left

    top left&right buttom
```

#### Reset all the default margins and paddings 
 ``` * {  
            margin :0;
            padding  : 0;
         }
 ```
 #### margin Collapsing
consider two elements 
 - element 1   and element 2
 lets say element 1 having bottom margin of 20px  and element 2 having top margin of 20px , then the distance between element 1 and element 2 is 20px but not 40px

## Adding Dimensions
> width : 500px;
  Height : 100px;

  height : auto;
  width : 100%; /* responsiveness */

## Centring page
> a  trick to center a page is put all the content you want to center in a container
  
  ``` .container{
    width : 700px;
    margin-left :auto ;
    margin-right : auto;
  }
   ```
> we can't add margins for small elements like `a`. 

## Types of boxes
### Block-level boxes
> - Elements formatted visually as blocks 
  - 100% of parents width
  - vertically , one after another
  - Box-model applies as showed
  - to change any elemnet to block use   `display : block;`
### Inline Boxes
> - Occupies only content's space
  - cause no line - breaks
  - Box model is different :height and widths do not apply
  - paddings and margins only horizontal (left and right)
  - to change any element to inline - use `display : inline`
### Inline - Block Boxes
> - Looks like inline from the **outside** , behaves like block -level  on the **inside**
  - Occupies only content's space
  - cause no line - break 
  - box model applies as showed
  - `display : inline-block`

> you can chane any two pseduo classes as mentioned `a:link:lastchild {   }`

- `img` is a `inline-block` element

## Absloute postioning (very important)
### Normal Flow
- Default positioning
- Element is **in** flow
- elements are simply laid out according to the  HTML code
> position : relative

### Adsloute positioning
- element is removed from the normal flow :**Out of flow**
- No impact on surrounding elements ,might overlap them
- we use Top , bottom , left , or right to offset the element  from its **relatively positioned container**
> position : absolute;
  top : 0
  buttom : 0
  left :0
  right :0+

> to use adbloute - the parent positioin should be relative

- we use absloute positioning for single elements like chat bot at corner.

## Pseudo elements
- pseudo elements are essiential elements that doesnt exists in the HTML but still we can select and style in css.
> eg :first letter of a paragraph or file line of a paragraph
 ```
 h1::first-letter{
    font-style: normal;
    margin-right :5px;
 }
p::first-line{
    color:red;
}
```
Adjacent elements 

```
h3 + p::first-line{
    color : red /* change p color adj to h3 */
}
```
top post label 
```
h1::after{
    content : "TOP";
    background-color : ffe70;
    font-size:16px ;
    font-weight : bold ;
    display : inline-block;
    position : absloute;
    top : -5px;
}  
```
## Developer Skills : Googling  and Reading Documentation
- use `css property to add a mouse cursor to a button` stack overflow.com 
- css-tricks.com
- MDN Documentation


