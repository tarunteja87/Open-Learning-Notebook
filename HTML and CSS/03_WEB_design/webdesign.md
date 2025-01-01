# Web design
- `span` is a generic iline element 
- `blockquote`

> WEB DESIGN VS DEVELOPMENT
- Web designers create the overall **look and feel** of a website.
- web developer implements the design using **Html, css and JS**

## Good Design vs Bad Design
### Good Design 
- Good Impression 
- Trust
- Percieved value
- Good design gives exactly **What they want**

### Bad Design
- Makes users believe that brand doesnt care
- make users insecure
- cheap
- Leaves user confused

> Any one can learn Good Design by following a framework/system

## Ingredients
1. Typography
2. colors
3. images /illustrations
4. icons
5. shadows and border-radius
6. whitespace
7. visual hierarchy
8. user experience
9. components and layouts

## Website Personalities
1. **Serious/elegant** : for luxury and elegance, based on thin serif typefaces, golden or pastel colors, and big high-quality images
2. **Minimalist/Simple** : Focusses on the essential text context , using small or medium -sized sans-serif black text, lines and few images and icons
3. **Plain /Neutral** : Design that gets out of the way by using neutral and small typefaces, and very structured layout. common in big corporations (microsoft / adobe)
4. **Bold/confident** : Makes impact, by featuring big and bold typography, paired with confident use of big and bright colored blocks
5. **Clam/Peaceful** :For Product and services that cares , transmitted by calming pastel colors, soft serif headings , and matching images/illustrations
6. **Startup/Upbeat** : Widely used in startups , Featuring medium-sized sans-serif typefaces , light-grey text and backgrounds , and rounded elements.
7. **Playful/fun** : Colorful and round designs , fueled by creative elements like hand-drawn icons or illustrations, animations , and fun language


## Typography
- Typography is the art and technique of arranging type to make written language legible, readable and appealing when displayed
### Serif vs san-serif
- serifs (having some tails called serifs)
- creates a traditional classic look and feel
- conveys trustworthiness
- Good for long text
- sans -serif ( will not have any type face)
- looks very clean and simple
- Modern look and feel
- Easier to choose for begineer designer
(sans-serifs is good for beginers)

### Rules for Typhography (USE GOOD TYPEFACES)
- use only good and popular typefaces and play it safe.
- **INTER** , **Open sans** , **Roboto** , **Montserray** , **Work sans** , **Lato** (SANS-SERIF)
- **Merriweather , Aleo , Playfair Display , Cormorant , Cardo , Lora**
- its okay to use just one typrface per page ! if you want more limit to 2.
### Font sizes and weights
- When choosing font-size, **Limit choices!** Use a **Type scale tool** or other **Pre -defined range**
- Use a font size between **16px and 32px** for **Normal text**
- For **Long text** (like a blog post), try a size of 20px or even bigger
- For Headings , you can go really big (50px+) and blod (600+), depending on personality.
- For any text , don't use a font weight under 400(regular)
### Create a Good Reading experience
- use less than 75 chars per line
- For normal-sized text , use a line height between 1.5 and 2. For big text , go below 1.5
 - smaller or longer the text , the larger the line height needs to be
- Decrease letter spacing in headlines , if it looks unnatural
- Experiment with all caps for short titles. Make them small and bold and increase letter-spacing
- Usually , don't justify text
- don't center long text blocks . small blocks are fine.
- **External fonts need to be place before the CSS link**
```
font-family :'Inter', sans-serif;
```
[typescale.com](typescale.com)

## Color
### Choosing the right color 
Make the main color match your website personality : colors convey meaning.
- **RED** draws a lot of attention , and symbolizes power, passion, and excitement.
- **Orange** is less aggressive , and conveys happiness, cheerfulness, and creativity.
- **Yellow** Means joy , brightness, and intelligence.
- **Greens** represents harmony, nature , growth and health.
- **Blues** is associated with peace, trustworthiness, and professionalism.
- **Purple** Conveys wealth, wisdom, and magic.
- **Pink** represents romance, care, and affection.
- **Brown** is associated with nature, durability and comfort.
- **Black** symbolize power, elegance and minimalism, but also grief and sorrow.

Use a good color tone , Don't choose a random tone or CSS named colors  
- **Open color**
- **tailwindcss**
- **Flat ui colors 2**
### Establish a color system
- You need at least two types of colors in your **colour palette** : a **main color** and a **grey color**
- Accent color - to choose accent color (**accent colors**) tool (**palleton.com**) (**COOLORS**)
- for diversity , create lighter and darker versions (tints and shades)  - tints means lighter color - shades means darker colors (**Tint&shadegenerator**)
- Use colors to add interesting accents or make entire components or sections stand out
- you can use color strategicallly in images and illustrations

### Relation Between COLOR and TYPOGRAPHY
- on dark colored backgrounds , try to use a tint of the background ("lighter version") for text
- Text shouls usually not be completely black . Lighten if up it looks heavy and uninviting
- Dont make text too light ! use a tool to check contrast between text and backgriund colors
- contrast ratio needs to be at least 4.5:1 for normal text and 3:1 for largr tet(18px+) (tool : **Coolors**)
 
## Images and illustrations

### Use Good Images
- Different types of images :**Product photos, storytelling photos, illustrations, patterns**
- Use images to support your websites **message and story**. so only use **relevant images**.
- Prefer **Original images** . If possible , use **original-looking** stock images(not generic ones)
- Tool box (**Unsplash , Pexels , DrawKit, unDraw**)

### Use images well
- Try to show **Real people** to trigger users emotions
- If necessary , **crop images** to fit your message
- Experiment **combining** photos, illustrations and patterns 

### Handrling Text on Images
- **Method 1:** Darkrn or briten images (completely or partially , using a gradient)
- **Method 2:** Position text into neutral image area
- **Method 3:** Put text in a box

### Some technical details 
- To Accounr for High resolutioin screens , amke image dimensions **2x as big** as their displayed size
- **Compress images** for a lower file size and better performance
- tools for image compression (**Unsplash , pexels , drawkit , undraw and Sqoosh(recomended)**)
- when using multiple images side-by-side , make sure they have exact same dimensions


## icons
### use good icons
- Use a good icon pack , there are tons of free and paid icon packs 
- tools (**ionicons , phosphor icons, icons8**)
- only use one icon pack , **Dont mix** icons from different icon packs
- Use **SVG** icons or icon fonts . Dont use bitmap images formats(.jpg and .png)
- Adjust to website personality **Roundness, weight and filled/outlined** depend on typography.
### When we can use icons
- use icons to **provide visual assistance** to text.
- use icons for **Product feature blocks**
- use icons **associated with actions** and **label them** (unless no space or icon is 100% clear)
- use icons **as bullet points**
### Use icons well
- To keep icons neutral , **use same color as text** . To draw more attention , **USe different color**
- Dont confuse your users : icons need to make sense and fit the text or action.
- Dont make icons larger than what they **Were designed for** ,if needed **Enclose them into shape**.
