# **<FONT COLOR="teal">Checkpoint _6</font>**

  ##  ***<FONT COLOR="teal"> ¿Para qué usamos Clases en Python?</FONT>***

### *En Python, las clases son una parte fundamental de la programación orientada a objetos **(POO)**. Nos permiten encapsular datos y funciones relacionadas en una sola entidad, facilitando la reutilización del código y la organización del programa.*

### *Las clases en Python nos ayudan a modelar entidades del mundo real o conceptos abstractos en nuestro código. Por ejemplo, si estamos desarrollando un juego, podríamos tener una clase Jugador para representar a cada jugador en el juego, con propiedades como nombre, puntuación, nivel, etc., y métodos para realizar acciones como moverse, atacar, etc.*

 ## <FONT COLOR="teal"> ***¿Qué método se ejecuta automáticamente cuando se crea una instancia de una clase?:</FONT>***

### El método que se ejecuta automáticamente cuando se crea una instancia de una clase en Python es __init__(), que se conoce como el constructor de la clase. Este método se utiliza para inicializar los atributos de la instancia. La palabra clave self se utiliza para hacer referencia a la instancia recién creada.
```python

class Coche:
    def __init__(self, marca, modelo):
        self.marca = marca
        self.modelo = modelo

mi_coche = Coche("BMW", "E90")
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

 ## <FONT COLOR="teal"> ¿Qué es una API?</FONT>

### *Una API **(Interfaz de Programación de Aplicaciones)** es un conjunto de reglas y protocolos que permite que diferentes aplicaciones se comuniquen entre sí. Proporciona una forma estandarizada para que las aplicaciones accedan a los datos y funcionalidades de otras aplicaciones, servicios o sistemas operativos.*

### *En el contexto del desarrollo de software, una API define cómo interactuar con un sistema para realizar ciertas acciones o acceder a ciertos recursos.* 
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
