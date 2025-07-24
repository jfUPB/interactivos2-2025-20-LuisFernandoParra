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
link: https://editor.p5js.org/LuisFernandoParra/sketches/XZO7Wh71r


<img width="302" height="297" alt="image" src="https://github.com/user-attachments/assets/f147b6d1-9e33-414a-8df3-00a1308d031f" />

#### CODIGO:
```JS
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
  stroke(180,30,160);
  strokeWeight(8)
  line(x1, y1, x2, y2);
  strokeWeight(0)
  fill(0,0,0);
  square(x1,y1,25);
  fill(0,0,0);
  circle(x2,y2,25);
  translate()
  
  if (mouseIsPressed){
    x1 = mouseY
    y1 = mouseX
  }
  
  x2 += ((x1 - x2)-30) * 0.4;
  y2 += ((y1 - y2)-30)* 0.4;
  
}


```

#### EXPLICACION:
lo que hice fue cambiar el color del stroke, aparte de eso cambie uno de los circles por square para volver  uno de lo




