_Constructors_ (de Clases): Los constructores son funciones dedicadas a la fabricación de objetos de acuerdo con una plantilla predeterminada.
    Cada uno de los objetos creados por un constructor compartirá propiedades (no necesariamente valores). 
    Una forma de crear un *constructor* es...
        function Usuario (user, name, password){        
            // Por convención, el nombre de las funciones constructoras empieza con mayúscula
            this.user = user || 'bunnymalo';
            this.name = name || ´Benito';
            this.password = password || 'LaSanta123';    
            // Los valores que siguen al operador OR (||) son valores predeterminados
        }
    Luego, para crear un nuevo objeto es necesario declararlo como variable y asignarle valores mediante la instrucción *new*...
        var romeo = new Usuario('aventurero', 'Romeo', 'Indi$entPropo$41');
    El objeto resultante es el siguiente...
        romeo // Usuario {user:'aventurero, name: 'Romeo', password: 'Indi$entPropo$41'}

'prototype': JavaScript también permite crear métodos y adjuntarlos a los objetos que crea la Clase o función constructora. A estos métodos
    se les llama prototipos y son creados mediante la instrucción *prototype* así...
        Usuario.prototype.meGusta = function(){
            return ('Me gusta la música de ' + this.user)
        }
    Para usar el prototipo basta con llamarlo como una propiedad del objeto...
        romeo.meGusta; // 'Me gusta la música de aventurero'