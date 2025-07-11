# Reto-10
Reto número 10. PDC

### Primer punto
- Desarrolle un programa que permita realizar la suma/resta de matrices. El programa debe validar las condiciones necesarias para ejecutar la operación.
```pseudocode
  def sumar_matrices(matriz_1_operable : list, matriz_2_operable : list, matriz_1 : list, matriz_2 : list) ->list:
	resultado_suma = []
	for i in range(len(matriz_1_operable)):
		for j in range(len(matriz_1[i])):
			resultado_suma.append(matriz_1_operable[i] + matriz_2_operable[i])
	return resultado_suma

def restar_matrices(matriz_1_operable : list, matriz_2_operable : list, matriz_1 : list, matriz_2 : list) ->list:
	resultado_resta = []
	for i in range(len(matriz_1_operable)):
		for j in range(len(matriz_1[i])):
			resultado_resta.append(matriz_1_operable[i] - matriz_2_operable[i])
	return resultado_resta

if __name__ == "__main__":
	print("Ingrese dos matrices de la misma magnitud, el programa le retornara la suma, la resta o ambas.ingrese los valores de las matrices separados por espacios")
	matriz_1 = input("Ingrese la primera matriz: ").split(" ")
	matriz_1_operable = [int(x) for x in matriz_1]
	matriz_2 = input("Ingrese la segunda matriz: ").split(" ")
	matriz_2_operable = [int(x) for x in matriz_2]
	if len(matriz_1) != len(matriz_2):
		print("La magnitud de las matrices son distintas, la cantidad de elementos de la primera matriz : " + str(len(matriz_1_operable)) + " , es diferente que la cantidad de elementos de la segunda matriz :  " + str(len(matriz_2_operable)))

	resultado_de_la_suma = sumar_matrices(matriz_1_operable, matriz_2_operable, matriz_1, matriz_2)
	resultado_de_la_resta = restar_matrices(matriz_1_operable, matriz_2_operable, matriz_1, matriz_2)
	
	if len(matriz_1) == len(matriz_2):
		resultado_de_la_suma = sumar_matrices(matriz_1_operable, matriz_2_operable, matriz_1, matriz_2)
		resultado_de_la_resta = restar_matrices(matriz_1_operable, matriz_2_operable, matriz_1, matriz_2)
		x : int
		x = int(input("¿ Qué operación desea realizar?, suma(1), resta(2), ambas(3): "))
		if x == 1:
			print("El resultado de sumar " + str(matriz_1_operable) + " con " + str(matriz_2_operable) + " es " + str(resultado_de_la_suma))
		if x == 2:
			print("El resultado de restar " + str(matriz_1_operable) + " con " + str(matriz_2_operable) + " es " + str(resultado_de_la_resta))
		if x == 3:
			print("El resultado de sumar " + str(matriz_1_operable) + " con " + str(matriz_2_operable) + " es " + str(resultado_de_la_suma) + "  y el resultado de restar " + str(matriz_1_operable) + " con " + str(matriz_2_operable) + " es " + str(resultado_de_la_resta))
	
```

### Segundo punto
- Desarrolle un programa que permita realizar el producto de matrices. El programa debe validar las condiciones necesarias para ejecutar la operación.
```pseudocode
```

### Tercer punto
- Desarrolle un programa que permita obtener la matriz transpuesta de una matriz ingresada. El programa debe validar las condiciones necesarias para ejecutar la operación.
```pseudocode
```

### Cuarto punto
- Desarrollar un programa que sume los elementos de una columna dada de una matriz.
```pseudocode
```

### Quinto punto
- Desarrollar un programa que sume los elementos de una fila dada de una matriz.
```pseudocode
```




