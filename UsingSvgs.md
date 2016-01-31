#SVG Basics
Scalable Vector Graphics are not only 'Scalable', they are powerful. Why are they powerful? They are defined in XML and as such every part is addressable through CSS an JS. This means that we can take a single SVG and not only morph it's size, but everything about it. In this tutorial, I will not get remotely close to the endless capabilities of SVGs, but hope inspire further investigation and creativity on your part by showing how easy they are to use. See [MDN](https://developer.mozilla.org/en-US/docs/Web/SVG/Element) to explore vastness of this useful technology.
##The Canvas
You may be familiar with the canvas element in HTML5. I like to see the SVG element in similar fasion. The SVG element is filled with other elements, that each can be manipulated together or individually providing an endless palette of possibilities.
Setting up that canvas is as simple as this ```<svg width="300" height="300"></svg>```. Just like that we have an 300X300px area to place a multitude of graphical interaction. We can add an id address it with JavaScript, and we can give it a class to manipulate it with CSS. ```<svg id="mySvg" class="svgClass" width="300" height="300"></svg>```. And of course we can do the same with the elements we place inside.
###Sizing Things Up
The figure below depicts the coordinates of a 300X300 svg. We use this system for placing our inner elements.

![image of svg coordinates](svgArea.svg.png)

This next figure shows a rectangle defined within the SVG. As you can see, the x and y attributes of the rectangle place the upper left corner at the intersection of 10,10 inside the SVG. A circle by contrast

![image inner element coordinates alignment](svgXY.svg.png)