# Bootcamp-Project-Travelling-Circles 
# Sameer Ahmed
# Sameerahmed.210403@gmail.com 


float circleY; 
float yspeed=10;
float circleX; // create a variable circle X
float xspeed=10; // create variable xspeed=10
float x=200; // assigning a value to variable x 
float y=200; // assigning a value to variable y
float x1=200; 
float y1=200; 
float x2=200; 
float y2=200; 
float x3=200;
float y3=200;
void setup() {
 size(400,400); 
 circleX=0; // 
 circleY=0;
} 
void draw() 
{ background(255,0,0); // creates red background
fill(0,255,0); 
stroke(255); // adds black stroke
ellipse(circleX,height/2,60,60); // coordinates of circle    
fill(255,0,255);
stroke(255);
ellipse(width/2,circleY,60,60);

circleX= circleX + xspeed;
if(circleX>width){ 
  xspeed=-10;      // makes cirlce goes backward on the X-axis 
} 
circleY= circleY + yspeed;
if(circleY>height){ 
  yspeed=-10;  // makes circle goes donwards on the Y-axis 
} 
  fill(20,90,200);  
  noStroke(); 
ellipse(x,y, 60, 60); 
fill(200,90,20);  
  noStroke();
ellipse(x1,y1, 60, 60); 
  noStroke();
fill(255,255,0);
ellipse(x2, y2,60,60); 
  noStroke();
fill(0,255,255); 
ellipse(x3,y3,60,60);
x= x+2; 
y=y-2 ;  // (x,y)- goes to bottom right corner 
x1= x1+2; 
y1= y1+2; // (x1,y1)- goes to top right corner 
x2= x2-2; 
y2= y2-2; // (x2,y2)- goes to bottom left corner
x3= x3-2; 
y3= y3+2; // (x3,y3) goes to top left corner
}
