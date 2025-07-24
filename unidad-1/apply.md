# Unidad 1

## 🛠 Fase: Apply

###  SELECT:
link: http://www.generative-gestaltung.de/2/sketches/?02_M/M_6_1_02
### DESCRIBE:
El diseno es el de de dos bolas negras que estan unidas por un hilo azul, estas bolas aparecen en un lugar aleatorio del lienzo por defecto, cuando uno presiona cualquier parte del lienzo hace  que una de las bolas en este caso la que mas cerca este de donde el mouse presiono la pantalla se trasnporte a dicho punto lo que hace que el hilo azul que las une se alargue y que la bola que se habia quedado en el posicion anterior se deslice atraves del hilo y quede a la misma distancia de que tenian entre ellas apenas se inicio el diseno, a su vez si decides mantener el curso y irte moviendo alrededor del lienzo ahi si las bolas seguiran el movimiento que haga el cursor.

### ANALYZE:
El programa debe tener unas variables tanto en x como en y para que lea la posicion del puntero en el lienzo, debe tambien de tener algun random en la posicion de las bolas al momento de iniciar el programa muy seguramente y debe tener algo que lea tambien cuando se esta presionando en el puntero en el lienzo.

### CONVERT:
link: https://editor.p5js.org/LuisFernandoParra/sketches/XZO7Wh71r
#### CODIGO:
``` JS
let x1, x2, y1, y2;

function setup() {
  createCanvas(400, 400);
  x1 = random(150,250)
  y1 = random(150,250)
  x2 = x1 - 80
  y2 = y1 - 80


  


}

function draw() {
 
  background(220);
  stroke(0,0,255);
  strokeWeight(3)
  line(x1, y1, x2, y2);
  strokeWeight(0)
  fill(0,0,0);
  circle(x1,y1,25);
  fill(0,0,0);
  circle(x2,y2,25);
  translate()
  
  if (mouseIsPressed){
    x1 = mouseX
    y1 = mouseY
  }
  
  x2 += ((x1 - x2)-80) * 0.1;
  y2 += ((y1 - y2)-80)* 0.1;
  
}


```
### EXPLORE:
link: https://editor.p5js.org/LuisFernandoParra/sketches/YaBX2hQpt

<img width="296" height="300" alt="image" src="https://github.com/user-attachments/assets/53bd48f5-4fd2-4f86-b3d7-a9bcd5a1a6fa" />

#### CODIGO:

```JS
let x1, x2, y1, y2;

function setup() {
  createCanvas(400, 400);
  x1 = random(150,250)
  y1 = random(150,250)
  x2 = x1 - 160
  y2 = y1 - 160


  


}

function draw() {
 
  background(220);
  stroke(180,30,160);
  strokeWeight(8)
  line(x1, y1, x2, y2);
  strokeWeight(0)
  fill(0,0,0);
  square(x1,y1,25);
  fill(0,0,0);
  circle(x2,y2,80);
  translate()
  
  if (mouseIsPressed){
    x1 = mouseY
    y1 = mouseX
  }
  
  x2 += ((x1 - x2)-160) * 0.4;
  y2 += ((y1 - y2)-160)* 0.4;
  
}




```

#### EXPLICACION:
lo que hice fue cambiar el color del stroke, aparte de eso cambie uno de los circles por square para volver  uno de los circulos en cuadrados, tambien quise cambiar el grosor de la linea asi que cambie el stroke weight de 3 a 8, tambien aumente el tamano de del circulo, tambien inverti los valores de x1 y y1 y ahora se movia de forma muy extrana y por ultimo alargue la linea que unia ambos alterando



### TINKER:
link: https://editor.p5js.org/LuisFernandoParra/sketches/qumFjkYrY


<img width="299" height="295" alt="image" src="https://github.com/user-attachments/assets/352d330d-83cc-437a-848b-de88637dc734" />

#### CODIGO:
``` JS
let x1, x2, y1, y2;

function setup() {
  createCanvas(400, 400);
  x1 = random(150,250)
  y1 = random(150,250)
  x2 = x1 - 80
  y2 = y1 - 80


  


}

function draw() {
 
  background(220);
  stroke(0,0,255);
  strokeWeight(3)
  line(x1, y1, x2, y2);
  strokeWeight(0)
  fill(0,0,0);
  circle(x1,y1,25);
  fill(0,0,0);
  circle(x2,y2,25);
  translate()
  
  if (mouseIsPressed){
    x1 = mouseX
    y1 = mouseY
  }
  
  x2 += ((x1 - x2)-80) * 10;
  y2 += ((y1 - y2)-80)* 10;
  
}


```

