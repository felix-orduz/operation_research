# Felix Ernesto Orduz Grimaldo - 614202008

## Ejercicio 1

Sunco transforma petróleo en queroseno y en aceite combustible. Cuesta 40 dólares comprar 1000 barriles de petróleo, que se destilan después y producen 500 barriles de queroseno y 500 barriles de aceite combustible. Se puede vender directamente lo que se obtiene de la destilación, o se puede pasarlo por un reactor catalítico. El queroseno obtenido después de la destilación y sin más procesos, se puede vender a 60 dólares los 1000 barriles. El aceite combustible obtenido después de la destilación y sin más procesos, se puede vender a 40 dólares los 100 barriles.

Tarda una hora procesar 1000 barriles de queroseno en el reactor catalítico, y se pueden vender estos 1000 barriles a 130 dólares. El proceso de 1000 barriles de aceite combustible en el reactor catalítico tarda 45 minutos, y se pueden vender estos 1000 barriles a 90 dólares. Se pueden comprar diariamente a lo más 20000 barriles de petróleo, y se disponen de 8 horas de desintegración catalítica. Formule y resuelva un modelo de programación lineal para maximizar las ganancias de sunco.

### Solución
**Variables De Decisión:**

- $x_1 =$  Cantidad de barriles de queroseno sin proceso catalitico (en miles)
- $x_2 =$  Cantidad de barriles de queroseno con proceso catalitico (en miles)
- $x_3 =$  Cantidad de barriles de aceite sin proceso catalitico (en miles)
- $x_4 =$  Cantidad de barriles de aciete con proceso catalitico (en miles)

**Función Objetivo**

$$\max Z = 60x_1 + 130x_2 + 400x_3 x_3 + 90x_4$$

**Restricciones:**
- $x_1 \geq 0$
- $x_2 \geq 0$
- $x_3 \geq 0$
- $x_4 \geq 0$
- $x_1 \geq x_2$
- $x_3 \geq x_4$
- $x_2 + \frac{3}{4}x_4 \leq 8$

## Ejercicio 2

Kelson Sporting fabrica dos modelos de guantes de beisbol: uno normal y uno manopla de catcher. La empresa tiene disponibles 900 horas de tiempo de producción en su departamento de corte y costura, 300 horas disponibles en su departamento de terminado y 100 horas disponibles en su departamento de empaque y embarque. Los requerimientos de tiempo y de producción y la contribución a la utilidad de cada uno de los productos es:

| MODELO | T. PRODUCCIÓN (HORAS)||| UTILIDAD/GUANTE |
|-|-|-|-|-|
| | Corte y Costura | Terminado | Empaque||
| Guante Normal    | 1  | 1/2  | 1/8 | $5  |
| Manopla Catcher  | 3/2  | 1/3 | 1/4  | $8 |


## Solución:

**Variables Decisión**
- $x_1 =$  Cantidad de guantes modelo normal
- $x_2 =$  Cantidad de guantes modelo catcher

**Función Objetivo**

$$\max Z = 5(x_1) + 8(x_2)$$

**Restricciones**

- $x_1 \geq 0$
- $x_2 \geq 0$
- $x_1 + 1.5x_2 \leq 900$
- $0.5x_1 +  \frac{1}{3} x_2 \leq 300$
- $0.125x_1 + 0.25 x_2 \leq 100$


## Ejercicio 3

Una compañía de fabricación de muebles ha de determinar cuántas mesas, sillas, pupitres y librerías debe hacer para optimizar el uso de sus recursos. Estos productos utilizan dos tipos diferentes de paneles, y la compañía dispone de 1500 tableros de un tipo y 1000 de otro tipo. Por otro lado cuenta con 800 horas de mano de obra. Las predicciones de venta así como los pedidos atrasados exigen la fabricación de al menos 40 mesas, 130 sillas, 30 pupitres y como máximo 10 librerías. Cada mesa, silla, pupitre y librería necesita 5, 1, 9, y 12 tableros, respectivamente, del primer tipo de panel y 2, 3, 4, y 1 tableros del segundo. Una mesa requiere 3 horas de trabajo; una silla, 2; un pupitre, 5; y una librería 10. La compañía obtiene un beneficio de 12 dólares en cada mesa, 5 dólares en cada silla, 15 dólares en un pupitre, y 10 dólares en una librería. Plantéese el modelo de programación lineal para maximizar los beneficios totales.


### Solución

**Variables de Decisión**

- $x_1 =$ Cantidad de mesas a fabricar
- $x_2 =$ cantidad de sillas a fabricar
- $x_3 =$ cantidad de pupitres a fabricar
- $x_4 =$ cantidad de librerias a fabricar

**Función Objetivo**

$$\max Z = 12x_1 + 5 x_2 + 15 x_3 +10x_4 $$

**Restricciones**

- $x_1 \geq 0$
- $x_2 \geq 0$
- $x_3 \geq 0$
- $x_4 \geq 0$

**Restricciones Pedidos atrasados**

- $x_1 \geq 40$
- $x_2 \geq 130$
- $x_3 \geq 30$
- $x_4 \leq 10$

**Restricciones Panel Tipo 1**
- $5x_1 + x_2 + 9x_3 + 12 x_4\leq 1500$

**Restricciones Panel Tipo 2**
- $2x_1 + 3x_2 + 4x_3 + x_4\leq 1000$

**Restricciones Horas**
- $3x_1 + 2x_2 + 5x_3 + 10x_4\leq 800$



## Ejercicio 4

Pedro Pérez fabrica cable eléctrico de alta calidad usando dos tipos de aleaciones metálicas, A y B. La aleación A contiene un 80% de cobre y un 20% de aluminio, mientras que la B incluye un 68% de cobre y un 32% de aluminio. La aleación A tiene un precio de 80 euros por tonelada, y la B, 60 euros por tonelada. ¿Cuáles son las cantidades que Pedro Pérez debe usar de cada aleación para producir una tonelada de cable que contenga al menos un 20% de aluminio y cuyo coste de producción sea el menor posible?

### Solución

**Variables de decisión**

- $x_1 =$ Cantidad de aleación tipo A
- $x_2 =$ Cantidad de aleación tipo B

**Función Objetivo**

$$ \min Z = 80x_1 + 60x_2$$

**Restricciones**

- $x_1 \geq 0$
- $x_2 \geq 0$
- $x_1 + $x_2 + 1
- $0.2x_1 +0.32 x_2 \geq 0,2$



## Ejercicio 5
Pepe construye dos tipos de transformadores eléctricos y tiene disponible 6 toneladas de material ferromagnético y 28 horas de tiempo de manufacturación. El transformador tipo 1 requiere 2 toneladas de material y 7 horas de trabajo, mientras que el transformador tipo 2 necesita 1 unidad de material y 8 horas de trabajo. Los precios de venta de los transformadores 1 y 2 son respectivamente 120 y 80 en miles de euros. ¿Cuántos transformadores de cada tipo ha de construir Pepe para maximizar sus beneficios?

### Solución

**Variables de Decisión**

- $x_1 =$ Cantidad de transformadores tipo 1
- $x_2 =$ Cantidad de transformadores tipo 2

**Función Objetivo**

$$\max Z = 120x_1 + 80x_2$$

**Restricciones**

- $x_1 \geq 0$
- $x_2 \geq 0$
- $2x_1 +x_2 \leq 6$
- $7x_1 +8x_2 \leq 28$
