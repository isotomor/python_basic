



# Esquema del operador ternario

El operador ternario es una forma de hacer condicionales en una sola línea.

Su esquema es
```
a if condition else b
```

y es equivalente a

```
if condition:
    a
else: 
    b
```



# List comprehension

List comprehension es una forma de crear objetos lista que ofrece una sintaxis __más corta__ cuando se quiere crear una nueva lista basada en los valores de una lista existente O un objeto iterable.

El esquema del list comprehension sería

```
[x for x in objeto_iterable]
```

Con esta forma, podemos seguir haciendo operaciones a los valores que estamos recorriendo, por ejemplo

```
[my_func(x) for x in objeto_iterable]
```
En el ejemplo de arriba llamamos a una función `my_func()` y le pasamos un valor `x` del objeto iterable, y guardamos en la lista la salida de la función `my_func()`

Ejemplos de objetos iterables = lista, un set, una tupla, un diccionario, un range()


# List comprehension con un condicional:

Si combinamos ambos conceptos, tenemos:

[a if condition else b for a in iterable ]


Un ejemplo para guardar valores en la lista que estamos creando en base a una condición

['par' if x%2 == 0 else 'impar' for x in range(10)]

Guardamos el string `par` si el numero es par, e `impar` en caso contrario.

