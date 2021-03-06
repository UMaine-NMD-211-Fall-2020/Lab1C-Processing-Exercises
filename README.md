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
  triangle( 50, 950, 100, 850, 150, 950); //(x1, y1, x2, y2, x3, y3)
}
```
5. **OPTIONAL STEP** (skipped in this example - need not define in terms of global variables. It would make it easier to move everything. ) Pick one part of the definition of the shape, not of the location. 
If it's an ellipse, choose at least one radius. 
If it's a rectangle or triangle, one leg. 
Define it in terms of global variables.
Comment those.
Run code to make sure everything still works.
6. Add a scalar global variable. Comment. Scale the shape with every run through draw.
```processing
/* Lab 1AC
Katarina Hoeger
Scale many shapes example 
- contains scaled ellipse
- contains scaled rectangle
- contains scaled triangle
*/

/* !!!!!! --- CHANGES HERE !!!! --- */
// scalars
float small = 0.5;
int med = 2;
int huge = 10;

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
  
  /* !!!!!! --- CHANGES HERE !!!! --- */
  // ellipse
  ellipse( 100, 100, 100, small*100); // (x, y, r1, r2)
  
  /* !!!!!! --- CHANGES HERE !!!! --- */
  // rectangle
  rect( 100, 500, 100, med*100);   // (x, y, w, h)
  
  /* !!!!!! --- CHANGES HERE !!!! --- */
  // triangle
  triangle( huge*50, 950, huge*100, 850, huge*150, 950); // (x1, y1, x2, y2, x3, y3)
}
```
7. (OPTIONAL) Make a color changing scalar, and change the color with every run through draw. 
If the last scalar was a float, make this one an int and vice versa
8. Play with the variables. Get comfortable. Have fun with it. Turn in an example you are proud of. Can use multiple shapes.  Play with it until you understand how to put the graphics where you want, at the scale you want. 

*The example code below shows you don't need to do much to make interesting graphics*
```processing
/* Lab 1AC
Katarina Hoeger
Scale many shapes example 
- contains scaled ellipse
- contains scaled rectangle
- contains scaled triangle
*/

// scalars
float small = 0.5;
int med = 2;
int huge = 10;

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
  /* Since this is an example,
  I will draw 1 of each shape 
  I need an example for.
  You just need one shape. */
  
  // --- ellipse 
  // set fill color
  fill( 255, 0, 0, 100);
  // left
  ellipse( 100, 100, 100, small*100); // (x, y, r1, r2)
  // center
  ellipse( 500, 100, 100, med*100);
  // right
  ellipse( 900, 100, 100, huge*100);
  
  // --- rectangle
  // set fill color
  fill( 100, 255, 200, 100);
  //left 
  rect( 100, 500, 100, med*100);   // (x, y, w, h)
  //center
  rect( 500, 500, 100, huge*100);
  //right
  rect( 900, 500, 100, small*100);
  
  
  // --- triangle
  // set fill color
  fill( 200, 100, 255, 100);
  // left
  triangle( huge*50, 950, huge*100, 850, huge*150, 950); // (x1, y1, x2, y2, x3, y3)
  // center <- ends up leftmost due to scalar
  triangle( small*50, 950, small*100, 850, small*150, 950);
  // right  <- ends up middle due to scalar
  triangle( med*50, 950, med*100, 850, med*150, 950);
}
```
![Image generated by code above - collection of geometric shapes in red, teal, purple](scaledShapes.jpg)
## Extra Example Submission
[Additional Lab 1AC Example Submission, with global variables defining everything and changing sizes and colors.](https://github.com/UMaine-NMD-211-Fall-2020/Lab1AC-ExampleFolder) - this is an advanced example of what can be done

## Student Lab Submission links
Link to your lab below, as shown in my example. 
- [1AC-Katarina-Hoeger](https://github.com/UMaine-NMD-211-Fall-2020/Lab1AC-ExampleFolder) 
