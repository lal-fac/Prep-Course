Conceptos JS-II
for. 'for' es una instrucción para que la computadora lleve a cabo una serie de instrucciones un número indicado de veces. Dentro de la sintáxis
    de un bucle for, es posible (¿necesario?) determinar la variable que cambiará cada vez que termine un ciclo (contador), las condiciones
    necesarias para que se detenga el ciclo (número de iteraciones) y la magnitud de cada incremento que seguirá el contador cuando complete una
    iteración. Una vez que el contador deje de cumplir con la condicióne establecida en el segundo parámetro del bucle, éste se detendrá.
Operadores lógicos. Cuando establecemos las condiciones necesarias para el funcionamiento de un programa, como en un statement if, a veces es 
    necesario incluir más de una condición. En esos casos, el programa necesita operadores lógicos que le digan cuáles condiciones obedecer y 
    cuáles igorar. Los operadores lógicos son AND, OR y NOT.
&&. El operador AND indica al programa que, para seguir adelante con las instrucciones, debe cumplir con todas las condiciones establecidas. Es
    decir, si es necesario cumplir con las condiciones *p* Y *q*, y *p* es *true*, pero *q* es *false*, el programa no ejecutará las
    instrucciones. Si ambas son true, el programa seguirá adelante. 
||. De forma similar, el operador OR indica al programa que puede seguir adelante con tan sólo una de las condiciones dadas. Si es necesario
    que *p* o *q* sean *true*, el programa evaluará *p* primero, si es *true* el programa seguirá adelante con las instrucciones, si es *false*
    evaluará *q*; si *q* es *true*, el programa continuará, si no, interrumpirá su funcionamiento. En una condición que ocupa el operador ||
    JavaScript evaluará de izquierda a derecha. Si alguna de las condiciones resulta *true*, no evaluará las que siguen. 
!. El operador NOT indica al programa la existencia de una condición que NO debe ser cumplida.