```
eslint
liveserver
prettier
markdown
devcamp
Secuencia de Escape	Descripción
\n	Nueva línea
\t	Tabulación horizontal
\\	Barra invertida (backslash)
\"	Comillas dobles
\'	Comillas simples
\r	Retorno de carro
\b	Retroceso
\f	Salto de página
\a	Alerta (campana)
\v	Tabulación vertical
\0	Carácter nulo
\xhh	Carácter con valor hexadecimal hh

```

```python
           Métodos de Cadenas (Strings)

.capitalize()   # Convierte el primer carácter de la cadena a mayúscula.
.casefold()     # Convierte la cadena a minúsculas, más agresivo que lower().
.center(width)  # Centra la cadena en un ancho especificado, rellenando con espacios.
.count(sub)     # Cuenta las apariciones de un subcadena en la cadena.
.encode()       # Codifica la cadena en bytes usando una codificación especificada.
.endswith(suffix)   # Verifica si la cadena termina con el sufijo especificado.
.expandtabs(tabsize) # Expande los tabuladores en espacios.
.find(sub)      # Devuelve el índice de la primera aparición de la subcadena, -1 si no se encuentra.
.format(*args, **kwargs) # Formatea la cadena usando los argumentos especificados.
.index(sub)     # Igual que find(), pero genera un ValueError si no se encuentra la subcadena.
.isalnum()      # Verifica si todos los caracteres de la cadena son alfanuméricos.
.isalpha()      # Verifica si todos los caracteres de la cadena son letras.
.isdecimal()    # Verifica si todos los caracteres de la cadena son decimales.
.isdigit()      # Verifica si todos los caracteres de la cadena son dígitos.
.islower()      # Verifica si todos los caracteres de la cadena están en minúsculas.
.isnumeric()    # Verifica si todos los caracteres de la cadena son numéricos.
.isspace()      # Verifica si todos los caracteres de la cadena son espacios en blanco.
.istitle()      # Verifica si la cadena está en formato de título.
.isupper()      # Verifica si todos los caracteres de la cadena están en mayúsculas.
.join(iterable) # Une un iterable de cadenas con la cadena como delimitador.
.ljust(width)   # Justifica la cadena a la izquierda en un ancho especificado.
.lower()        # Convierte todos los caracteres de la cadena a minúsculas.
.lstrip()       # Elimina los espacios en blanco al inicio de la cadena.
.partition(sep) # Divide la cadena en tres partes usando el separador especificado.
.replace(old, new) # Reemplaza las ocurrencias de una subcadena por otra.
.rfind(sub)     # Igual que find(), pero busca desde el final de la cadena.
.rindex(sub)    # Igual que index(), pero busca desde el final de la cadena.
.rjust(width)   # Justifica la cadena a la derecha en un ancho especificado.
.rpartition(sep) # Igual que partition(), pero busca desde el final de la cadena.
.rsplit(sep)    # Divide la cadena en una lista usando el separador especificado.
.rstrip()       # Elimina los espacios en blanco al final de la cadena.
.split(sep)     # Divide la cadena en una lista usando el separador especificado.
.splitlines()   # Divide la cadena en una lista por líneas.
.startswith(prefix) # Verifica si la cadena comienza con el prefijo especificado.
.strip()        # Elimina los espacios en blanco al inicio y al final de la cadena.
.swapcase()     # Invierte el caso de todos los caracteres de la cadena.
.title()        # Convierte la cadena a formato de título.
.upper()        # Convierte todos los caracteres de la cadena a mayúsculas.
.zfill(width)   # Rellena la cadena con ceros a la izquierda hasta un ancho especificado.

```

# metodos de lista

```python
# append: agrega un elemento al final de la lista
lista = [1, 2, 3]
lista.append(4)
print(lista)  # [1, 2, 3, 4]

# extend: extiende la lista agregando todos los elementos de otro iterable
lista.extend([5, 6])
print(lista)  # [1, 2, 3, 4, 5, 6]

# insert: inserta un elemento en una posición específica
lista.insert(1, 'a')
print(lista)  # [1, 'a', 2, 3, 4, 5, 6]

# remove: elimina la primera aparición de un valor específico
lista.remove('a')
print(lista)  # [1, 2, 3, 4, 5, 6]

# pop: elimina y devuelve el elemento en una posición específica (por defecto el último)
elemento = lista.pop()
print(elemento)  # 6
print(lista)     # [1, 2, 3, 4, 5]

# clear: elimina todos los elementos de la lista
lista.clear()
print(lista)  # []

# index: devuelve el índice de la primera aparición de un valor específico
lista = [1, 2, 3, 4, 5]
indice = lista.index(3)
print(indice)  # 2

# count: devuelve el número de apariciones de un valor específico en la lista
contador = lista.count(3)
print(contador)  # 1

# sort: ordena los elementos de la lista
lista.sort()
print(lista)  # [1, 2, 3, 4, 5]

# reverse: invierte el orden de los elementos de la lista
lista.reverse()
print(lista)  # [5, 4, 3, 2, 1]

# copy: devuelve una copia superficial de la lista
copia = lista.copy()
print(copia)  # [5, 4, 3, 2, 1]

```

# metodos de cadenas

```python
# upper: convierte todos los caracteres de la cadena a mayúsculas
cadena = "hola"
print(cadena.upper())  # HOLA

# lower: convierte todos los caracteres de la cadena a minúsculas
print(cadena.lower())  # hola

# capitalize: convierte el primer carácter de la cadena a mayúsculas
print(cadena.capitalize())  # Hola

# title: convierte el primer carácter de cada palabra a mayúsculas
print(cadena.title())  # Hola

# strip: elimina los espacios en blanco al inicio y al final de la cadena
cadena_espacios = "  hola  "
print(cadena_espacios.strip())  # "hola"

# lstrip: elimina los espacios en blanco al inicio de la cadena
print(cadena_espacios.lstrip())  # "hola  "

# rstrip: elimina los espacios en blanco al final de la cadena
print(cadena_espacios.rstrip())  # "  hola"

# split: divide la cadena en una lista utilizando un delimitador
print(cadena.split())  # ['hola']

# join: une una lista de cadenas en una sola cadena con un delimitador
lista_cadenas = ['hola', 'mundo']
print(" ".join(lista_cadenas))  # "hola mundo"

# find: devuelve el índice de la primera aparición de una subcadena
print(cadena.find('o'))  # 1

# replace: reemplaza todas las apariciones de una subcadena por otra
print(cadena.replace('o', 'a'))  # hala

# isdigit: verifica si todos los caracteres de la cadena son dígitos
print(cadena.isdigit())  # False

# isalpha: verifica si todos los caracteres de la cadena son letras
print(cadena.isalpha())  # True

```

# Métodos de diccionarios

```python
# keys: devuelve una vista de las claves del diccionario
dic = {'a': 1, 'b': 2}
print(dic.keys())  # dict_keys(['a', 'b'])

# values: devuelve una vista de los valores del diccionario
print(dic.values())  # dict_values([1, 2])

# items: devuelve una vista de los pares clave-valor del diccionario
print(dic.items())  # dict_items([('a', 1), ('b', 2)])

# get: devuelve el valor asociado a una clave, o un valor por defecto si la clave no existe
print(dic.get('a'))  # 1
print(dic.get('c', 'No existe'))  # No existe

# pop: elimina una clave y devuelve su valor
valor = dic.pop('a')
print(valor)  # 1
print(dic)    # {'b': 2}

# popitem: elimina y devuelve un par clave-valor aleatorio del diccionario
par = dic.popitem()
print(par)  # ('b', 2)
print(dic)  # {}

# update: actualiza el diccionario con pares clave-valor de otro diccionario o iterables de pares clave-valor
dic.update({'c': 3, 'd': 4})
print(dic)  # {'c': 3, 'd': 4}

# clear: elimina todos los elementos del diccionario
dic.clear()
print(dic)  # {}

# copy: devuelve una copia superficial del diccionario
dic = {'e': 5, 'f': 6}
copia_dic = dic.copy()
print(copia_dic)  # {'e': 5, 'f': 6}

# setdefault: devuelve el valor de una clave, si no existe, inserta la clave con un valor por defecto
valor = dic.setdefault('g', 7)
print(valor)  # 7
print(dic)    # {'e': 5, 'f': 6, 'g': 7}

```

# Métodos de conjuntos

```python
# add: agrega un elemento al conjunto
conjunto = {1, 2, 3}
conjunto.add(4)
print(conjunto)  # {1, 2, 3, 4}

# remove: elimina un elemento del conjunto (lanza un error si el elemento no existe)
conjunto.remove(4)
print(conjunto)  # {1, 2, 3}

# discard: elimina un elemento del conjunto (no lanza error si el elemento no existe)
conjunto.discard(5)
print(conjunto)  # {1, 2, 3}

# pop: elimina y devuelve un elemento aleatorio del conjunto
elemento = conjunto.pop()
print(elemento)  # 1
print(conjunto)  # {2, 3}

# clear: elimina todos los elementos del conjunto
conjunto.clear()
print(conjunto)  # set()

# copy: devuelve una copia superficial del conjunto
conjunto = {1, 2, 3}
copia_conjunto = conjunto.copy()
print(copia_conjunto)  # {1, 2, 3}

# union: devuelve la unión de dos conjuntos
otro_conjunto = {3, 4, 5}
union = conjunto.union(otro_conjunto)
print(union)  # {1, 2, 3, 4, 5}

# intersection: devuelve la intersección de dos conjuntos
interseccion = conjunto.intersection(otro_conjunto)
print(interseccion)  # {3}

# difference: devuelve la diferencia de dos conjuntos
diferencia = conjunto.difference(otro_conjunto)
print(diferencia)  # {1, 2}

# symmetric_difference: devuelve la diferencia simétrica de dos conjuntos
dif_simetrica = conjunto.symmetric_difference(otro_conjunto)
print(dif_simetrica)  # {1, 2, 4, 5}

# issubset: verifica si un conjunto es subconjunto de otro
es_subconjunto = conjunto.issubset(otro_conjunto)
print(es_subconjunto)  # False

# issuperset: verifica si un conjunto es superconjunto de otro
es_superconjunto = conjunto.issuperset(otro_conjunto)
print(es_superconjunto)  # False

# isdisjoint: verifica si dos conjuntos son disjuntos (no tienen elementos en común)
es_disjunto = conjunto.isdisjoint(otro_conjunto)
print(es_disjunto)  # False


```

# Métodos de archivos

```python
# open: abre un archivo y devuelve un objeto de archivo
archivo = open('archivo.txt', 'w')
archivo.write('Hola, mundo!')
archivo.close()

# read: lee el contenido del archivo
archivo = open('archivo.txt', 'r')
contenido = archivo.read()
print(contenido)  # Hola, mundo!
archivo.close()

# readline: lee una línea del archivo
archivo = open('archivo.txt', 'r')
linea = archivo.readline()
print(linea)  # Hola, mundo!
archivo.close()

# readlines: lee todas las líneas del archivo y devuelve una lista
archivo = open('archivo.txt', 'r')
lineas = archivo.readlines()
print(lineas)  # ['Hola, mundo!']
archivo.close()

# write: escribe una cadena en el archivo
archivo = open('archivo.txt', 'w')
archivo.write('Nueva línea de texto\n')
archivo.write('Otra línea de texto\n')
archivo.close()

# writelines: escribe una lista de cadenas en el archivo
archivo = open('archivo.txt', 'w')
archivo.writelines(['Primera línea\n', 'Segunda línea\n'])
archivo.close()

# close: cierra el archivo
archivo.close()

# tell: devuelve la posición actual del cursor en el archivo
archivo = open('archivo.txt', 'r')
print(archivo.tell())  # 0
archivo.close()

# seek: mueve el cursor a una posición específica en el archivo
archivo = open('archivo.txt', 'r')
archivo.seek(5)
print(archivo.tell())  # 5
archivo.close()

```

# Métodos de módulos y paquetes

```python
# import: importa un módulo
import math
print(math.sqrt(16))  # 4.0

# from ... import: importa una función o variable específica de un módulo
from math import pi
print(pi)  # 3.141592653589793

# as: da un alias a un módulo o función importada
import math as m
print(m.sqrt(16))  # 4.0

# dir: lista los atributos y métodos de un módulo
import math
print(dir(math))

# help: muestra la documentación de un módulo, función o clase
help(math)


```

# E jemplos

```python
# Tipos de datos básicos
x = 10               # Entero
y = 3.14             # Flotante
texto = "Hola, Mundo" # Cadena
es_verdad = True     # Booleano

# Operadores básicos
suma = 5 + 3          # Suma
producto = 2 * 4      # Multiplicación
division = 10 / 2     # División
division_entera = 10 // 3  # División entera
modulo = 10 % 3       # Módulo
potencia = 2 ** 3     # Potencia

# Operadores de comparación
es_igual = 5 == 5     # True
es_diferente = 5 != 3 # True
es_mayor = 5 > 3      # True
es_menor = 5 < 3      # False
es_mayor_igual = 5 >= 3 # True
es_menor_igual = 5 <= 3 # False

# Operadores lógicos
condicion_and = (5 > 3) and (3 < 8)  # True
condicion_or = (5 > 3) or (3 > 8)    # True
condicion_not = not (5 > 3)          # False

# Estructuras de control
x = 10
if x > 5:
    print("x es mayor que 5")
elif x == 5:
    print("x es igual a 5")
else:
    print("x es menor que 5")

# Bucles
# Bucle for
for i in range(5):
    print(i)  # Imprime 0, 1, 2, 3, 4

# Bucle while
i = 0
while i < 5:
    print(i)  # Imprime 0, 1, 2, 3, 4
    i += 1

# Funciones
def saludar(nombre):
    return f"Hola, {nombre}"

mensaje = saludar("Carlos")
print(mensaje)  # Hola, Carlos

# Colecciones
# Listas
numeros = [1, 2, 3, 4, 5]
numeros.append(6)
print(numeros)  # [1, 2, 3, 4, 5, 6]

# Tuplas
dias = ("lunes", "martes", "miércoles")
print(dias[0])  # lunes

# Conjuntos (sets)
frutas = {"manzana", "banana", "cereza"}
frutas.add("naranja")
print(frutas)  # {'banana', 'naranja', 'manzana', 'cereza'}

# Diccionarios
edades = {"Alice": 30, "Bob": 25}
print(edades["Alice"])  # 30

# Comprensiones de listas
cuadrados = [x**2 for x in range(5)]
print(cuadrados)  # [0, 1, 4, 9, 16]

# Manejo de excepciones
try:
    division = 10 / 0
except ZeroDivisionError:
    print("No se puede dividir por cero")

# Clases y objetos
class Persona:
    def __init__(self, nombre, edad):
        self.nombre = nombre
        self.edad = edad

    def saludar(self):
        return f"Hola, me llamo {self.nombre} y tengo {self.edad} años"

persona = Persona("Carlos", 30)
print(persona.saludar())  # Hola, me llamo Carlos y tengo 30 años

# Más sobre listas
# Indexación y rebanado
numeros = [1, 2, 3, 4, 5]
print(numeros[0])     # 1
print(numeros[-1])    # 5
print(numeros[1:3])   # [2, 3]

# Métodos de listas
numeros.append(6)     # Añadir un elemento al final
numeros.remove(2)     # Eliminar el primer elemento con valor 2
print(numeros)        # [1, 3, 4, 5, 6]

# Métodos de cadenas
texto = "Hola, Mundo"
print(texto.lower())  # hola, mundo
print(texto.upper())  # HOLA, MUNDO
print(texto.split())  # ['Hola,', 'Mundo']
print(texto.replace("Mundo", "Python"))  # Hola, Python

# Diccionarios
edades = {"Alice": 30, "Bob": 25}
print(edades["Alice"])  # 30

# Métodos de diccionarios
edades["Charlie"] = 20  # Añadir un par clave-valor
del edades["Alice"]     # Eliminar una clave
print(edades)           # {'Bob': 25, 'Charlie': 20}

# Iterar sobre diccionarios
for nombre, edad in edades.items():
    print(f"{nombre} tiene {edad} años")

# Conjuntos (sets)
frutas = {"manzana", "banana", "cereza"}
frutas.add("naranja")
frutas.remove("banana")
print(frutas)  # {'manzana', 'naranja', 'cereza'}

# Operaciones con conjuntos
A = {1, 2, 3}
B = {3, 4, 5}
print(A | B)  # Unión: {1, 2, 3, 4, 5}
print(A & B)  # Intersección: {3}
print(A - B)  # Diferencia: {1, 2}

# Comprensiones de diccionarios y conjuntos
cuadrados = {x: x**2 for x in range(5)}
print(cuadrados)  # {0: 0, 1: 1, 2: 4, 3: 9, 4: 16}

pares = {x for x in range(10) if x % 2 == 0}
print(pares)  # {0, 2, 4, 6, 8}

# Funciones anónimas (lambda)
suma = lambda a, b: a + b
print(suma(2, 3))  # 5

# Funciones integradas más comunes
print(len(numeros))  # Longitud: 5
print(max(numeros))  # Máximo: 6
print(min(numeros))  # Mínimo: 1
print(sum(numeros))  # Suma: 19

# Map, filter, reduce
from functools import reduce
numeros = [1, 2, 3, 4, 5]
cuadrados = list(map(lambda x: x**2, numeros))
pares = list(filter(lambda x: x % 2 == 0, numeros))
producto = reduce(lambda x, y: x * y, numeros)

print(cuadrados)  # [1, 4, 9, 16, 25]
print(pares)      # [2, 4]
print(producto)   # 120

# Decoradores
def decorador(func):
    def nueva_funcion(*args, **kwargs):
        print("Función decorada")
        resultado = func(*args, **kwargs)
        return resultado
    return nueva_funcion

@decorador
def saludar(nombre):
    return f"Hola, {nombre}"

print(saludar("Carlos"))  # Función decorada \n Hola, Carlos

# Manejo de archivos
# Leer un archivo
with open("archivo.txt", "r") as archivo:
    contenido = archivo.read()
    print(contenido)

# Escribir en un archivo
with open("archivo.txt", "w") as archivo:
    archivo.write("Hola, archivo")

# Módulos y paquetes
# Importar módulos
import math
print(math.sqrt(16))  # 4.0

# Importar funciones específicas
from math import pi, sqrt
print(pi)            # 3.141592653589793
print(sqrt(16))      # 4.0

# Importar con alias
import numpy as np
array = np.array([1, 2, 3])
print(array)  # [1 2 3]

# Programación orientada a objetos
class Persona:
    def __init__(self, nombre, edad):
        self.nombre = nombre
        self.edad = edad

    def saludar(self):
        return f"Hola, me llamo {self.nombre} y tengo {self.edad} años"

class Empleado(Persona):
    def __init__(self, nombre, edad, salario):
        super().__init__(nombre, edad)
        self.salario = salario

    def saludar(self):
        return f"Hola, me llamo {self.nombre}, tengo {self.edad} años y gano {self.salario}"

empleado = Empleado("Carlos", 30, 50000)
print(empleado.saludar())  # Hola, me llamo Carlos, tengo 30 años y gano 50000


# Generadores
def generador():
    yield 1
    yield 2
    yield 3

gen = generador()
for valor in gen:
    print(valor)  # 1, 2, 3

# Expresiones generadoras
gen_exp = (x**2 for x in range(5))
for valor in gen_exp:
    print(valor)  # 0, 1, 4, 9, 16

# Manejo de contexto con 'with'
class Recurso:
    def __enter__(self):
        print("Recurso adquirido")
        return self

    def __exit__(self, tipo, valor, traceback):
        print("Recurso liberado")

with Recurso():
    print("Dentro del bloque with")

# Anotaciones de tipos
def suma(a: int, b: int) -> int:
    return a + b

print(suma(2, 3))  # 5

# Tipos avanzados con el módulo typing
from typing import List, Dict, Tuple

def procesar_lista(lista: List[int]) -> List[int]:
    return [x * 2 for x in lista]

def obtener_datos() -> Dict[str, int]:
    return {"a": 1, "b": 2}

# Clases abstractas
from abc import ABC, abstractmethod

class Animal(ABC):
    @abstractmethod
    def hacer_sonido(self):
        pass

class Perro(Animal):
    def hacer_sonido(self):
        return "Guau"

perro = Perro()
print(perro.hacer_sonido())  # Guau

# Propiedades
class Circulo:
    def __init__(self, radio):
        self._radio = radio

    @property
    def radio(self):
        return self._radio

    @radio.setter
    def radio(self, valor):
        if valor <= 0:
            raise ValueError("El radio debe ser positivo")
        self._radio = valor

circulo = Circulo(5)
print(circulo.radio)  # 5
circulo.radio = 10
print(circulo.radio)  # 10

# Métodos estáticos y de clase
class Matematica:
    @staticmethod
    def sumar(a, b):
        return a + b

    @classmethod
    def pi(cls):
        return 3.141592653589793

print(Matematica.sumar(2, 3))  # 5
print(Matematica.pi())         # 3.141592653589793

# Clases y métodos privados
class PersonaPrivada:
    def __init__(self, nombre, edad):
        self.__nombre = nombre  # Atributo privado
        self.__edad = edad      # Atributo privado

    def __saludar(self):        # Método privado
        return f"Hola, me llamo {self.__nombre} y tengo {self.__edad} años"

    def presentarse(self):
        return self.__saludar()

persona = PersonaPrivada("Carlos", 30)
print(persona.presentarse())  # Hola, me llamo Carlos y tengo 30 años

# Herencia múltiple
class A:
    def metodo(self):
        return "A"

class B:
    def metodo(self):
        return "B"

class C(A, B):
    pass

c = C()
print(c.metodo())  # A (MRO: Method Resolution Order)

# Decoradores de clase
def decorador_de_clase(cls):
    cls.decorado = True
    return cls

@decorador_de_clase
class MiClase:
    pass

print(MiClase.decorado)  # True

# Módulos y paquetes
# Estructura básica de un paquete
# paquete/
# ├── __init__.py
# ├── modulo1.py
# └── modulo2.py

# En __init__.py
from .modulo1 import funcion1
from .modulo2 import funcion2

# Importar el paquete
import paquete
paquete.funcion1()
paquete.funcion2()

# Importar desde submódulos
from paquete.modulo1 import funcion1
funcion1()

# Manejo de fechas y tiempos
from datetime import datetime, timedelta

ahora = datetime.now()
print(ahora)  # Fecha y hora actual

mañana = ahora + timedelta(days=1)
print(mañana)  # Fecha y hora de mañana

# Manejo de zonas horarias
import pytz

zona_horaria = pytz.timezone("America/New_York")
ahora_ny = datetime.now(zona_horaria)
print(ahora_ny)  # Fecha y hora actual en Nueva York

# Itertools para combinaciones y permutaciones
import itertools

# Combinaciones
combinaciones = list(itertools.combinations([1, 2, 3], 2))
print(combinaciones)  # [(1, 2), (1, 3), (2, 3)]

# Permutaciones
permutaciones = list(itertools.permutations([1, 2, 3]))
print(permutaciones)  # [(1, 2, 3), (1, 3, 2), (2, 1, 3), (2, 3, 1), (3, 1, 2), (3, 2, 1)]

# Enumerate para obtener índices en un bucle
numeros = [10, 20, 30]
for indice, valor in enumerate(numeros):
    print(indice, valor)  # 0 10, 1 20, 2 30

# Zip para iterar sobre múltiples iterables
nombres = ["Alice", "Bob", "Charlie"]
edades = [25, 30, 35]

for nombre, edad in zip(nombres, edades):
    print(nombre, edad)  # Alice 25, Bob 30, Charlie 35

# Slicing avanzado
lista = [0, 1, 2, 3, 4, 5]
print(lista[1:5:2])  # [1, 3] (start:end:step)
print(lista[::-1])   # [5, 4, 3, 2, 1, 0] (inverso)



# Más sobre generadores
def contador(inicio, fin):
    while inicio <= fin:
        yield inicio
        inicio += 1

for numero in contador(1, 5):
    print(numero)  # 1, 2, 3, 4, 5

# Decoradores con parámetros
def decorador_con_parametros(mensaje):
    def decorador(func):
        def nueva_funcion(*args, **kwargs):
            print(mensaje)
            return func(*args, **kwargs)
        return nueva_funcion
    return decorador

@decorador_con_parametros("Llamando a la función")
def saludar(nombre):
    return f"Hola, {nombre}"

print(saludar("Carlos"))  # Llamando a la función \n Hola, Carlos

# Contextlib para crear context managers
from contextlib import contextmanager

@contextmanager
def mi_contexto():
    print("Inicio del contexto")
    yield
    print("Fin del contexto")

with mi_contexto():
    print("Dentro del contexto")

# Atributos de clase vs atributos de instancia
class MiClase:
    atributo_clase = "Atributo de clase"

    def __init__(self, atributo_instancia):
        self.atributo_instancia = atributo_instancia

objeto = MiClase("Atributo de instancia")
print(objeto.atributo_clase)       # Atributo de clase
print(objeto.atributo_instancia)   # Atributo de instancia
print(MiClase.atributo_clase)      # Atributo de clase

# Métodos especiales (Dunder methods)
class Numero:
    def __init__(self, valor):
        self.valor = valor

    def __add__(self, otro):
        return self.valor + otro.valor

    def __str__(self):
        return str(self.valor)

num1 = Numero(10)
num2 = Numero(20)
print(num1 + num2)  # 30
print(num1)         # 10

# Serialización y deserialización (pickle)
import pickle

# Serializar (guardar)
datos = {"nombre": "Alice", "edad": 30}
with open("datos.pkl", "wb") as archivo:
    pickle.dump(datos, archivo)

# Deserializar (cargar)
with open("datos.pkl", "rb") as archivo:
    datos_cargados = pickle.load(archivo)
    print(datos_cargados)  # {'nombre': 'Alice', 'edad': 30}

# JSON
import json

# Serializar a JSON
datos_json = json.dumps(datos)
print(datos_json)  # {"nombre": "Alice", "edad": 30}

# Deserializar desde JSON
datos_cargados_json = json.loads(datos_json)
print(datos_cargados_json)  # {'nombre': 'Alice', 'edad': 30}

# Módulo collections
from collections import namedtuple, deque, Counter, defaultdict

# namedtuple
Punto = namedtuple('Punto', 'x y')
p = Punto(1, 2)
print(p.x, p.y)  # 1 2

# deque
dq = deque([1, 2, 3])
dq.appendleft(0)
print(dq)  # deque([0, 1, 2, 3])

# Counter
contador = Counter("abracadabra")
print(contador)  # Counter({'a': 5, 'b': 2, 'r': 2, 'c': 1, 'd': 1})

# defaultdict
dd = defaultdict(int)
dd['a'] += 1
print(dd)  # defaultdict(<class 'int'>, {'a': 1})

# Itertools para productos cartesianos
import itertools

producto = list(itertools.product([1, 2], ['a', 'b']))
print(producto)  # [(1, 'a'), (1, 'b'), (2, 'a'), (2, 'b')]

# Enumerate para iteración con índice
animales = ['gato', 'perro', 'elefante']
for indice, animal in enumerate(animales):
    print(indice, animal)  # 0 gato, 1 perro, 2 elefante

# Zip para iterar sobre múltiples listas
nombres = ['Alice', 'Bob', 'Charlie']
edades = [24, 50, 18]
for nombre, edad in zip(nombres, edades):
    print(f"{nombre} tiene {edad} años")

# Usando functools para memoización
from functools import lru_cache

@lru_cache(maxsize=None)
def fibonacci(n):
    if n < 2:
        return n
    return fibonacci(n-1) + fibonacci(n-2)

print(fibonacci(10))  # 55

# Decoradores para métodos de clase y estáticos
class Matematica:
    @staticmethod
    def suma(a, b):
        return a + b

    @classmethod
    def valor_pi(cls):
        return 3.1416

print(Matematica.suma(10, 5))  # 15
print(Matematica.valor_pi())   # 3.1416

# Contextlib para simplificar manejo de contexto
from contextlib import closing
import sqlite3

with closing(sqlite3.connect('mi_base_de_datos.db')) as conexion:
    with closing(conexion.cursor()) as cursor:
        cursor.execute('CREATE TABLE IF NOT EXISTS tabla (id INTEGER PRIMARY KEY, nombre TEXT)')
        cursor.execute('INSERT INTO tabla (nombre) VALUES (?)', ('Alice',))
        conexion.commit()

# Uso de propiedades con setter y getter
class Persona:
    def __init__(self, nombre):
        self._nombre = nombre

    @property
    def nombre(self):
        return self._nombre

    @nombre.setter
    def nombre(self, valor):
        if not valor:
            raise ValueError("El nombre no puede estar vacío")
        self._nombre = valor

persona = Persona("Alice")
print(persona.nombre)  # Alice
persona.nombre = "Bob"
print(persona.nombre)  # Bob


# Métodos mágicos (Dunder methods) adicionales
class Vector:
    def __init__(self, x, y):
        self.x = x
        self.y = y

    def __repr__(self):
        return f"Vector({self.x}, {self.y})"

    def __eq__(self, otro):
        return self.x == otro.x and self.y == otro.y

    def __lt__(self, otro):
        return (self.x ** 2 + self.y ** 2) < (otro.x ** 2 + otro.y ** 2)

    def __add__(self, otro):
        return Vector(self.x + otro.x, self.y + otro.y)

v1 = Vector(2, 3)
v2 = Vector(2, 3)
v3 = Vector(1, 1)
print(v1)             # Vector(2, 3)
print(v1 == v2)       # True
print(v1 < v3)        # False
print(v1 + v3)        # Vector(3, 4)

# Funciones de orden superior
def aplicar_funcion(funcion, valor):
    return funcion(valor)

print(aplicar_funcion(lambda x: x * 2, 5))  # 10

# Iteradores personalizados
class Contador:
    def __init__(self, inicio, fin):
        self.inicio = inicio
        self.fin = fin

    def __iter__(self):
        self.actual = self.inicio
        return self

    def __next__(self):
        if self.actual > self.fin:
            raise StopIteration
        else:
            self.actual += 1
            return self.actual - 1

contador = Contador(1, 5)
for numero in contador:
    print(numero)  # 1, 2, 3, 4, 5

# Decoradores anidados
def decorador1(func):
    def nueva_funcion(*args, **kwargs):
        print("Ejecutando decorador 1")
        return func(*args, **kwargs)
    return nueva_funcion

def decorador2(func):
    def nueva_funcion(*args, **kwargs):
        print("Ejecutando decorador 2")
        return func(*args, **kwargs)
    return nueva_funcion

@decorador1
@decorador2
def mi_funcion():
    print("Función original")

mi_funcion()
# Ejecutando decorador 1
# Ejecutando decorador 2
# Función original

# Variables de clase vs instancia
class Ejemplo:
    variable_clase = "Variable de clase"

    def __init__(self, variable_instancia):
        self.variable_instancia = variable_instancia

obj1 = Ejemplo("Instancia 1")
obj2 = Ejemplo("Instancia 2")

print(obj1.variable_clase)      # Variable de clase
print(obj1.variable_instancia)  # Instancia 1
print(obj2.variable_clase)      # Variable de clase
print(obj2.variable_instancia)  # Instancia 2

Ejemplo.variable_clase = "Nueva variable de clase"
print(obj1.variable_clase)      # Nueva variable de clase
print(obj2.variable_clase)      # Nueva variable de clase

# Metaclases
class Meta(type):
    def __new__(cls, nombre, bases, diccionario):
        diccionario['atributo_nuevo'] = 'Valor añadido por la metaclase'
        return super().__new__(cls, nombre, bases, diccionario)

class MiClase(metaclass=Meta):
    pass

obj = MiClase()
print(obj.atributo_nuevo)  # Valor añadido por la metaclase

# Context managers personalizados con __enter__ y __exit__
class GestorRecursos:
    def __enter__(self):
        print("Recursos adquiridos")
        return self

    def __exit__(self, tipo, valor, traceback):
        print("Recursos liberados")

with GestorRecursos():
    print("Dentro del contexto")

# Atributos y métodos dinámicos
class Dinamico:
    pass

dinamico = Dinamico()
dinamico.atributo = "Valor dinámico"
print(dinamico.atributo)  # Valor dinámico

def metodo_dinamico(self):
    return "Método dinámico"

from types import MethodType
dinamico.metodo = MethodType(metodo_dinamico, dinamico)
print(dinamico.metodo())  # Método dinámico

# NamedTuple avanzado
from collections import namedtuple

Persona = namedtuple('Persona', 'nombre edad')
persona = Persona(nombre="Alice", edad=30)
print(persona.nombre)  # Alice
print(persona.edad)    # 30

# NamedTuple con valores por defecto
PersonaConDefault = namedtuple('PersonaConDefault', 'nombre edad')
PersonaConDefault.__new__.__defaults__ = ("Desconocido", 0)
persona_default = PersonaConDefault()
print(persona_default.nombre)  # Desconocido
print(persona_default.edad)    # 0

# Uso avanzado de defaultdict
def default_valor():
    return "Valor por defecto"

dd = defaultdict(default_valor)
print(dd["clave_inexistente"])  # Valor por defecto

# Manejo avanzado de fechas con datetime
from datetime import datetime, timedelta

# Crear una fecha
fecha = datetime(2024, 1, 1)
print(fecha)  # 2024-01-01 00:00:00

# Sumar días a una fecha
nueva_fecha = fecha + timedelta(days=10)
print(nueva_fecha)  # 2024-01-11 00:00:00

# Formatear fechas
formateada = fecha.strftime("%d/%m/%Y")
print(formateada)  # 01/01/2024

# Parsear fechas desde cadenas
cadena_fecha = "12-06-2024"
fecha_parseada = datetime.strptime(cadena_fecha, "%d-%m-%Y")
print(fecha_parseada)  # 2024-06-12 00:00:00

# Ejemplo avanzado con itertools (chain, islice, cycle)
import itertools

# chain para concatenar iterables
cadena = itertools.chain("ABC", "DEF")
print(list(cadena))  # ['A', 'B', 'C', 'D', 'E', 'F']

# islice para rebanar iterables
rebanada = itertools.islice(range(10), 2, 8)
print(list(rebanada))  # [2, 3, 4, 5, 6, 7]

# cycle para ciclar sobre un iterable
ciclo = itertools.cycle([1, 2, 3])
for i in range(6):
    print(next(ciclo))  # 1, 2, 3, 1, 2, 3

# Creación de iteradores personalizados
class MiIterador:
    def __init__(self, valor):
        self.valor = valor

    def __iter__(self):
        return self

    def __next__(self):
        if self.valor <= 0:
            raise StopIteration
        self.valor -= 1
        return self.valor

mi_iterador = MiIterador(5)
for valor in mi_iterador:
    print(valor)  # 4, 3, 2, 1, 0

# Uso avanzado de lru_cache con parámetros
@lru_cache(maxsize=32)
def factorial(n):
    if n < 2:
        return 1
    return n * factorial(n - 1)

print([factorial(n) for n in range(10)])  # [1, 1, 2, 6, 24, 120, 720, 5040, 40320, 362880]

# Variables de entorno con os
import os

# Establecer una variable de entorno
os.environ['MI_VARIABLE'] = 'valor'

# Leer una variable de entorno
print(os.getenv('MI_VARIABLE'))  # valor

# Itertools para permutaciones y combinaciones
import itertools

# Permutaciones
permutaciones = list(itertools.permutations([1, 2, 3]))
print(permutaciones)  # [(1, 2, 3), (1, 3, 2), (2, 1, 3), (2, 3, 1), (3, 1, 2), (3, 2, 1)]

# Combinaciones
combinaciones = list(itertools.combinations([1, 2, 3], 2))
print(combinaciones)  # [(1, 2), (1, 3), (2, 3)]

# Itertools para productos cartesianos
producto = list(itertools.product([1, 2], ['a', 'b']))
print(producto)  # [(1, 'a'), (1, 'b'), (2, 'a'), (2, 'b')]

# Multiprocessing para paralelismo
import multiprocessing

def tarea(n):
    print(f"Procesando {n}")

if __name__ == '__main__':
    with multiprocessing.Pool(4) as p:
        p.map(tarea, range(5))

# Threading para hilos
import threading

def imprimir_mensaje():
    print("Hilo en ejecución")

hilo = threading.Thread(target=imprimir_mensaje)
hilo.start()
hilo




```
