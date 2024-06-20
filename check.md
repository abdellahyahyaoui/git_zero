# **<FONT COLOR="teal">Checkpoint _6</font>**

  ##  ***<FONT COLOR="teal"> ¿Para qué usamos Clases en Python?</FONT>***

### *En Python, las clases son una parte fundamental de la programación orientada a objetos **(POO)**. Nos permiten encapsular datos y funciones relacionadas en una sola entidad, facilitando la reutilización del código y la organización del programa.*

### *Las clases en Python nos ayudan a modelar entidades del mundo real o conceptos abstractos en nuestro código. Por ejemplo, si estamos desarrollando un juego, podríamos tener una clase Jugador para representar a cada jugador en el juego, con propiedades como nombre, puntuación, nivel, etc., y métodos para realizar acciones como moverse, atacar, etc.*

 ### *"Una clase define una plantilla o molde para crear objetos, los cuales son instancias de esa clase. Los objetos creados a partir de una clase tienen las mismas propiedades y comportamientos definidos por la clase, pero pueden tener valores diferentes para los atributos que se definen en la clase.En Python, una clase se define mediante la palabra clave «class», seguida del nombre de la clase y dos puntos (:) y luego el cuerpo de la clase. El cuerpo de la clase contiene definiciones de métodos y atributos, que pueden ser públicos o privados según su acceso."*

 # "Ventajas y desventajas del uso de las clases en Python

 ## Ventajas

 ### Reutilización de código:
  *las clases pueden reutilizarse en diferentes partes del programa o en distintos programas, lo que ahorra tiempo y reduce la duplicación de código.*
  ### Encapsulación:
   *permiten ocultar la complejidad de un objeto y exponer solo una interfaz simple y fácil de usar para interactuar con él.*
  ### Modularidad: 
  *pueden descomponer un programa en componentes más pequeños y manejables, lo que facilita el mantenimiento y la solución de problemas.*
  ### Polimorfismo: 
  *ayudan a implementar el mismo conjunto de métodos con diferentes comportamientos para distintos tipos de objetos, lo que permite una mayor flexibilidad y extensibilidad en el diseño de programas.*
  ## Desventajas

  ### Sobrecarga de complejidad:
   *las clases pueden agregar complejidad adicional a un programa y hacer que sea más difícil de entender y depurar.*
   ### Curva de aprendizaje: 
   *el aprendizaje de las clases y la programación orientada a objetos en general pueden requerir una curva de aprendizaje más pronunciada para los programadores principiantes.*
   ### Uso innecesario: 
   *a veces, las clases se utilizan innecesariamente en situaciones en las que una función simple podría haber hecho el trabajo de manera más eficiente.*
 ## <FONT COLOR="teal"> ***¿Qué método se ejecuta automáticamente cuando se crea una instancia de una clase?:</FONT>***

### En la definición de una clase suele haber un método llamado __init__ que se conoce como inicializador. Este método es un método especial que se llama cada vez que se instancia una clase y sirve para inicializar el objeto que se crea. Este método crea los atributos que deben tener todos los objetos de la clase y por tanto contiene los parámetros necesarios para su creación, pero no devuelve nada. Se invoca cada vez que se instancia un objeto de esa clase.
### El método que se ejecuta automáticamente cuando se crea una instancia de una clase en Python es __init__(), que se conoce como el constructor de la clase. Este método se utiliza para inicializar los atributos de la instancia. La palabra clave self se utiliza para hacer referencia a la instancia recién creada.
```python

class Coche:
    def __init__(self, marca, modelo):
        self.marca = marca
        self.modelo = modelo

mi_coche = Coche("BMW", "E90")
```
```python
>>> class Tarjeta:
...     def __init__(self, id, cantidad = 0):    # Inicializador
            self.id = id                         # Creación del atributo id  
...         self.saldo = cantidad                # Creación del atributo saldo
...         return
...     def mostrar_saldo(self):
...         print('El saldo es', self.saldo, '€')
...         return
>>> t = Tarjeta('1111111111', 1000)     # Creación de un objeto con argumentos             
>>> t.muestra_saldo()
El saldo es 1000 €
```
## Atributos de instancia vs atributos de clase
*Los atributos que se crean dentro del método __init__ se conocen como atributos del objeto, mientras que los que se crean fuera de él se conocen como atributos de la clase. Mientras que los primeros son propios de cada objeto y por tanto pueden tomar valores distintos, los valores de los atributos de la clase son los mismos para cualquier objeto de la clase.*

### En general, no deben usarse atributos de clase, excepto para almacenar valores constantes.
```python
>>> class Circulo:
...     pi = 3.14159                     # Atributo de clase
...     def __init__(self, radio):
...         self.radio = radio           # Atributo de instancia
...     def area(self):
...         return Circulo.pi * self.radio ** 2
... 
>>> c1 = Circulo(2)
>>> c2 = Circulo(3)
>>> print(c1.area())
12.56636
>>> print(c2.area())
28.27431
>>> print(c1.pi)
3.14159
>>> print(c2.pi)
3.14159
```


  ## ***<FONT COLOR="teal">¿Cuáles son los tres verbos de API?</FONT>***

### **Los tres verbos principales de una API son:**

1. ### GET:Se utiliza para recuperar datos del servidor. 
   
 Por ejemplo,

  *al solicitar información de un usuario mediante una solicitud GET a una **API** de redes sociales.*

2. ### POST: Se utiliza para enviar datos nuevos al servidor. 
 Por ejemplo,

 *al enviar un nuevo tweet a través de una API de Twitter.*
 
3. ### **DELETE: Se utiliza para eliminar datos del servidor.** 

Por ejemplo,

 *al eliminar una publicación de un usuario en una red social.*
### **Estos verbos son parte del protocolo **HTTP** y se utilizan para interactuar con los recursos en un servidor.**

 ## ***<FONT COLOR="teal"> ¿Es MongoDB una base de datos SQL o NoSQL?</FONT>***

### MongoDB es una base de datos NoSQL. A diferencia de las bases de datos SQL tradicionales, que se basan en un modelo de datos relacional y utilizan tablas para almacenar datos, MongoDB utiliza un modelo de datos de documentos. Los datos se almacenan en documentos **JSON-like**, lo que proporciona flexibilidad y escalabilidad para manejar datos no estructurados o semi-estructurados.
*MongoDB es una base de datos orientada a documentos. Esto quiere decir que en lugar de guardar los datos en registros, guarda los datos en documentos. Estos documentos son almacenados en BSON, que es una representación binaria de JSON.*

*Esto representa una de las diferencias más importantes con respecto a las bases de datos relacionales. Y resulta que no es que no es necesario seguir un esquema. Los documentos de una misma colección - concepto similar a una tabla de una base de datos relacional -, pueden tener esquemas diferentes.*

*Imaginemos que tenemos una colección a la que llamamos Personas. Un documento podría almacenarse de la siguiente manera:*
```
{

   Nombre: "Miguel",
   Apellidos: "Parada",
   Edad: 39,
   Aficiones: ["Música","Ciclismo","Baloncesto"],
   Amigos: [
       {
         Nombre:"Marie",
         Edad:35    },
       {
         Nombre:"Elsa", 
         Edad:42
       }
   ]
} 
```
*Como se puede ver el documento es exactamente igual a lo que conocemos de un documento JSON.*

*Lo interesante viene cuando queremos almacenar en una misma colección un documento como este: { Nombre: "Roger Rabbit", Estudios: "Dibu y conejo", Amigos:102 } Tal como podemos ver, este no sigue el mismo esquema del primero, añadiendo algún campo nuevo que no existe en el documento anterior o incluso de un tipo distinto, pero no importa. Algo que resulta impensable en una base de datos relacional como SQL es posible en MongoDB.*

## Ventajas y desventajas
*¿Sirve MongoDB para todo y todo? Antes de entrar a definir por qué usar MondoDB en tu proyecto, conviene revisar pros y contras. MongoDB es un recurso muy interesante para desarrolladores pero no es perfecto.* ***Por ejemplo:***

### VENTAJAS

*Validación de documentos
1. Motores de almacenamiento integrado
2. Menor tiempo de recuperación ante fallos
   
### DESVENTAJAS

1. No es una solución adecuada para aplicaciones con transacciones complejas
2. No tiene un reemplazo para las soluciones de herencia
Aún es una tecnología joven

 ## <FONT COLOR="teal"> ¿Qué es una API?</FONT>

### *Una API **(Interfaz de Programación de Aplicaciones)** es un conjunto de reglas y protocolos que permite que diferentes aplicaciones se comuniquen entre sí. Proporciona una forma estandarizada para que las aplicaciones accedan a los datos y funcionalidades de otras aplicaciones, servicios o sistemas operativos.*

### *En el contexto del desarrollo de software, una API define cómo interactuar con un sistema para realizar ciertas acciones o acceder a ciertos recursos.* 

## ¿Cómo funciona una API?
L*as API permiten que sus productos y servicios se comuniquen con otros, sin necesidad de saber cómo están implementados. Esto simplifica el desarrollo de las aplicaciones y permite ahorrar tiempo y dinero. Las API le otorgan flexibilidad; simplifican el diseño, la administración y el uso de las aplicaciones; y ofrecen oportunidades de innovación, lo cual es ideal al momento de diseñar herramientas y productos nuevos (o de gestionar los actuales).*

*A veces, las API se consideran como contratos, con documentación que representa un acuerdo entre las partes: si una de las partes envía una solicitud remota con cierta estructura en particular, esa misma estructura determinará cómo responderá el software de la otra parte.*

*También permiten la colaboración entre el equipo comercial y el de TI, ya que simplifican la forma en que los desarrolladores integran los elementos de las aplicaciones nuevas en una arquitectura actual. Las necesidades comerciales suelen cambiar rápidamente en respuesta a los mercados digitales en constante cambio, donde la competencia puede modificar un sector entero con una aplicación nueva. Para seguir siendo competitivos, es importante admitir la implementación y el desarrollo rápidos de servicios innovadores. El desarrollo de aplicaciones nativas de la nube es una forma identificable de aumentar la velocidad de desarrollo y se basa en la conexión de una arquitectura de aplicaciones de microservicios a través de las API.*

*Las API son un medio simplificado para conectar su propia infraestructura a través del desarrollo de aplicaciones nativas de la nube, pero también le permiten compartir sus datos con clientes y otros usuarios externos. Las API públicas aportan un valor comercial único porque simplifican y amplían sus conexiones con los partners y, además, pueden rentabilizar sus datos (un ejemplo conocido es la API de Google Maps).*





## Por ejemplo, 
*una API de redes sociales podría permitir a los desarrolladores acceder a los perfiles de usuario, publicar nuevos mensajes o buscar publicaciones existentes.*

 ## ***<FONT COLOR="teal"> ¿Qué es Postman?</FONT>***

## **Postman es una herramienta popular utilizada por los desarrolladores para probar, documentar y compartir APIs. Proporciona una interfaz gráfica de usuario que permite enviar solicitudes HTTP a endpoints específicos, ver las respuestas del servidor y realizar pruebas de integración para asegurar el correcto funcionamiento de una API.**

### *Postman también ofrece características avanzadas como la automatización de pruebas, la creación de colecciones de solicitudes para compartir con otros miembros del equipo, y la generación de documentación para <FONT COLOR="RED">APIs</FONT>.*

  ## <FONT COLOR="teal"> ***¿Qué es el polimorfismo?***</FONT>

### El polimorfismo es un concepto de la programación orientada a objetos que permite tratar objetos de diferentes clases de manera uniforme. Esto significa que un objeto puede comportarse de múltiples maneras dependiendo del contexto en el que se utiliza.

### En Python, el polimorfismo se logra mediante la implementación de métodos con el mismo nombre en diferentes clases. Cada clase puede tener su propia implementación de estos métodos, lo que permite que los objetos de esas clases respondan de manera diferente a la misma llamada de método.

 ## ***<FONT COLOR="teal">¿Qué es un método dunder?***
  </FONT>

### *Un método dunder ***(del inglés "double underscore")*** es un método especial en Python que tiene dos guiones bajos al principio y al final de su nombre. Estos métodos también se conocen como métodos mágicos o métodos especiales. Son utilizados por Python para realizar operaciones específicas en objetos.*

### *Algunos ejemplos de métodos dunder son *____init__ __()* para la inicialización de objetos, *____str__ __()*  para la representación de cadenas, y *____add__ __()*  para la sobrecarga del operador de suma *(+)*. Estos métodos permiten que los objetos de una clase respondan a ciertas operaciones de manera personalizada*.

## ____init__ __: Este método se llama automáticamente cuando se crea una nueva instancia de una clase. Se utiliza para inicializar los atributos de la clase.

```python

class Persona:
    def __init__(self, nombre, edad):
        self.nombre = nombre
        self.edad = edad

persona1 = Persona("Juan", 30)




```
## ____str__ __: Este método se utiliza para devolver una representación de cadena legible para humanos del objeto.
```python
class Persona:
    def __init__(self, nombre, edad):
        self.nombre = nombre
        self.edad = edad
    
    def __str__(self):
        return f"Nombre: {self.nombre}, Edad: {self.edad}"

persona1 = Persona("Juan", 30)
print(persona1)  # Imprimirá: Nombre: Juan, Edad: 30

```
## ____add__ __: Este método permite definir la operación de suma para objetos de la clase.
```python
class Punto:
    def __init__(self, x, y):
        self.x = x
        self.y = y
    
    def __add__(self, otro):
        return Punto(self.x + otro.x, self.y + otro.y)

punto1 = Punto(1, 2)
punto2 = Punto(3, 4)
resultado = punto1 + punto2
print(resultado.x, resultado.y)  # Imprimirá: 4 6

```
## ____len__ __: Este método se utiliza para devolver la longitud de un objeto.
```python
class MiLista:
    def __init__(self, elementos):
        self.elementos = elementos
    
    def __len__(self):
        return len(self.elementos)

lista = MiLista([1, 2, 3, 4, 5])
print(len(lista))  # Imprimirá: 5

```

***Estos son solo algunos ejemplos de los muchos métodos dunder que existen en Python. Se utilizan para personalizar el comportamiento de los objetos según las necesidades de la aplicación.***


## ***<FONT COLOR="teal">  ¿Qué es un decorador de Python?</FONT>***

## Un decorador en Python es una función que toma otra función como argumento y devuelve una nueva función modificada. Los decoradores se utilizan para agregar funcionalidad adicional a una función existente sin modificar su código interno. Esto permite extender o modificar el comportamiento de una función de manera modular y reutilizable.

  ## Por ejemplo, 

  *un decorador puede ser utilizado para realizar la validación de entrada antes de ejecutar una función, para medir el tiempo de ejecución de una función, o para manejar errores de manera centralizada.*
  ```py
  def decorador(funcion):
    def wrapper(*args, **kwargs):
        # Agregar funcionalidad adicional antes de llamar a la función
        resultado = funcion(*args, **kwargs)
        # Agregar funcionalidad adicional después de llamar a la función
        return resultado
    return wrapper

@decorador
def funcion_a_decorar():
    pass
    
```

### En este ejemplo, 
***'decorador'*** es una función que toma ***'funcion_a_decorar'*** como argumento y devuelve una nueva función *'wrapper'* que envuelve la función original. Esto permite agregar funcionalidad adicional antes y después de llamar a ***'funcion_a_decorar'***.



```py
import time

def calcular_tiempo_ejecucion(funcion):
    def wrapper(*args, **kwargs):
        inicio = time.time()
        resultado = funcion(*args, **kwargs)
        fin = time.time()
        print(f"Tiempo de ejecución de {funcion.__name__}: {fin - inicio} segundos")
        return resultado
    return wrapper

# Decorador para medir el tiempo de ejecución de una función
@calcular_tiempo_ejecucion
def suma(a, b):
    time.sleep(1)  # Simulamos una función que tarda 1 segundo en ejecutarse
    return a + b

resultado = suma(3, 5)
print("Resultado de la suma:", resultado)

```



*En este ejemplo, calcular_tiempo_ejecucion es el decorador. Toma una función como argumento, crea y devuelve una función envoltura (wrapper) que mide el tiempo de ejecución antes y después de llamar a la función original.*

*Luego, decoramos la función suma con @calcular_tiempo_ejecucion. Cuando llamamos a suma(3, 5), en realidad estamos llamando a wrapper(3, 5), que mide el tiempo antes y después de ejecutar la función suma original y luego devuelve el resultado.*

*Esto nos permite medir el tiempo de ejecución de la función suma sin modificar su implementación original.*