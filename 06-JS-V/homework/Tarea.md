Explicación de conceptos

* `prototype`
    El prototype es la forma que tienen las clases para crear un método una única vez y que cada objeto de esta clase puede acceder a dicho método. Esto se hace con el fin de ahorrar espacio en la memoria y da mayor facilidad para que los objetos accedan a los métodos que se desee.

        Ejemplo:

        function Pelicula(nombre,cine,hora){
            this.nombre = nombre;
            this.cine = cine;
            this.hora = hora;
        }

        Pelicula.prototype.disponibilidad= function(){
            return 'Hay 20 entradas para la película ' + this.nombre + ' en el cine ' + this.cine + ' a las ' + this.hora;
        }

        var rapunzel = new Pelicula('Rapunzel','Cine Colombia','6:00 pm');

        console.log(rapunzel.disponibilidad());

* _Constructors_ (de Clases)
    Los constructores son clases que sirven para crear objetos con diferentes propiedades, un constructor puede heredar propiedades de otro constructor, por ejemplo, se tiene un constructor llamado animal con las propiedades nombre y edad, y otro constructor llamado perro puede heredar las propiedades de animal y tener sus propias propiedades.

        Ejemplo:

        function Animal(nombre,edad){
            this.nombre = nombre;
            this.edad = edad;
        }

        Animal.prototype.presentacion = function(){
            console.log(this.nombre + ' es un animal y tiene ' + this.edad + ' años');
        }

        var Max = new Animal('Max',5);

        Max.presentacion();

        function Perro(nombre,edad,tipo_animal){
            Animal.call(this,nombre,edad);
            this.tipo_animal = tipo_animal;
        }

        Perro.prototype = Object.create(Animal.prototype);

        Perro.prototype.constructor = Animal;

        var Lucian = new Perro('Lucian',2);

        Lucian.presentacion();