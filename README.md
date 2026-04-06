# EVALUACIÓN MÓDULO 1 - DATA ANALYTICS

A continuación explicaré brevemente el cómo se realiza el proyecto.

## Ejercicio 1 - Agregar productos a un inventario

Hay que crear una función para agregar productos a un inventario de manera que si el nombre del producto a agregar coincide con un producto que ya está en el inventario, solo actualiza la cantidad. Si no coincide, se hace una actualización del inventario. 

```bash
def agregar_producto(nombre, precio, cantidad): 
    for producto in inventario:
        if producto ["nombre"] == nombre:
            producto ["cantidad"] = producto["cantidad"]+cantidad   
            return
    inventario.append({"nombre": nombre, 
                        "precio": precio, 
                        "cantidad": cantidad})
```

## Ejercicio 2 - Ver inventario

En el segundo ejercicio nos piden ver el inventario. Hay que imprimir el inventario poniendo el símbolo de $ al lado del precio. Para eso basta con escribir el siguiente código.  

```bash
def ver_inventario(inventario):
    for producto in inventario:
        print("Nombre:",producto["nombre"],", Precio:$",producto["precio"],", Cantidad",producto["cantidad"])
    return
```
## Ejercicio 3 - Buscar producto

Para buscar el producto según el nombre del producto hay que escribir una función que recorra el inventario (bucle for) y ver si los nombres coinciden. En caso de que no lo hagan, hay que imprimir "producto no encontrado".

```bash
def buscar_producto(nombre):
    for producto in inventario:
        if producto ["nombre"] == nombre:
            print(producto)           
            return
    print("Producto no encontrado")
    return
```
## Ejercicio 4 - Actualizar stock

Para actualizar stock hay que utilizar el .update(cantidad) en caso de que nos nombre del producto coincida con el producto del inventario. 

```bash
def actualizar_stock(nombre, cantidad):
    for producto in inventario:
        if producto["nombre"] == nombre:
            producto.update({"cantidad":cantidad})
            return    
    print("no hay suficiente stock")
```

## Ejercicio 5 - Eliminar un producto

Similar al ejercicio 4 pero con la diferencia de que aquí se elimina el producto con .remove(producto). 

```bash
def eliminar_producto_nombre(nombre):
    for producto in inventario:
        if producto["nombre"] == nombre.lower():
           inventario.remove(producto)
           return
    print("El producto no está en el inventaro")
```

## Ejercicio 6 - Calcular el valor del inventario

Para calcular el valor del inventario hay que crear una variable con valor 0 de manera que cada vez que se itere el inventario se vaya añadiendo (sumando) el valor del producto al valor que ya previamente hemos sumado.
 

```bash
def eliminar_producto_nombre(nombre):
    for producto in inventario:
        if producto["nombre"] == nombre.lower():
           inventario.remove(producto)
           return
    print("El producto no está en el inventaro")
```

## Ejercicio 7 - Realizar la compra

Este ejercicio es una combinación de todos los ejercicios hasta ahora. Sin embargo, en este ejercicio es importante usar el bucle while porque la lógica es pensar que se seguirá comprando hasta que el cliente diga parar. 

Para ello, se crea una condición: seguir comprando = True

Los pasos que se deben seguir son los siguientes:
 


```python

# mostrar inventario al cliente: productos, precios y cantidades

# preguntar qué quiere comprar: el cliente escribe nombre del producto

# comprobar si existe. Ese producto está en el inventario?

# pedir cantidad. Preguntar al cliente cuántos quiere comprar

# añadir al carrito: se guarda lo que se ha comprado

# actualizar el inventario

# preguntar si quiere seguir comprando

# calcular total

# mostrar resultado final



```
