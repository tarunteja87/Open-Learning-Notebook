# Html and CSS
1. Webdesign
2. HTML
3. CSS
4. Responsive Design

> Reference Course [Build Responsive Real-world Websites with HTML and CSS](https://www.udemy.com/course/design-and-develop-a-killer-website-with-html5-and-css3/)

## Index
1. HTML Fundamentals
2. CSS Fundamentals
3. Building Layouts
4. Web design Framework
5. Components and Layouts 
6. OMINIFOOD : Desktop
7. OMINIFOOD : Responsive
8. OMINIFOOD : Optimization

## Some useful VS code extensions 
- prettier Code Formatter
- image preview
- color highligh
- Auto rename tag
- live server

# need to write notes 
- Box Shadow
- Box-sizing
- General reset (*)

## To make the header height to enire height of the view port
- view port is visible area of a page 
- `height:100% ` wont work
- by using new unit called `vh`  
```
height:100vh;
```
- `vw` is for view port width

# Responsive Design Principle
- Design technique to make a webpage adjust its layout and visual style to **any possible screen size** (window or viewport size)
- In practice , this means that responsive design makes websites usable on all devices , such as **desktop computers, tablets, and mobile phones**.
- Its a set of best practices, **not a seperate technology** its all just CSS!.

## Responsive Design Ingredients
1. Fluid layouts.
2. Responsive Units.
3. Flexible Images.
4. Media Queries.

### Fluid  Layouts
- To allow webpage to adapt to the **current Viewport** width (or even height)
- Use %(or vh / vw) unit instead of px for elements that should adapt to viewport
- USe max-width instead of width

### Responsive Units
- Use `rem` unit instead fo px for most lengths
- to make it easy to **scale the entire layout down** (or up) automatically.
- **Helpful trick** : setting 1rem to 10px for easy calculations.

### Flexible images
- By default , image **don't scale automatically** as we change the viewport, so we need to fix that.
- Always use % for image dimensions , together with the max-width property

### Media Queries
- Bring responsive sites to life
- To change CSS styles on **certain viewport widths** (called breakpoints)


## Desktop - first vs Mobile first development

### Desktop - first
- Start writing CSS for the desktop : **large screen**
- Then , Media queries **shrink design** to smaller screens.

### Mobile - first
- Start writing CSS for mobile devices : **small screen**.
- Then ,media queries **expand design to a large screen.
- Forces us to reduce websites and apps to the absolute essentials.

## How Rem and maxwidth property works
- `max-width : 1000px;`
### REM
- Root Elements Font-size REM
- one REM default = 16px 
- 50 rem = 50 X 16 = 800px
- if we want to change the default rem 

```
html
{
    font-size:10px;
    /* now one rem = 10px*/
}
```
- above method have some complications
- to over come those complications we use percentage instead of px
- 10px/16px = 0.625 =62.5% 
```
html
{
    font-size : 62.5%;
    /* this will respect the users browser font-size setting*/
}
