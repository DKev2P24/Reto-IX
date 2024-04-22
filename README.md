# Reto-IX
## Funciones Recursivas

### Funciones de retos anteriores pasadas a lambda
#### - Funcion 4 Reto # 6
```python
if __name__ == "__main__":
    # cantidades
    p = int(input("panes: "))
    m = int(input("bolsas: "))
    h = int(input("huevos: "))
    b = int(input("valor billete: "))
    # Funcion del valor total
    vc= ((300 * p) + (3300 * m) + (350 * h))
    # cambio de la compra
    c = (lambda x, y: x - y)(b,vc)
    # impresion del resultado
    print(f"al comprar {p} huevos, {m} bolsas y {h} huevos, me queda {c}")
```
#### - Funcion 3 Reto #6
```python
if __name__ == "__main__":
   # cantidades
    n = int(input("gallinas: "))
    m = int(input("gallos: "))
    k = int(input("pollos: "))
   # peso total
    kg = (lambda x, y, z: 6*x + 7*y + z )(n,m,k)
   # resultado
    print(f"entre {n} gallinas, {m} gallos y {k} pollos, hay {kg} kg de carne")
```
#### - Funcion 8 Reto #8
```python
import math  # importa el modulo
if __name__ == "__main__":
# variables
 n = int(input("Último término: "))
 x = int(input("Exponente: "))
 a = 0
 # Bucle 
for i in range(n):
        t = x**i / math.factorial(i)
        a += t
maclaurin = (lambda x: x)(a) # aignar valor a la variable
print(f"McL {a}") # imprime aproximacion
print(math.e**x) # imprime valor "e**x"
```
### Funciones de retos anteriores con argumentos no definidos
#### Funcion 7.1 Reto 6
```python
def promedio(*args) -> float: # Funcion con argumentos variables
    promx: float = 0 # almacena valores
    for num in args:
        promx += num
    return promx / len(args) # se realiza la suma de valores y se divide entre la cantidad de valores

# variables
if __name__ == "__main__":
    a = float(input("Ingrese número a: "))
    b = float(input("Ingrese número b: "))
    c = float(input("Ingrese número c: "))
    d = float(input("Ingrese número d: "))
    e = float(input("Ingrese número e: "))
    resultado = promedio(a, b, c, d, e)
    print(f"El promedio es: {resultado}")
```
#### Funcion 7.3 Reto 6
```python
def promul(*args)-> float: # Funcion con argumentos variables
    mulp: float = 1 # almacena valores
    for num in args:   
        mulp *= num
    return mulp**(1/len(args)) # se realiza el calculo del produto de los valores, y saca la raiz n-sima de ese valor, dependiendo la cantidad de valores

# Valores
if __name__ == "__main__":
    a = float(input("Ingrese a: "))
    b = float(input("Ingrese b: "))
    c = float(input("Ingrese c: "))
    d = float(input("Ingrese d: "))
    e = float(input("Ingrese e: "))
    resultado = promul(a, b, c, d, e)
    print(f"El promedio multiplicativo es: {resultado}")
```
#### Funcion 7.6
```python
def m_e_n(*args) -> float: # funcion con argumentos variables
    minx = min(args)
    maxx = max(args)
    return maxx ** minx # se eleva el mayor numero a la n potencia, siendo n el menor valor 

# variables
if __name__ == "__main__":
    a = float(input("Ingrese a: "))
    b = float(input("Ingrese b: "))
    c = float(input("Ingrese c: "))
    d = float(input("Ingrese d: "))
    e = float(input("Ingrese e: "))
    r = m_e_n(a, b, c, d, e)
    print(f"El resultado es: {r}")
```
### Potencia Recursiva
```python
def pot(n: int, m: int) -> int:
    # Caso base
    if m == 0:
        return 1 # Cualquier numero elevado a 0 es igual a 1
    else:
        return n * pot(n, m - 1) # Condicion Recursiva
# variables
if __name__ == "__main__":
 n = int(input("Base: "))
 m = int(input("Exponente: "))
 r = pot(n, m)
 print(f"{n} elevado a {m} es igual a {r}")
```

### FIbonacci
```python
import time # se importa el modulo .time
n = int(input("Ingrese numero: "))
i : int = 1 
n1 : int = 0
n2 : int = 1  # se inician los valores en los inscritos 

def fiboI(n : int )-> int:
  return Sfib # funcion

start_time_fiboI = time.time() # inicia el tiempo
for i in range(n-1): #bucle definido entre 1 a n-1
    Sfib = n1 + n2
    n1 = n2
    n2 = Sfib
end_time_fiboI = time.time() # finaliza el contador al entregar el valor
timer = end_time_fiboI - start_time_fiboI # se deduce la duracion del rendimiento
print(n, sfib, timer) # se imprime el numero inicial, su valor en la funcion y el tiempo realizado
 #Empieza a tardar mas de 1 segundo a partir de n = +300.000
```

### StackOverFlow
![](https://github.com/DKev2P24/Reto-IX/blob/main/Captura%20de%20pantalla%20(43).png)

### Linkedin
https://www.linkedin.com/in/kevin-daniel-castellanos-pe%C3%B1a-b98171305/ 

