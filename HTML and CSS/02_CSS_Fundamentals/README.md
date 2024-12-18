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

# LAYOUTS : Floats, Flexbox,and CSS Grid Fundamentals
- layout is the way text, images and other content is placed and arranged on a webpage
- Layout gives visual structure
- page layout and component layout.

The 3 ways of building layouts with CSS
1. Float layout
2. Flexbox 
    - Modern way of laying out elements in a 1-dimentional row without using floats.
    perfect for component layouts.
3. CSS Grid
    - For laying out elemet in a fully-fledged 2-dimentional grid. Perfect for page layouts and complex components.

## Floats
> float:left;
  float:right;

- Element is removed from the normal flow : **out of** flow
- Text and inline elements will wrap around the floated element
- The container will **not** adjust its height element.
- if you want to add margin for the element next to float element , there will be some conflit like marging will overlaping with flot element
- to fix we need to float the another element as well 

**Colapsing elements**
Consider a container having two elements - if both the elements  having the property flot , then the container looses its height 

**How to clear floats**
- by adding an element with empty content in the container and add css property as below

```
clear :both;
```

**another technique** is clear fix ( to avoid empty divs)
 - add a class name `clearfix` to the main cointainer
 - add css as shown below
 ```
 .clear::after
 {
    clear :both;
    content :'';
    display : block;
 }
 ```

**box-sizing**
box-sizing helps to hold the width even when you add padding and not for margin 
- final width = exactly same width what we have applied for the element
`box-sizing:border-box`
`box-sizing: content-box`

## Flexbox
lets consider a main container having 5 sub container , if we apply the `display : flex` property to the main container then all the subcontainer takes the place horizontally , which is needed by the elements in the subcontainers. and height will be as per the highest height of the sub container

- One the most useful application is `vertical centerig`
 to center all the items vertically , all we need to do is 
 `align-items:center`
 - to put them at very start `align-item:flex-start`
 - to put them at the buttom `align-item:flex-end`
 - default is `stretch`

 - to put the sub container to be `Center` in the main cointainer `justify-content:center`
 - `justify-content:space-between` will equally distribute the remainig space in between elements
 ### Flexbox overview
 - Flexbox is a set of related **CSS properties** for **building 1-dimensional layouts**.
 - the main idea behind flex box is that empty space inside a container element can be automatically divided by its child elements.
 - Flexbox makes it easy to automatically align items to one another inside a parent container , both horizontally and vertically.
 - flexbox solves common problems such as vertical centering and creating equal height columns.
 - Flexbox is perfect fro replacing floats , allowing us to write fewer and cleaner HTML and CSS code
 ### Flexbox terminology
 - the element which we want to use flex box is called `flex cointainer`
 - to create a flex cointainer , we need to add  display property to flex `display:flex`.
 - Direct children of flex cointainer is called `flex items`
 - the direction in which the flex items are laid out is called `main axis`
 - another perpendicular axis simply called the `cross axis`

 > flex container
 1.  gap : 0
 to create `space between items`, with out using margins
 2. justify-content:flex-start , flex-end, center , space-between , space around , space evenly - to align items along main axis (horizontally, by default)
 3. align-items:stretch , flex-start. flex-end, center , baseline - to align items along cross axis (vertically , by default)
 4. flex-direction:row , row-reverse, colum column-reverse - to define which is the main axis
 5. flex-wrap :nowrap , wrap , wrap reverse - to allow items to wrap into a new line if they are too large
 6. align-content :stretch , flex-start, flex-end, center , space-between , space-around - only applies when there are multiple lines (flex-wrap:wrap)

 >flex item
 1. 

