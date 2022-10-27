![image](https://camo.githubusercontent.com/35e9d7d200795e6ec6bbf764d7f700d8da81cb5bc28ef9787d104a22eb3293a6/68747470733a2f2f696d67732e7365617263682e62726176652e636f6d2f37315a705a5949444b4a46463468797a765a5f4b6133636f2d625875356d5330756f496a637635757679342f72733a6669743a313230303a3638373a312f673a63652f6148523063446f764c336433647935312f593239734c6d31344c324e76626e526c2f626e51765932317a4c7a6b76615731682f5a3255765657526c51305644556c4d342f4d4734756347356e)
# Universidad de Colima
### Facultad de Ingenieria Mecanica y Electrica
### Ingenieria en Computacion Inteligente
##### Estudiante: Diana Laura Llamas Alcaraz
##### Profesor: Dr. Walter Alexander Mata Lopez
---
## Introducción:

Este es el portafolio de la segunda parcial en la materia de programacion funcional de la carrera de ICI. 
Donde estaran adjuntos los diferentes codigos de las clases en las que trabajamos con el lenguaje de Dart.

---
# Segunda Parcial

## Lenguaje Dart...

### _Introducción al lenguaje:_

##
  ### Impresión de un "Hola mundo"
         void main() {
          print("hola mundo");
         }
##
  ### Declaracion de Variables 

 Maneja un tipado  explicito 
 
 - #### Tipo Entero
 
 Sirve para datos de tipo entero sin decimales  
 
        void main() {
         int miEntero = 10;
         print(miEntero);
        }
 
 - #### Tipo Flotante 
 
 Sirve para datos con decimales 
 
        void main() {
         double miDouble = 3.1416;
         print(miDouble);
        }
 
 - #### Tipo Numerico
 
 Este sirve para cuando no se sabe que tipo de dato es el que se va a emplear: int y double;
 tambien conocida como una super clase, por el hecho de que facilita al programador la
 captura de un dato ya sea entero o decimal.
 
         void main() {
          num miNumero1 = 10;
          num miNumero2 = 3.1416;

          print(miNumero1);
          print(miNumero2);
         } 

- #### Tipo String

         void main() {
          String miString = "hola";
          print(miString);
         } 
  
- #### Tipo Dynamic
 Es conocido como tipo de dato dinamico; Este se utiliza cunado no sabes que tipo de dato es el que vas utilizar,
 puede contener datos del tipo entero, decimal y texto.

     void main() {
      dynamic miDinamico = "hola";
      print(miDinamico);
      dynamic miDinamico1 = 3.1416;
      print(miDinamico1);
     }
     
 - #### Tipo final 
 se utliza para que eldato no se pueda cambiar ("tiempo de ejecucion".
       
      void main() { 
      final double miPI = 3.1416;  
      print(miPI);
      }
      
      
### Programas de clase:

    void main(){
        num a =4;
        a as int; //casting sobre datos numericos
        print(a.isEven); // saber si es impar

        var infInt = 5;
        var infDouble = 9.81;
        print("${infInt.runtimeType}"); //saber el tipo de dato que es
        print("${infDouble.runtimeType}");

        num infNum;
        infNum = 3.6;
        print("${infNum.runtimeType}");
        infNum = 5;
        print("${infNum.runtimeType}");

        print(5.isEven); // saber si es impar
        print(5.isOdd); // saber si es par
    }

##

##

    void main(List<String> args){
        int a = -3000;
        doble b = 9.89;

        print(a.isNegative); // saber si es negativo

        print(b.floor()); // pone el numero menor
        print(b.ceil()); // pone el numero mayor

        print(b.round()); // redondear

        print(b.truncate()); // quitar decimales

        var c = "Hola";

        print(!b.isNaN); //saber si es un numero
    }


##
    void main(){
      num a = 3;
      a as int;// casting sobre datos numericos
      print(a.isEven);
      var infInt = 5;
      var infDouble = 9.81;

      print("${infInt.runtimeType}");
      print("${infDouble.runtimeType}");

      num infNum;
      infNum = 3.6;
      print("${infNum.runtimeType}");
      infNum = 5;
      print("${infInt.runtimeType}");
      print(5.isEven);
     }

##

    void main() {
      int a = -3000;
      double b = 9.4;

      print(a.isNegative); // indicar si es negativo

      print(b.floor()); //piso numero menor
      print(b.ceil()); //cielo te pone el numero mayor

      print(b.round()); //redondear

      print(b.truncate()); //quitar decimales

      print(!b.isNaN); //isNaN para saber si es un número
    }

##

    import 'dart:math';

    main(){ //division
      print((10 / 3).truncate());
      print(10 ~/ 3);

     print(cos(45 * pi / 180));
     print(sin(45 * pi / 180));
     print(sqrt(9));
     print(pow(2, 3));
     print(max(6, 10));
     print(min(6, 10));
    }
##
- ## Incrementos

      void main(List<String> args) {//Incfrementos
        var contador = 10;
        contador = contador + 1;
        print(contador);
        contador += 1;
        print(contador);
        contador++;
        print(contador);
        ++contador;
        print(contador);

        var c = 10;
        print(++c);
        c = 10;
        print(c++);
        print(c);
      }
##
- ## Decrementos.

      void main(List<String> args) {//Decrementos
        var contador = 10;
        contador = contador - 1;
        print(contador);
        contador -= 1;
        print(contador);
        contador--;
        print(contador);
        --contador;
        print(contador);

        var c = 10;
        print(--c);
        c = 10;
        print(c--);
        print(c);
      }
##
       void main(List<String> args) {
         int a = 5;
         double b = 3.5;
         print(a.toDouble());
         print(b.toInt());
         print("El valor es: $a ");
         print("El valor es: "+ a.toString());
         print( a + b );
         print( a / b );

       }
##
       void main(List<String> args) {
          var a = "10";
          var b = "8.5";

          print(int.parse(a) * 2);
          print(double.parse(b) * 2);

          var num = 3.141615925687;
          print(num.toStringAsFixed(3));
        }

##
- ## Hacer Comentarios en Dart.

    - //una sola linea
    

    - /* comentarios 
      en bloque*/

##
- ## Uso de clases.

       void main() {
          User usuario = User();
          print(usuario);
          usuario.nombre = "Diana";
          usuario.edad = 18;
          print(usuario.nombre);
          print(usuario.edad);
          User usuario2 = User();
          print(usuario2);
          usuario2.nombre = "Leo";
          usuario2.edad = 25;
          print(usuario2.nombre);
          print(usuario2.edad);
       }

      // clase que representa un usuario
       class User {
      // propiedad mombre de tipo string
        String? nombre;
        int? edad;
      }
##
        void main() {
          User usuario = User();
          print(usuario);
          usuario.nombre = "Diana";
          usuario.edad = 18;
          usuario.reporteUser();

          User usuario2 = User();
          print(usuario2);
          usuario2.nombre = "Leo";
          usuario2.edad = 25;
          usuario2.reporteUser();
        }

        // clase que representa un usuario
        class User {
          // propiedad mombre de tipo string
          String? _nombre = "Diana";
          //Propiedad edad de tipo int mayor de 0(cero)
          int? _edad = 21;
          //metodo que imprimeun usuario
          void reporteUser() {
            print(_nombre);
            print(_edad);
          }

          void set nombre(String nombre) {
            _nombre = nombre;
          }

          String get nombre {
            return _nombre!;
          }
        }
##
  ## Objetos: Clases y atributos.
  
  ### Ejemplos:

         class User{
            String? nombre;
            int? edad;
        }
        void main(List<String>args){
            User usuario1= User();
            print(usuario1);
            print(usuario1.nombre);
            print(usuario1.edad);
        } 
##
        class User {
          String nombre = "Alex";
          int edad = 50;
        }

        void main(List<String> args) {
          User usuario1 = User();
          print(usuario1.nombre);
          print(usuario1.edad);
        }
##      
        class User {
          String? nombre;
          int? edad;
        }

        void main(List<String> args) {
          User usuario1 = User();
          var usuario2 = User();

          usuario1.nombre = "Diana";
          usuario1.edad = 30;
          usuario2.nombre = "Hector";
          usuario2.edad = 22;

          print(usuario1.nombre);
          print(usuario1.edad);
          print(usuario2.nombre);
          print(usuario2.edad);
        }


##
  
  ## Objetos: clases, atributos y métodos.

         class User {
          String? nombre;
          int? edad;
          void reporte() {
            print("Nombre: $nombre");
            print("Edad: $edad años");
          }
         }

         void main(List<String> args) {
          User usuario1 = User();
          usuario1.nombre = "Diana";
          usuario1.edad = 13;

          usuario1.reporte();
         }


##

  ## Métodos Constructores: Getter y Setter

##
    - Setter: Son métodos que establecen/inicializan los atributos de la clase.
    - Getter: Son métodos que retoman los valores de los atributos de la clase. 
##

  ### Ejemplos:
            class User {
                String? _nombre;
                int? _edad;
                void set nombre(String nombre) {
                _nombre = nombre;
              }

              String get nombre {
                return _nombre!;
              }

              void reporte() {
                print("Nombre: $_nombre");
                print("Edad  : $_edad años")
              }
            }
              void main(List<String> args) {
                final usuario1 = User();
                usuario1.nombre = "Diana";
                print(usuario1.nombre);
                usuario1.reporte();
              }
##
              class User {
                String? _nombre;
                int? _edad;

                void set nombre(String nombre) {
                  _nombre = nombre;
                }

                String get nombre {
                  return _nombre!;
                }
                void set edad(int edad){
                  _edad = edad;

                }
                int get edad{
                  return _edad!;
                }
                void reporte(){
                  print("Nombre: $_nombre");
                  print("Edad  : $edad años");
                }
            }
            void main(List<String> args) {
              final usuario1 = User();
              usuario1.nombre = "Alex";
              usuario1.edad =50;
              usuario1.reporte(); 
            }

   ###  Ejemplo: Usando métodos arrow.
    
            class User {
                String? _nombre;
                int? _edad;

                void set nombre(String nombre) => _nombre = nombre;
                void set edad(int edad) => _edad = edad;

                String get nombre => _nombre!;
                int get edad => _edad!;
                void reporte() {
                  print("Nombre: $_nombre");
                  print("Edad  : $_edad años");
                }
             }

              void main(List<String> args) {
                final usuario1 = User();
                usuario1.nombre = "Alex";
                usuario1.edad = 50;
                print(usuario1.nombre);
                print(usuario1.edad);
                usuario1.reporte();
            }    

##
  ## Constructores.


- #### Método de la clase que se encarga de inicializar los atributos
- #### Es el primer método que se llama al crear la instancia
- #### El método lleva el nombre de la clase

##
  ### Ejemplo:
    
            class User {
              User() { //Creacion del constructor User
                print("Constructor User");
              }
            }
            void main(List<String> args) {
              final usuario1 = User(); //Creacion de la instancia usuario 1 que invoca al constructor User
              print(usuario1);
            }
            
  ### Ejemplo: Equivalencia a los setters y getters
 
            class User {
              String? _nombre;
              int? _edad;
              User(String nombre, int edad) {
                this._nombre = nombre;
                this._edad = edad;
              }
              String? get nombre => _nombre;
              int? get edad => _edad;
            }

            void main(List<String> args) {
              final usuario1 = User("Alex", 50);
              print(usuario1.nombre);
              print(usuario1.edad);
            }
 ##
   ### Ejemplo: Version corta de constructores(short hand)
   
            class User {
              String _nombre;
              int _edad;

              User(this._nombre, this._edad);

              String get nombre => _nombre;
              int get edad => _edad;
            }

            void main(List<String> args) {
              final usuario1 = User("Alex", 50);
              print(usuario1.nombre);
              print(usuario1.edad);
            }
##
  ## Constructores con propiedades nombradas
  ### Ejemplo:
            class User {
                String? nombre; //Creacion de las propiedades
                int? edad;

                User({this.nombre, this.edad}); //Creacion del contructor

                String? get getNombre => nombre; //Creacion de los getters
                int? get getEdad => edad;
            }

            void main(List<String> args) {
                final usuario1 = User(nombre: "Alex", edad: 50); //Creacion de la instancia User con su contruccion
                print(usuario1.nombre);
                print(usuario1.edad);
            }
##
  ## Varios constructores para una clase
  ### Ejemplos:
            class User {
                String? nombre;
                int? edad;

                User.nombre(this.nombre); //Constructor para la propieda nombre
                User.edad(this.edad); //Constructor para la propiedad edad

                String? get getNombre => nombre;
                int? get getEdad => edad;
            }

            void main(List<String> args) {
                final usuario1 = User.nombre("Alex"); //Creacion de la instancia usuario1 con el constructor nombre
                final usuario2 = User.edad(50); //Creacion de la instancia usuario2 con el constructor edad

                print(usuario1.getNombre);
                print(usuario1.getEdad);

                print(usuario2.getEdad);
                print(usuario2.getNombre);
            }
##
            class User {
                String? _nombre;
                int? _edad;

            User.nombre(String nombre) {
                _nombre = nombre;
                _edad = 0;
            }

            User.edad(int edad) {
                _nombre = "-";
                _edad = edad;
            }

            String? get getNombre => _nombre;
            int? get getEdad => _edad;
            }

            void main(List<String> args) {
                final usuario1 = User.nombre("Alex");
                final usuario2 = User.edad(50);

                print(usuario1.getNombre);
                print(usuario1.getEdad);

                print(usuario2.getEdad);
                print(usuario2.getNombre);
            }
##
  ## Herencia y polimorfismo.
  ### Herencia
   - #### Mecanismo con el que se puede extender la funcionalidad de una clase
   - #### Por ejemplo usuario puede ser:
      - #### Estudiante.
      - #### Profesor.
      - #### Directivo.
      - #### Etc.
  
  #### Ejemplos:
  
            class Estudiante {
                String nombre = "";
                int edad = 0;

                void mostrarDatos() {
                print("Nombre: $nombre");
                print("Edad: $edad");
                }
            }

            class Profesor {
                String nombre = "";
                int edad = 0;

                void mostrarDatos() {
                print("Nombre: $nombre");
                print("Edad: $edad");
                }
            }

            class Directivo {
                String nombre = "";
                int edad = 0;

                void mostrarDatos() {
                print("Nombre: $nombre");
                print("Edad: $edad");
                }
            }

            void main(List<String> args) {
                final estudiante1 = Estudiante();
                estudiante1.nombre = "Diana";
                estudiante1.edad = 15;
                estudiante1.mostrarDatos();

                final profesor1 = Profesor();
                profesor1.nombre = "Edgar";
                profesor1.edad = 25;
                profesor1.mostrarDatos();

                final directivo1 = Directivo();
                directivo1.nombre = "Juan";
                directivo1.edad = 30;
                directivo1.mostrarDatos();
                }


##
                class User {
                    String nombre = "";
                    int edad = 0;

                    void mostrarDatos() {
                    print("Nombre: $nombre");
                    print("Edad: $edad");
                    }
                }

                class Estudiante extends User {}
                class Profesor extends User{}
                class Directivo extends User{}

                void main(List<String> args) {
                    final estudiante1 = Estudiante();
                    estudiante1.nombre = "Hugo";
                    estudiante1.edad = 15;
                    estudiante1.mostrarDatos();

                    final profesor1 = Profesor();
                    profesor1.nombre = "Paco";
                    profesor1.edad = 25;
                    profesor1.mostrarDatos();

                    final directivo1 = Directivo();
                    directivo1.nombre = "Luis";
                    directivo1.edad = 30;
                    directivo1.mostrarDatos();
                }
##

  ## Polimorfismo
   - #### Mecanismo que permite a las instancias de una clase acceder a  los distintos métodos de las clases relacionadas con el tiempo de ejecución. 
##
  ## Sobreescritura de metodos (Overriding)
  ### Ejemplos:
                class User {
                    String nombre = "";
                    int edad = 0;

                    void mostrarDatos() {
                    print("Nombre: $nombre");
                    print("Edad: $edad");
                    }
                }

                class Estudiante extends User {
                    @override
                    void mostrarDatos() {
                    print("Estudiante: $nombre");
                    print("Edad: $edad");
                    }
                }

                class Profesor extends User{}
                class Directivo extends User{}

                void main(List<String> args) {
                    final estudiante1 = Estudiante();
                    estudiante1.nombre = "Hugo";
                    estudiante1.edad = 15;
                    estudiante1.mostrarDatos();

                    final profesor1 = Profesor();
                    profesor1.nombre = "Paco";
                    profesor1.edad = 25;
                    profesor1.mostrarDatos();

                    final directivo1 = Directivo();
                    directivo1.nombre = "Luis";
                    directivo1.edad = 30;
                    directivo1.mostrarDatos();
                }
##
  ## Uso del constructor super
  ### Ejemplos:
                class User {
                    String nombre = "";
                    int edad = 0;
                    User(this.nombre, this.edad);

                    void mostrarDatos() {
                    print("Nombre: $nombre");
                    print("Edad: $edad");
                    }
                }

                class Estudiante extends User {
                    Estudiante(String nombre, int edad) : super(nombre, edad);
                }

                class Profesor extends User {
                    Profesor(String nombre, int edad) : super(nombre, edad);
                }

                class Directivo extends User {
                    Directivo(String nombre, int edad) : super(nombre, edad);
                }

                void main(List<String> args) {
                    final estudiante1 = Estudiante("Hugo", 15);
                    estudiante1.mostrarDatos();

                    final profesor1 = Profesor("Paco", 25);
                    profesor1.mostrarDatos();

                    final directivo1 = Directivo("Luis", 30);
                    directivo1.mostrarDatos();
                }

##
  ## Ejecucion de metodos de la superclase
  ### Ejemplos:
  
                class User {
                    String nombre = "";
                    int edad = 0;
                    User(this.nombre, this.edad);

                    void mostrarDatos() {
                    print("Nombre: $nombre");
                    print("Edad $edad");
                    }
                }

                class Estudiante extends User {
                    Estudiante(String nombre, int edad) : super(nombre, edad);
                    @override
                    
                    void mostraDatos() {
                    print("Estudiante");
                    super.mostrarDatos();
                    }
                }

                class Profesor extends User {
                    Profesor(String nombre, int edad) : super(nombre, edad);
                    @override
                    
                    void mostraDatos() {
                    print("Profesor");
                    super.mostrarDatos();
                    }
                }

                class Directivo extends User {
                    Directivo(String nombre, int edad) : super(nombre, edad);

                    @override
                    void mostraDatos() {
                    print("Directivo");
                    super.mostrarDatos();
                    }
                }

                void main(List<String> args) {
                    final estudiante1 = Estudiante("Hugo", 15);
                    estudiante1.mostrarDatos();

                    final profesor1 = Profesor("Paco", 25);
                    profesor1.mostrarDatos();

                    final directivo1 = Directivo("Luis", 30);
                    directivo1.mostrarDatos();
                }
##
  ## Clase Abstractas con metodos
  
  - ### Permites la creacion de metodos y propiedades generales sin su implementacion
  - ### No son instanciables

##
  ### Ejemplos:

                abstract class User {
                    String? nombre;
                    int? edad;

                    void mostarDatos();
                }

                class Estudiante extends User {
                    void mostrarDatos() {
                        print("Estudiante");
                        print("Nombre: $nombre");
                        print("Edad: $edad");
                    }
                }

                void main(List<String> args) {
                
                    final estudiante1 = Estudiante();
                    estudiante1.nombre = "Alex";
                    estudiante1.edad = 50;
                    estudiante1.mostarDatos();
                }

##
  ## Clases abstractas con constructores
  ### Ejemplos:
                abstract class User {
                    String? nombre;
                    int? edad;

                    User(this.nombre, this.edad);
                    void mostrarDatos();
                }

                class Estudiante extends User {
                    Estudiante(String nombre, int edad) : super(nombre, edad);
                    void mostrarDatos() {
                        print("Estudiante");
                        print("Nombre $nombre");
                        print("Edad: $edad");
                    }
                }

                void main(List<String> args) {
                    final estudiante1 = Estudiante("Alex", 50);
                    estudiante1.mostrarDatos();
                }
##
  ## Interfaces
  ### Ejemplos:
                class User {
                    String? nombre;
                    int? edad;

                    void mostrarDatos() {}
                }

                class Estudiante implements User {
                    String? nombre;
                    int? edad;

                    void mostrarDatos() {
                        print("Estudiante");
                        print("Nombre $nombre");
                        print("Edad $edad");
                    }
                }

                void main(List<String> args) {
                    final estudiante1 = Estudiante();
                    estudiante1.nombre = "Alex";
                    estudiante1.edad = 52;
                    estudiante1.mostrarDatos();
                }

##
  ## Multi-Interfaces
  ### Ejemplos:
                class User {
                    String? nombre;
                    int? edad;

                    void mostrarDatos() {}
                }
                class Estudiante implements User, Materia {
                    String? nombre;
                    int? edad;
                    String? materia;

                void mostrarDatos() {
                    print("Estudiante");
                    print("Nombre: $nombre");
                    print("Edad $edad");
                    }
                }

                class Materia {
                    String? materia;
                }

                void main(List<String> args) {
                    final estudiante1 = Estudiante();
                    estudiante1.nombre = "Alex";
                    estudiante1.edad = 50;
                    estudiante1.mostrarDatos();
                    estudiante1.materia = "Matematicas";
                    print("Materia: ${estudiante1.materia}");
                }

##
  ## Atributos y Metodos de clase (estaticos)
  ### Ejemplo: Propiedaes de instancia
  
                void main(List<String> args) {
                    final usuario1 = User();
                    final usuario2 = User();
                    print(usuario1.maxUsers);
                    print(usuario2.maxUsers);
                }

                class User {
                    int maxUsers = 10;
                }

  ### Ejemplo: Propiedades de clase
  
                void main(List<String> args) {
                    print(User.maxUsers);
                }

                class User {
                    static int maxUsers = 10;
                }

  ### Ejemplo: Metodos de clase
  
                void main(List<String> args) {
                    print(User.maxUsers);
                    print("Maximo de usuarios: ${User.getMAxUsers()}");
                }

                class User {
                    static int maxUsers = 10;
                    
                    static int getMAxUsers() {
                    return maxUsers;
                    }
                }


















