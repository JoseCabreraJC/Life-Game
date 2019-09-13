# El juego de la vida (Leng: Smalltalk)
El juego de la vida es un autómata celular, es decir una rejilla en dos dimensiones cuyas celdas
están ocupadas por lo que se denominan autómatas finitos, se trata de un objeto que se encuentra
en uno de entre un conjunto de estados posibles finito. Su actualización, es decir el cálculo de cuál
será su estado en el tiempo siguiente (t+1) utiliza un conjunto de reglas que se conocen como reglas
de transición, que serán las que actualizarán el estado de cada autómata finito teniendo en cuenta
tanto su estado actual como los estados de los autómatas vecinos que se encuentran a su alrededor.
En este caso, cada autómata finito tiene 8 vecinos, los situados a su alrededor. Además se asume
que los autómatas tienen solo dos estados posibles, el estado 0 (muerto) o 1 (vivo). El juego actualiza
el estado de los autómatas finitos aplicando la siguientes reglas:

- Regla 1: sea el estado de un autómata finito 𝑎𝑖𝑗igual a 0 o 1. Su estado futuro será idéntico al anterior
si el número de vecinos en estado 1 es igual a 2.
- Regla 2: el estado de un autómata finito 𝑎𝑖𝑗pasará al estado 1 en el tiempo 𝑡 + 1 si el número de
vecinos en estado 1 es igual a 3. Este cambio sólo tendrá lugar si su estado era 0 en el tiempo 𝑡.
- Regla 3: sea el estado de un autómata finito 𝑎𝑖𝑗morirá (pasará al estado 0) en el tiempo 𝑡 + 1 si el
número de vecinos en estado 1 es inferior a 2 o superior a 3. Este cambio sólo tendrá lugar si su
estado era 1 en el tiempo 𝑡.
Aplicar reiteradas veces las reglas de transición a cada uno de los autómatas finitos que componen
el autómata celular permitiendo parametrizar las dimensiones de la grilla donde se ubicarán los
autómatas finitos y la cantidad de generaciones de evolución.

Proponga una variación al modelo enunciado.

## Variaciones propuestas por el alumno 
Se podrian agregar condiciones adicionales para que muera, o viva.
Estados adicionales: quizas atributos extras a cada celula, como canibalismo, altruismo, clanes, comida?
