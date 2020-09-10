# Lab1C-Processing-Exercises
Some basic processing exercises and an example. 

## Includes
- Float vs. int declaration
- global variables
- variables instead of hardcoding
- documenting code
- changing size & shape based off of a scalar. 

## Exercise 
1. In `1AC-*YOUR FIRST NAME*-*YOUR LAST NAME*`, start a processing document. 
2. In the comment section at the top, include the lab number, your name, and a description of what you are drawing.
```processing
/*  Lab 1AC 
    Katarina Hoeger
    
    Scale many shapes example 
    - contains scaled ellipse
    - contains scaled rectangle
    - contains scaled triangle
*/
```
3. Set up your drawing area (size & background color). Add any extra default settings here.
```processing
/*  Lab 1AC 
    Katarina Hoeger
    
    Scale many shapes example 
    - contains scaled ellipse
    - contains scaled rectangle
    - contains scaled triangle
*/

void setup(){
  // drawing surface size and color
  size(1000, 1000);
  background(0, 0, 0);
  
  // initial settings
  noStroke();           // no object outlines
  ellipseMode(CENTER);  // draw ellipses from center
  rectMode(CENTER);     // draw rectangles from center 
}
```
4. Draw & fill a shape, placing it somewhere specific on the canvas. Comment it.
```processing
/* Lab 1AC
Katarina Hoeger
Scale many shapes example 
- contains scaled ellipse
- contains scaled rectangle
- contains scaled triangle
*/

void setup(){
  // drawing surface size and color
  size(1000, 1000);
  background(0, 0, 0);
  
  // initial settings
  noStroke();           // no object outlines
  ellipseMode(CENTER);  // draw ellipses from center
  rectMode(CENTER);     // draw rectangles from center 
}

void draw(){
  // set fill color
  fill( 255, 0, 0, 200);
  
  /* Since this is an example, I will draw 1 of each shape.
  I need an example for each shape. You just need one shape. 
  Do not just copy my example - use the same technique, make your shape and placement. 
  Use colors. Place shapes anywhere on the canvas.
  Feel free to have fun with this exercise. */
  
  // ellipse
  ellipse( 100, 100, 100, 100); // (x, y, r1, r2)
  
  // rectangle
  rect( 100, 500, 100, 100);   // (x, y, w, h)
  
  // triangle
  triangle( 50, 950, 100, 850, 150, 950);
}
```
5. Pick one part of the definition of the shape, not of the location. 
If it's an ellipse, choose at least one radius. 
If it's a rectangle or triangle, one leg. 
Define it in terms of global variables.
Comment those.
Run code to make sure everything still works.
6. Add a scalar global variable. Comment. Scale the shape with every run through draw.
7. Make a color changing scalar, and change the color with every run through draw. 
If the last scalar was a float, make this one an int and vice versa
8. Play with the variables. Get comfortable. Have fun with it. Turn in an example you are proud of. Can use multiple shapes.

## Example Submission
[Lab 1AC Example Submission](https://github.com/UMaine-NMD-211-Fall-2020/Lab1AC-ExampleFolder) - it has a typo 
in the processing file's comments, but apart from that, should work as a reference


