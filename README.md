# Reto-IX
## Funciones Recursivas

### Funciones de retos anteriores pasadas a lambda
#### - Funcion 4 Reto # 6
```python
if __name__ == "__main__":
    # variables
    p = int(input("panes: "))
    m = int(input("bolsas: "))
    h = int(input("huevos: "))
    b = int(input("valor billete: "))
    # Funcion
    vc= ((300 * p) + (3300 * m) + (350 * h))
    c = (lambda x, y: x - y)(b,vc)
    print(f"al comprar {p} huevos, {m} bolsas y {h} huevos, me queda {c}")
```
#### - Funcion 3 Reto #6
```python
if __name__ == "__main__":
    n = int(input("gallinas: "))
    m = int(input("gallos: "))
    k = int(input("pollos: "))
    kg = (lambda x, y, z: 6*x + 7*y + z )(n,m,k)
    print(f"entre {n} gallinas, {m} gallos y {k} pollos, hay {kg} kg de carne")
```
#### - Funcion 8 Reto #8
```python
import math
if __name__ == "__main__":    
 n = int(input("Último término: "))
 x = int(input("Exponente: "))
 a = 0
for i in range(n):
        t = x**i / math.factorial(i)
        a += t
maclaurin = (lambda x: x)(a)
print(f"McL {a}")
print(math.e**x)
```
### Funciones de retos anteriores con argumentos no definidos
#### Funcion 7.1 Reto 6
```python
def promedio(*args) -> float:
    promx: float = 0
    for num in args:
        promx += num
    return promx / len(args)

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
def promul(*args)-> float:
    mulp: float = 1
    for num in args:
        mulp *= num
    return mulp**(1/len(args))

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
def m_e_n(*args) -> float:
    minx = min(args)
    maxx = max(args)
    return maxx ** minx

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

if __name__ == "__main__":
 n = int(input("Base: "))
 m = int(input("Exponente: "))
 r = pot(n, m)
 print(f"{n} elevado a {m} es igual a {r}")
```

### FIbonacci
```python
import time
n = int(input("Ingrese numero: "))
i : int = 1
n1 : int = 0
n2 : int = 1

def fiboI(n : int )-> int:
  return Sfib

start_time_fiboI = time.time()
for i in range(n-1):
    Sfib = n1 + n2
    n1 = n2
    n2 = Sfib
end_time_fiboI = time.time()
timer = end_time_fiboI - start_time_fiboI
print(n, timer) 
 #Empieza a tardar mas de 1 segundo a partir de n = +300.000
```

### StackOverFlow
![](https://github.com/DKev2P24/Reto-IX/blob/main/Captura%20de%20pantalla%20(43).png)

### Linkedin
https://www.linkedin.com/in/kevin-daniel-castellanos-pe%C3%B1a-b98171305/ 

