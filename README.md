# Ejercicio-5
Composición (for, interacción con el mouse)


void setup(){
size(700,675);

}

void draw(){
  background(177,126,73);
      for(int beex=50; beex<650; beex= beex + 100){
        for(int beey=50; beey<650; beey= beey + 100){
          for(int colmx=55; colmx<650; colmx= colmx + 100){
            for(int colmy=55; colmy<650; colmy= colmy + 100){           
  
  noStroke();
  fill(229,189,19);
  rect(beex,beey,100,60);
  triangle(beex+50,beey-25,beex,beey,beex+100,beey);
  triangle(beex+50,beey+85,beex,beey+60,beex+100,beey+60);

  noStroke();
  fill(247,207,40);
  rect(colmx,colmy,90,50);
  triangle(colmx+45,colmy-20,colmx,colmy,colmx+90,colmy);
  triangle(colmx+45,colmy+70,colmx,colmy+50,colmx+90,colmy+50);
  
  //cabeza
  fill(66,34,18);
  ellipse(mouseX,mouseY,30,30);
  fill(117,79,33);
  ellipse(mouseX,mouseY,20,20);
 
  //aguijon
   fill(66,34,18);
     ellipse(mouseX,mouseY+45,10,15);

//cuerpo
  fill(66,34,18);
  ellipse(mouseX,mouseY+20,40,50);
  fill(247,175,59);
  ellipse(mouseX,mouseY+20,30,40);
 
  //lìneas del cuerpo
    for(int lin=5; lin<35; lin=lin + 12){
  fill(66,34,18);
rect(mouseX-17,mouseY+lin,34,5);

//alitas
fill(255,255,255,50);
  ellipse(mouseX-20,mouseY+15,30,15);
fill(255,255,255,50);
  ellipse(mouseX+20,mouseY+15,30,15);
  
  //antenitas
  fill(66,34,18);
  rect(mouseX-7,mouseY-25,3,15);
    rect(mouseX+3,mouseY-25,3,15); 
   ellipse(mouseX-6,mouseY-25,5,5);
   ellipse(mouseX+4,mouseY-25,5,5);
   
 }

}
}
}
}
}
