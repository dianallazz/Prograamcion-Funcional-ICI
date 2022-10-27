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

### _Lenguaje Dart_

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

clase del 10/10/2022

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


































