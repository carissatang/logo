float theta_i = 0+ PI/12;
float theta_j = PI/9+ PI/12;
float theta_k = 2*PI/9+ PI/12;
int a = 1, b = 1;
int c = 127, d = 1;

void setup(){
  size(500, 500);
}

void draw (){
 // fill(15, 26, 41, 10);
  fill(223, 223, 221);
  rect(0, 0, width, height);

  smooth();
  stroke(15, 26, 41);
  strokeWeight(3);
  fill(15, 26, 41);
  ellipse(238, 97, 1, 1);
  ellipse(245, 97, 1, 1);
  ellipse(254, 98, 1, 1);
  ellipse(263, 100, 1, 1);
  ellipse(272, 104, 1, 1);
  ellipse(281, 106, 1, 1);
  ellipse(288, 112, 1, 1);
  ellipse(296, 118, 1, 1);
  ellipse(302, 125, 1, 1);
  ellipse(307, 133, 1, 1);
  ellipse(311, 141, 1, 1);
  ellipse(314, 151, 1, 1);
  ellipse(316, 160, 1, 1);
  ellipse(316, 169, 1, 1);
  ellipse(316, 178, 1, 1);
  ellipse(315, 189, 1, 1);
  noFill();
  arc(246, 168, 150, 140, 0.42, 4.54);
  arc(275, 145, 129, 130, 0.90, 3.96);
  
 // fill(255);
//  noStroke();
 // ellipse(random(width), random(height), 2, 2);
  
  fill(171, 135, 66);
  stroke(171, 135, 66);
  strokeWeight(2);
  beginShape();
  vertex(270, 169);
  vertex(272, 175);
  vertex(277, 180);
  vertex(272, 181);
  vertex(266, 187);
  vertex(265, 181);
  vertex(259, 176);
  vertex(267, 174);
  endShape(CLOSE);
  
  beginShape();
  vertex(267, 129);
  vertex(270, 130);
  vertex(274, 130);
  vertex(273, 134);
  vertex(274, 138);
  vertex(265, 136);
  vertex(267, 133);
  vertex(266, 129);
  endShape(CLOSE);
  
  beginShape();
  vertex(241, 151);
  vertex(245, 151);
  vertex(245, 156);
  vertex(241, 154);
  endShape(CLOSE);

  //println(mouseX, " ", mouseY);
  
  translate(246, 170);
  strokeWeight(3); 
  if (a == 0 || a == 255){b = -b;}
    a += b;
    stroke(15, 26, 41, a);
    for (float i = 0; i < TWO_PI; i += PI/3){
      pushMatrix(); 
      rotate(theta_i + i);
      line(58, 58, 90, 90);
      popMatrix();
    }
  strokeWeight(2);
  if (c == 0 || c == 255){
    d = -d;
    }
  else {
    c += d;
    stroke(15, 26, 41, c);
    }
    for (float j = 0; j < TWO_PI; j += PI/3){
        pushMatrix(); 
        rotate(theta_j + j);
        line(58, 58, 68, 68);
        line(75, 75, 80, 80);
        popMatrix();
     }
  for (float k = 0; k < TWO_PI; k += PI/3){
      pushMatrix(); 
      rotate(theta_k + k);
      line(58, 58, 80, 80);
      popMatrix();
   }
  
}
