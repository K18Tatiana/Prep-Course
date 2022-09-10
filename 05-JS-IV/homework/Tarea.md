Explicación de conceptos

* Objetos
    Los objetos son contenedores de información de una sola cosa, básicamente guarda características de un valor, para esto, se usa una palabra clave que guarda el valor; las palabras claves deben ser diferentes, sin embargo, el contenido puede repetirse.
        Ejemplo:
        const persona = {
            nombre : 'Tatiana',
            apellido : 'Vega',
            edad : 18
        };

* Propiedades
    Una propiedad de un objeto es una información o característica que tenga el objeto, es lo que se agrega o elimina a un objeto. Por ejemplo, las propiedad del objeto 'persona' del ejemplo anterior, serían nombre, apellido y edad.

* Métodos
    Los métodos son funciones guardadas en un objeto, estas se crean como si fueran una preopiedad del objeto pero son funciones que permiten recibir argumentos y retornar un resultado.
        Ejemplo:
        const perro = {
            nombre : 'Max',
            edad : 3,
            ladrar : function(){
                console.log('Guauuu');
            }
        }; 
        perro.ladrar();

* Bucle `for…in`
    Un bluce for... in es un un 'for... in loop', el cual se utiliza para recorrer todas las claves o propiedades de un objeto. Este for... in es similar a un for normal, sin embargo, la sintaxis es un poco distinta, primero se declara la variable, seguido se usa una palabra clave 'in' y por último el nombre del objeto.
        Ejemplo:
        for(var clave in persona){
            console.log(clave + ':');
            console.log(persona[clave]);
        }

* Notación de puntos vs notación de corchetes
    Hay dos formas para llamar las propiedades de un objeto, a partir de un punto o corchetes. Con puntos solo se nombra el objeto y seguido de un punto va la propiedad, en el caso de corchetes se escribe el nombre del objeto y entre corchetes se escribe el nombre de la propiedad entre comillas.
        Ejemplo:
        - Con puntos:
        persona.nombre; // Tatiana
        persona.edad;   // 18
        - Con corchetes:
        persona['nombre']; //Tatiana
        persona['edad'];   // 18