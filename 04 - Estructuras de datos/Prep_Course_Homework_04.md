## Estructuras de Datos

1) Crear una lista que contenga nombres de ciudades del mundo que contenga más de 5 elementos e imprimir por pantalla
    lista = ['Paris', 'Ciudad de Mexico' , 'Rio de Janeiro', 'Estocolmo', 'Los Angeles']
    print (lista)
2) Imprimir por pantalla el segundo elemento de la lista
print(lista[1])
3) Imprimir por pantalla del segundo al cuarto elemento
print(lista[1:4])
4) Visualizar el tipo de dato de la lista
print(type(lista))
5) Visualizar todos los elementos de la lista a partir del tercero de manera genérica, es decir, sin explicitar la posición del último elemento
print(lista[2:])
6) Visualizar los primeros 4 elementos de la lista
print(lista[:4])
7) Agregar una ciudad más a la lista que ya exista y otra que no ¿Arroja algún tipo de error?
lista.append("Seoul")
lista.append("Paris")
8) Agregar otra ciudad, pero en la cuarta posición
 lista.insert(3, "Bogota")
9) Concatenar otra lista a la ya creada
lista.extend(["Madrid", "Barcelona", "Valencia"])
print(lista + lista2)
10) Encontrar el índice de la ciudad que en el punto 7 agregamos duplicada. ¿Se nota alguna particularidad?
lista.index("Bogota")
11) ¿Qué pasa si se busca un elemento que no existe?
lista.index("Montevideo")
12) Eliminar un elemento de la lista
lista.remove("Paris")
print(lista)
13) ¿Qué pasa si el elemento a eliminar no existe?
lista.remove("Hong Kong")
print(lista)
14) Extraer el úlimo elemento de la lista, guardarlo en una variable e imprimirlo
ultimo = lista[-1]
print(ultimo)
15) Mostrar la lista multiplicada por 4
print(lista * 4)
16) Crear una tupla que contenga los números enteros del 1 al 20
tupla1=(1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20)
print(tupla)
17) Imprimir desde el índice 10 al 15 de la tupla
print(tupla1[10:16])
18) Evaluar si los números 20 y 30 están dentro de la tupla
print(20 in tupla1)
print(30 in tupla1)
19) Con la lista creada en el punto 1, validar la existencia del elemento 'París' y si no existe, agregarlo. Utilizar una variable e informar lo sucedido.
elemento = 'Paris'
if elemento in lista:
    print( elemento + " ya estaba en la lista")
else:
    lista.append('Paris')
print(lista)
20) Mostrar la cantidad de veces que se encuentra un elemento específico dentro de la tupla y de la lista
print(tupla1.count(1))
print(lista.count('Paris'))
21) Convertir la tupla en una lista
nuevalista = list(tupla1)
print(nuevalista)
22) Desempaquetar solo los primeros 3 elementos de la tupla en 3 variables
a,b,c,_ ,_ ,_ ,_ ,_ ,_ ,_ ,_ ,_ ,_ ,_ ,_ ,_ ,_ ,_ ,_ ,_ = tupla1
print(a)
print(b)
print(c)
23) Crear un diccionario utilizando la lista crada en el punto 1, asignandole la clave "ciudad". Agregar tambien otras claves, como puede ser "Pais" y "Continente".

dicc = {"Ciudad" : lista, "Pais": ['Mexico', 'Colombia', 'Brazil', 'Colombia', 'Suecia', 'Estados Unidos', 'Corea del Sur', 'Francia'], 'Continente' : ['America', 'America', 'America', 'America', 'Europa', 'America', 'Asia', 'Europa' ] }
print(dicc)
24) Imprimir las claves del diccionario
print(dicc.keys())
25) Imprimir las ciudades a través de su clave
print(dicc['Ciudad'])