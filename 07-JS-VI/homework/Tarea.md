Explicación de conceptos

* Funciones Callback
    Las funciones callback son las funciones que se pueden pasar como argumento a otra función, por ejemplo, se crea una función con un argumento y retorna algo, y además, se crea otra funcion que recibe un argumento del usuario y el otro argumento es la función anterior, de esta forma, esta función retorna lo mismo que la función que recibe como argumento.

        Ejemplo:

        function Suma(num1,num2){
            return num1 + num2;
        }

        function Resta(num1,num2){
            return num1 - num2;
        }

        function Multiplicacion(num1,num2){
            return num1 * num2;
        }

        function Division(num1,num2){
            return num1/num2;
        }

        function Operacion(num1,num2,cb){
            return cb(num1,num2);
        }

        console.log(Operacion(10,4,Suma));
        console.log(Operacion(10,4,Resta));
        console.log(Operacion(10,4,Multiplicacion));
        console.log(Operacion(10,4,Division));