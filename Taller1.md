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
---
---
## Ejercicio 2

Kelson Sporting fabrica dos modelos de guantes de beisbol: uno normal y uno manopla de catcher. La empresa tiene disponibles 900 horas de tiempo de producción en su departamento de corte y costura, 300 horas disponibles en su departamento de terminado y 100 horas disponibles en su departamento de empaque y embarque. Los requerimientos de tiempo y de producción y la contribución a la utilidad de cada uno de los productos es:

| MODELO           | TIEMPO DE PRODUCCIÓN (HORAS) ||| UTILIDAD/GUANTE |
|------------------|-----------------------------|---|---|-------------|
|                  | Corte y Costura             | Terminado | Empaque y Embarque |             |
|------------------|-----------------------------|-----------|--------------------|-------------|
| Guante Normal    | 1                           | 1/2       | 1/8                | $5          |
| Manopla Catcher  | 3/2                         | 1/3       | 1/4                | $8          |


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
