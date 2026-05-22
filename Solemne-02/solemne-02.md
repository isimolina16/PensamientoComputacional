# Plantilla para solemne-02
https://editor.p5js.org/SoftBlue_Ali/sketches/5dHI209fc 

## Integrantes del grupo

- (Almendra Manzi) [cuentaGithub](https://github.com/cuentaGithub)
- (Isidora Molina) [](https://github.com/cuentaGithub)

## Descripción del disco

![Portada de álbum xxxx yyyy](./img/cover.jpg)

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


### Declaración sobre el uso de IA

- IA utilizada(s) y tipo de licencia (pago, gratuita)

> Chatgpt gratis, Claude pagado, etc

- Problema a resolver a través de la IA

> Generación de grillas, animación de imagen, etc

- Prompts utilizados

> Prompt 1

> Prompt 2

> Prompt 3

- Secciones de código entregadas por la IA

```js
//código entregado por IA acá
```