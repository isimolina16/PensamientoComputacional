# Plantilla para solemne-02
https://editor.p5js.org/SoftBlue_Ali/sketches/5dHI209fc 

## Integrantes del grupo

- (Almendra Manzi) [Almendra-Manzi](https://github.com/Almendra-Manzi)
- (Isidora Molina) [isimolina16](https://github.com/isimolina16)

## Descripción del disco
lanzado el 15 de septiembre de 1986, Pateando piedras entrega un potente mensaje de la sociedad Chilena de la epoca, marcado la dictadura, la desigualdad y la frustración causada por la falta de oportunidades presente en las clases menos acomodadas, visto desde las vivencias de los miembros de la banda.

![Portada de álbum pateando piedras](./pateando-piedras.jpg)

- (Pateando Piedras)
- 1986
- Los prisioneros (Jorge Gonzales, Claudio Narea, Miguel Tapia)
- Tracklist

```txt
1. Muevan las industrias
2. ¿Por qué no se van?
3. Estar solo
4. El baile de los que sobran
5. Exijo ser un héroe
6. Quieren dinero
7. Por favor
8. ¿Por qué los ricos?
9. Una mujer que no llame la atención
10. Independencia cultural
```

- Aspecto del álbum a desarrollar (premisa)

> Este proyecto busca retratar la esencia del álbum que se caracteriza por ser el sujeto que encarnar la desigualdad de clases sociales, viviendo en una dicotomía donde unos pocos lo tienen todo, y la mayoría tiene poco, siendo parte de la clase más vulnerable. Queremos representar esta dualidad a través de la moneda de 10 pesos de 1973, mostrando  en la cara y en el sello de la moneda, mientras gira, un elemento que represente a cada clase social para demostrar las diferencias que existen entre ellas.


## Conclusión del proceso

- Distancia entre premisa y resultado

> El resultado obtenido es la moneda girando, mostrando  el sello original. Por otro lado, la cara cuenta con la figura original del angel pero en vez de tener sus brazos extendidos rompiendo las cadenas, esta siendo apresada por ellas, dado el contexto de dictadura.

- Cosas no conseguidas

> Faltaron agregar elementos más representativos del album y falta de complejidad al proyecto.

- Descubrimientos al trabajar

> Uso de else

## Explicación del código (3 aspectos)

### Bloque de código 1

```js
// let sello;
let cara;

function setup() {
  createCanvas(400, 400);
  
//cargo ambas imagenes 
  sello = loadImage("./sello.png")
  cara = loadImage("./cara.png")

```
Aquí se realiza la carga de las imagenes utilizadas para componer la moneda.

### Bloque de código 2

```js
// push();
  if (tam > 0){
    image (cara, width/2, height/2, tam, 200);
  } else {
    image (sello, width/2, height/2, abs(tam), 200);
  }
pop();
```
Aquí se utiliza if y else para generar el efecto de cambiar del lado de la moneda.

### Bloque de código 3

```js
//let t = frameCount * 0.05;
  
//declaro "tam" como la deformación del objeto con seno
  let tam = 20 + sin(t) * 200;
```
La primera parte establece la velocidad con la que se realizará la animación (t), la segunda parte contiene los valores que se utilizaran para deformar el objeto, suavizando el movimiento con "sin"

### Declaración sobre el uso de IA

- IA utilizada(s) y tipo de licencia (pago, gratuita)

> Chatgpt gratis

- Problema a resolver a través de la IA

> lograr el efecto de cambio de cara para lograr la ilusión de un objeto en 3d

- Prompts utilizados

> Prompt 1: "Estoy intentando crear un codigo en p5js para generar una animación con 3 o más variables, Hasta ahora me han enseñado comandos básicos de figuras (square, ellipse, rect, etc), frame rate, random, if, let, mouse x/y, sin y cos, no puedo activar WEBGL aun. Ya tengo una parte hecha, me puedes dar ideas de variables que puedo agregar a mi proyecto?"

> Prompt 2: "Quiero hacer un efecto de cara y sello con los comandos que se pero de momento solo se como animar una cara"

> Prompt 3: (Enviada una captura del código)
"Este es mi codigo, me ayudas a integrar el otro lado de la moneda? (Sello)"

- Secciones de código entregadas por la IA

```js
  if (tam > 0) {

    image(cara,
          width/2,
          height/2,
          tam,
          200);

  } else {

    image(sello,
          width/2,
          height/2,
          abs(tam),
          200);
  }
```
