* Variables
    Las variables son asignaciones que se da a algún valor que se almacena en un código para poder usarlas en cualquier momento; en otras palabras, una variable es un valor almacenado en el código que puede ser usado en cualquier parte de este. Estas variables pueden ser tipo number (número), string (cadena de texto) o boolean (verdadero o falso).
        Ejemplo:
        var numero = 23;
        var miperro = "Max";
        var condicion = true;

* Strings
    Un string es una variable de tipo texto o cadena, se puede guardar con comillas simples o dobles.
        Ejemplo:
        var nombre = "Tatiana";
        var apellido = 'Vega';

* Funciones (argumentos, `return`)
    Una función es un bloque de código que se encarga de realizar alguna operación u objetivo en específico, para esto, dependiendo de la operación deseada es necesario que una función reciba ciertos argumentos para realizar dicha operación y que posteriormente retorne su resultado. Por ejemplo, para realizar una multiplicación a partir de una función, es necesario mandar dos argumentos a la función, los cuales serían dos números que la función se encargará de multiplicar y retornar su resultado.
        Ejemplo:
        function MultiplicarDosNumeros(numero1,numero2){
            var multiplicacion = numero1 * numero2;
            return multiplicacion
        }

        var multiplicacionn = MultiplicarDosNumeros(4,6);
        console.log(multiplicacionn); //24

* Declaraciones `if`
    Una declaración 'if' es una condición que se establece para que lo que está dentro del if pase únicamente si dicha condición se cumple.
        Ejemplo:
        var numero = 20;
        if (numero < 25){
            console.log('El número es menor a 25');
        }
* Valores booleanos (`true`, `false`)
    Un valor booleano es aquel que solo puede ser true (verdadero) o false (falso), este puede ser declarado con las palabras, o al realizar una asignación de una comparación se le asignará un true o false dependiendo de esta.
        Ejemplo:
        var condicion = false;
        var condicion2 = 15 > 7; //true

        console.log(condicion);
        console.log(condicion2);