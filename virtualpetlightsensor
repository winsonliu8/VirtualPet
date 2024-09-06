import processing.serial.*;
import cc.arduino.*;
Arduino arduino;

void setup(){
  size(500,500);
  arduino = new Arduino(this, Arduino.list()[1], 57600); //change the [0] to a [1] or [2] etc. if your program doesn't work
}


void draw(){
 /*cursor coordinate code
  background(255);
  fill(10, 9, 4);
  text(mouseX, 5, 20);
  text(mouseY, 30, 20);
 */
 
  background(237, 226, 201);
 
 
//head
fill(137, 121, 121);
noStroke();
ellipse (120, 200, 135, 120);


//eyes

 
  int w = arduino.analogRead(5); //5 is light
  int h = arduino.analogRead(5); //5 is light

  if (w>40){
    w=40;
    h=40;
  System.out.println(w);
  System.out.println(h);
  }
 

fill(0);
ellipse(95, 207, 20+h, 20+w);

fill(255);
ellipse(95, 209, 6+h, 6+w);

//beak
pushMatrix();
fill(201, 186, 128);
//change point of rotation to that spot
translate(width/5, height/2); 
rotate(radians(20));
rect(0, 0, 20, 101);
popMatrix();

//sharp part beak
fill(201, 186, 128);
triangle(70, 357, 85, 351, 66, 344);

//body
fill (137, 121, 121);
ellipse(320, 145, 280, 240);

//neck
fill (137, 121, 121);
rect (151, 157, 120, 90);

//thigh
fill (137, 121, 121);
ellipse(327, 250, 105, 85);

//legs
fill(10, 9, 4);
stroke(1);
strokeWeight(10);
line(323, 296, 291, 346);
line(359, 283, 390, 336);

//toes
fill(255);
stroke(1);
strokeWeight(10);
line(291, 346, 240, 337);
line(291, 346, 262, 371);
line(291, 346, 293, 383);

line(390, 336, 367, 369);
line(390, 336, 388, 383);
line(390, 336, 433, 347);

//kiwi
pushMatrix();
fill(130, 242, 143);
stroke(219, 173, 73);
translate(width/40, height/2.2); 
rotate(radians(15));
arc(150, 150, 130, 140, 0, PI);
popMatrix();

//seeds
fill(5, 2, 2);
noStroke();
ellipse(82, 419, 10, 10);
ellipse(99, 419, 10, 10);
ellipse(112, 431, 10, 10);
ellipse(131, 426, 10, 10);
ellipse(152, 432, 10, 10);

}






/*rotate(radians(-10));
for ellipse
first value is x coordinate
second value is y coordinate
third is how much it stretches horizontally
fourth is how much stretch vertical */
