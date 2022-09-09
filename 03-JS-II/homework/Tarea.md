Explicación de conceptos

* `for`
    Un for es un ciclo o bucle que se encarga de repetir el bloque de código que este tenga hasta que la condición del ciclo sea falsa, usualmente se usa la variable 'i' para esto, primero se crea la variable y se iguala a 0 o lo que se quiera, luego se coloca el condicional, que puede ser hasta que i sea mayor a cierto número, y por último, se escribe a que cantidad va aumentar el ciclo, que puede ser de uno en uno o más; todo esto se separa con un punto y coma.
        Ejemplo:
        for(var i=0; i<=5; i++){
            console.log('Ejercicio ' + i);
        }

* `&&`
    Es un operador lógico que significa 'y', es usado para determinar que algo se cumpla cuando dos o más cosas sean verdaderas, es decir, para que algo se cumpla todas las condiciones deben ser verdaderas.
        Ejemplo:
        var num = 16;
        if(num < 20 && num > 10){
            console.log('El número está entre 10 y 20');
        }

* `||`
    Es un operador lógico que significa 'o', determina que algo se cumpla cuando cualquiera de las condiciones se cumpla, con solo una condición verdadera el código se ejecutará.
        Ejemplo:
        var num2 = 23;
        if(num2 > 20 || num2 < 10){
            console.log('El número es mayor a 20 o menor a 10');
        }

* `!`
    Es un operador lógico que significa 'No' o 'Diferente', es decir, el código se ejecutará si algo es diferente a lo que se compare o si la condición es verdadera al usar el 'No', por ejemplo, cuando algo es false y se usa el '!', se convertiria en un true, por lo tanto, la condición se cumple.
        Ejemplo:
        var num3 = 10;
        var num4 = 20;
        if(num3 !== num4){
            console.log('Los números son diferentes');
        }
        if(!(num3 === num4)){
            console.log('Los números no son iguales');
        }