# Reto-IX
## Funciones Recursivas

### Funciones de retos anteriores pasadas a lambda
#### - Funcion 4 Reto # 6
```python
if __name__ == "__main__":
    p = int(input("panes: "))
    m = int(input("bolsas: "))
    h = int(input("huevos: "))
    b = int(input("valor billete: "))
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
