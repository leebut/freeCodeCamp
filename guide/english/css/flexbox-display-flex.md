# Display Flex

A flexbox container can grow and shrink dynamically according to the size of the viewport.
To transform a CSS container into a flexbox container, we need to use ```display:flex;```.
Any elements nested inside the flex container will be displayed according to any attributes given to it.

![alt text](https://raw.githubusercontent.com/leebut/Flexbox-Images/master/flexcontainer.png "Flex container with nested flex items") 

**Example:**
CSS CODE
--------

```
.container {
  display: flex;
  background: yellow;
}
.box {
  background-color: brown;
  width: 200px;
  height: 200px;
  box-sizing: border-box;
  border: solid 1px black;
  color: white;
```
HTML CODE
---------
```
<div class="container">
  <div class="box">
    <p>Box 1</p>
  </div>
  <div class="box">
    <p>Box 2</p>
  </div>
  <div class="box">
    <p>Box 3</p>
  </div>
  <div class="box">
    <p>Box 4</p>
  </div>
</div>
```
Here's the result:
![alt text](https://raw.githubusercontent.com/leebut/Flexbox-Images/master/flex-direction-row.png "Container set to flex-direction: row;")

The normal behaviour of divs is for them to stack vertically, but ```display: flex;``` lays out the divs into a single horizontal row, along what is called the **main axis**, which runs horizontally from left to right. This is because the default direction of a flex container is ```flex-direction: row;```. It is behaving in the same way as ```float: left;```.

The other flex direction is _column_, and its main axis runs vertically from top to bottom.
The images below summarise the significance of the main axis, and they also show some alignment attributes.

![alt text](https://raw.githubusercontent.com/leebut/Flexbox-Images/master/main%20axis%20row.png "Row: the main axis")

![alt text](https://raw.githubusercontent.com/leebut/Flexbox-Images/master/main%20axis%20col.png "Column: the main axis")
