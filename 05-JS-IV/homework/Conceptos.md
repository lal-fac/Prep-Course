Objetos: El objeto es la estructura básica dentro de JavaScript. Todos los tipos de dato, funciones y estructuras están construidos a partir de
    la configuración de un objeto. Los objetos consisten en un conjunto de propiedades y sus respectivos valores (*key:value*). Los arreglos,
    por ejemplo, son tipos de objetos especializados que tienen como "propiedades" (o *keys*, o argumentos), números del 0 al (*length - 1*).
    En los objetos literales, las propiedades pueden ser cualquier cadena de texto. 
    Por otra parte, así como en los arreglos, los valores de los objetos pueden ser cualquier tipo de dato, variable o función que pueda 
    procesar JavaScript. 
    
    Para crear un objeto, basta con definirlo así...
        var objeto = {
            key1 : 'value 1',
            key2 : true,
            key3 : 23,
            key4 : function(){
                return true;
            }
        }

    Existen dos formas de llamar una propiedad para verla, modificarla, usarla, etc... La primera es la 'notación de punto' que consiste en 
    escribir el nombre de objeto, seguido de la propiedad por acceder. (Ej: objeto.key1 // 'value 1'). La segunda forma es similar a la usada 
    en los arreglos, consiste en escribir el nombre de un objeto seguido por el nombre de la propiedad encerrado en corchetes (Ej: objeto
    ['key3'] // 23).

    Método: Cuando el valor de un objeto es una función, a ésta se le llama "método". Habrá ocasiones en las que será necesario repetir un
    mismo método (acción específica, función) dentro de distintos objetos. En estos casos, conviene acceder a las propiedades del objeto 
    mediante la *keyword this* que hace referencia al objeto en el que está siendo llamado el método y no a un objeto con un nombre específico. 

    Bucles *for ... in*: Así como los arreglos permiten iterar a través de cada uno de los elementos mediante el índice numérico, los objetos 
    permiten hacer esa misma iteración mediante el bucle *for ... in*. Éste comando declara una variable de iteración que será ocupada por  
    cualquiera de los argumentos que contenga el objeto. 
    El bucle está descrito así...
        for (var keys in objeto){
            console.log(objeto.key);
        }