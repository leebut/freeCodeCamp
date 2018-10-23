---
title: Flex Basis
---

# Flex-basis

To determine the initial width or height of a flex element along the main axis, we can use ```flex-basis:``` instead of ```width:``` or ```height:```. ```flex-basis:``` is dynamic, so it can shrink or grow to fit inside the flex container.
```flex-basis:``` can be set as a value, e.g. ```200px;``` ```20vw;``` ```50vh;``` or ```auto```. Auto will assess the contents of the flex item and expand or contract with them. Example 1 shows a nested div with ```flex-basis: 20vw;```, while the second and third use ```flex-basis: auto;```.

**Example 1:**
```css
.container {
display: flex;
flex-direction: row;
justify-content: center;
background-color: yellow;
}
.box {
background-color: brown;
flex-basis: 20vw;
height: 200px;
box-sizing: border-box;
border: solid 1px black;
color: white;
}
```
```html
<div class="container">
<div class="box">Box 1</div>
</div>
```
![text alt](https://raw.githubusercontent.com/leebut/Flexbox-Images/master/flex-basis-20vw.png "flex-basis: 20vw;")

**Examples 2 and 3:**
```css
.box {
background-color: brown;
flex-basis: auto;
height: 200px;
box-sizing: border-box;
border: solid 1px black;
color: white;
}
```
![text alt](https://raw.githubusercontent.com/leebut/Flexbox-Images/master/flex-basis-auto-shrank.png "flex-basis: auto;") 

![text alt](https://raw.githubusercontent.com/leebut/Flexbox-Images/master/flex-basis-auto-resized-to-longer-content.png "flex-basis: auto;") 
