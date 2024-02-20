# Cheatseet for CSS

```<link href="./path/to/stylesheet/style.css" rel="stylesheet" type="text/css">```

## 1 Sintax and selectors
#### ```.class-name { property: value; }``` Class scope
#### ```#id-name { property: value; }``` Single element scope by ID
#### ```* { property: value; }``` All elements
#### ```element { property: value; }``` Element scope
#### ```element.class-name { property: value; }``` Element and class scope
#### ```element#id-name  { property: value; }``` Element and ID scope
#### ```element, element { property: value; }``` Multiple selectors
#### ```element element { property: value; }``` Descendant (one elemenent followed by the other)
#### ```selector { property: value !important; }``` Important takes precedence

## 2 Visual rules

#### ```color: #fff;``` color, rgb(255, 255, 255), rgba(255, 255, 255, 0.5), hsl(0, 0%, 100%), hsla(0, 0%, 100%, 0.5)
#### ```background-color: #000;``` color, rgb(0, 0, 0), rgba(0, 0, 0, 0.5), hsl(0, 0%, 0%), hsla(0, 0%, 0%, 0.5)
#### ```font-size: 30px;```
#### ```font-weight: bold;``` normal, bold, bolder, lighter, 100, 200, 300, 400, 500, 600, 700, 800, 900
#### ```text-align: right;``` left, right, center, justify
#### ```opacity: 0.5;``` from 0 to 1

### 2.1 Backgrounds
#### ```background-color: #000;``` color, rgb(0, 0, 0), rgba(0, 0, 0, 0.5), hsl(0, 0%, 0%), hsla(0, 0%, 0%, 0.5)
#### ```background-image: url('./path/to/image.jpg');``` url, linear-gradient(to right, #000, #fff), radial-gradient(#000, #fff)
#### ```background-size: cover;``` cover, contain
#### ```background-position: center;``` top, right, bottom, left, center
#### ```background-repeat: no-repeat;``` repeat, no-repeat, repeat-x, repeat-y
#### ```background-attachment: fixed;``` fixed, scroll
#### ```background: #000 url('./path/to/image.jpg') no-repeat center/cover;``` color image repeat position/size

## 3 The box model
#### ```box-sizing: border-box``` content-box is default, border-box when padding+border is needed
#### ```margin: auto``` for centering
#### ```overflow: scroll``` visible, hidden, scroll, auto
#### ```display: flex``` flex, inline-flex
#### ```min-[width|height]: 100px``` in px, em
#### ```max-[width|height]: 100px``` in px, em
#### ```width: 100px``` in px, em
#### ```height: 100px``` in px, em
#### ```padding: 10px``` in px, em
#### ```margin: 10px``` in px, em
#### ```border: 1px solid #000``` width style color

#### ```margin-[top|right|bottom|left]: 10px``` in px, em
#### ```padding-[top|right|bottom|left]: 10px``` in px, em
#### ```border-[top|right|bottom|left]-[width/color/style]: 10px solid #000``` width color style
#### ```border-top-style: solid``` none, hidden, dotted, dashed, solid, double, groove, ridge, inset, outset
#### ```border-radius: 10px``` in px, em
#### ```border-[top|bottom]-[left|right]-radius: 10px``` in px, em
#### ```border-top: 10px solid #000``` width style color
#### ```box-shadow: 10px 10px 10px #000``` horizontal vertical blur color inset

#### ```visibility: hidden;``` hidden, visible

# 4 Display and positioning

#### ```position: relative;``` relative, absolute, fixed, sticky
#### ```display: none;``` none, block, inline, inline-block, flex, grid
#### ```float: left;``` left, right
#### ```clear: left;``` left, right, both, none
#### ```top: 10px;``` in px, em
#### ```right: 10px;``` in px, em
#### ```bottom: 10px;``` in px, em
#### ```left: 10px;``` in px, em
#### ```z-index: 10;``` negative and positive numbers
#### ```overflow: hidden;``` hidden, visible, scroll, auto
#### ```cursor: pointer;``` pointer, default, help, wait, text, move, not-allowed, crosshair, e-resize, n-resize, ne-resize, nw-resize, s-resize, se-resize, sw-resize, w-resize

# 5 Colors
#### ```color: #fff;``` color, rgb(255, 255, 255), rgba(255, 255, 255, 0.5), hsl(0, 0%, 100%), hsla(0, 0%, 100%, 0.5)
#### ```background-color: #000;``` color, rgb(0, 0, 0), rgba(0, 0, 0, 0.5), hsl(0, 0%, 0%), hsla(0, 0%, 0%, 0.5)

# 6 Typography

#### ```font-family: 'Helvetica', 'Arial';``` Verdana, Tahoma, Times New Roman, Geooria, Courier New,
#### ```font-size: 16px;``` in px, em
#### ```font-weight: 700;``` from 100 to 900 (lighter 100, normal 400, bold 900)
#### ```font-style: italic;``` italic, normal,
#### ```line-height: 1.5;``` in unitless, px or em
#### ```text-align: center;``` left, right, center, justify
#### ```text-decoration: none;``` none, underline, overline, line-through
#### ```text-transform: uppercase;``` uppercase, lowercase, capitalize
#### ```letter-spacing: 1px;``` in px, em
#### ```word-spacing: 2px;``` in px, em
#### ```text-indent: 20px;``` in px, em
#### ```font-size: 16px;``` in px, em

Declaration new font:
#### 
```
@font-face {
  font-family: 'Open Sans';
  src: url('../fonts/OpenSans-Regular.ttf');
}
```

#### Using it inside < head >
```<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@100&display=swap" rel="stylesheet">```

# 7 Flex

#### ```display: flex;``` flex, inline-flex
#### ```flex-direction: row;``` row, row-reverse, column, column-reverse
#### ```flex-wrap: wrap;``` wrap, nowrap, wrap-reverse
#### ```justify-content: center;``` Position H: flex-start, flex-end, center, space-between, space-around
#### ```align-items: center;``` Position V: flex-start, flex-end, center, baseline, stretch
#### ```align-content: center;``` flex-start, flex-end, center, space-between, space-around, stretch
#### ```flex-flow: row wrap;``` direction wrap
### 7.1 Flex items
#### ```order: 1;``` in numbers. 0 Default. -1 First: 1 Second: 2
#### ```flex-grow: 1;``` in numbers
#### ```flex-shrink: 1;``` in numbers
#### ```flex-basis: 100px;``` in px, em, %
#### ```flex: 1 1 100px;``` grow shrink basis
#### ```align-self: center;``` flex-start, flex-end, center, baseline, stretch

# 8 Grid

#### ```display: grid;``` grid
#### ```grid-template-columns: 100px 100px 100px;``` in px, em, %
#### ```grid-template-rows: 100px 100px 100px;``` in px, em, %
#### ```grid-template-areas: "header header header" "main main main" "footer footer footer";```
#### ```grid-template: 100px / 100px 100px 100px;``` rows / columns
#### ```grid-column-gap: 10px;``` in px, em
#### ```grid-row-gap: 10px;``` in px, em
#### ```grid-gap: 10px 20px;``` row column
#### ```justify-items: center;``` start, end, center, stretch
#### ```align-items: center;``` start, end, center, stretch
#### ```place-items: center center;``` align-items justify-items
#### ```justify-content: center;``` start, end, center, stretch, space-around, space-between
#### ```align-content: center;``` start, end, center, stretch, space-around, space-between
#### ```place-content: center center;``` align-content justify-content
### 8.1 Grid items
#### ```grid-column: 2 / 4;``` start / end
#### ```grid-row: 2 / 4;``` start / end
#### ```grid-area: header;``` name




