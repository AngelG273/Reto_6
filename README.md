# Reto_6

### Ejercicio 1:

La solucion del punto "Imprimir un listado con los números del 1 al 100 cada uno con su respectivo cuadrado" es :
- Diagrama de flujo:
  
``` mermaid
flowchart TD
    A[Inicio] --> C(Mientras i sea menor que 100)
    A --> B(i = 0 para poder evaluar el numero)
    C -->D(Se debe sumar 1)
    B -->D
    D --> E(Imprimir el numero)
    D --> F(Imprimir su cuadrado)
```
- Codigo:
``` python
i : int = 0 
# Se evaluan los i hasta 100
while(i < 100): 
  # se la suma 1 para evaluar digito por digito
  i += 1 
  # Se imprime cada i y su cuadrado
  print(i, i**2)
```

### Ejercicio 2:

La solución del segundo puto " Imprimir un listado con los números impares desde 1 hasta 999 y seguidamente otro listado con los números pares desde 2 hasta 1000 " es:
- Diagrama de flujo:
``` mermaid
flowchart TD
    A[Inicio] --> C(Los i menores a 999)
    C --> B(Evaluar los i cuando es igual a -1)
    B --> D(Se realiza i+=2)
    D --> E(Imprimir i)
    A --> F(Los i menores a 1000)
    F --> G(Evaluar los i cuando es igual a 0)
    G --> H(Se realiza i+=2)
    H --> J(Imprimir i)
```
- Codigo:
```Python
print("Numeros impares")
# Numeros impares hasta el 999
i : int= -1
while i < 999:
  i+=2  # Al sumarle 2 a valor que toma i apartir de -1 este se vuelve impar
  print (i)

print("Numeros pares")
# Numeros pares hasta el 1000
i : int= 0
while i < 999:
  i+=2  # Al sumarle 2 a cada valor que toma i apartir de 0 este se vuelve par
  print (i)
```

### Ejercicio 3:

La solución del segundo puto " Imprimir los números pares en forma descendente hasta 2 que son menores o iguales a un número natural n ≥ 2 dado " es:
- Diagrama de flujo:
``` mermaid
flowchart TD
    A[Inicio] --> C(Ingresar un numero n)
    C --> B(Evaluar si n es mayor o igual a 2)
    B --> D(Se da el rango n,1,-1 )
    D --> E(Se evaluan los i donde el % 2 ==0 )
    E --> F(Se imprimen los i)
```
- Codigo:
``` python
#Se evalua que el numero ingresado sea mayor o igual a 2
while n:   
  n = int ( input ("Ingrese un numero mayor a 2:"))
  if n >= 2:
    break
  else:
    print (int(input("Ingrese un numero mayor a 2:")))

# Se evalua que el numero sea par
for i in range(n,1,-1):
  if i % 2 == 0:
    # Se imprime el numero par
    print (i)
```

El resto de los puntos se encuentran en el archivo adjunto.
