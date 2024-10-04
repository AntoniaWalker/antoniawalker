# Problema 1 
En un rango de 1 a 101 se pueden observar todos los números que contiene este tramo, a excepción de el último, por lo que se recorre del 1 al 100. Esto se codifica: for x in range(1, 101). Luego, pido que se “impriman” los números que contiene el rango: print(x). De esta forma, puedo generar el listado desde el número 1 al 100. 

# Problema 2 
En un rango de 1 a 100 se pueden observar todos los números que contiene este tramo y que son divisibles por tres. En este caso, no se incluye el 101, ya que, el 99 es el último número divisible por tres. Esto se codifica: for i in range(1, 100). Posteriormente, incluyo la fórmula que dividirá los números del rango. En % se ocupa como división y el == como igual a 0. Al ser igual a 0, damos a entender que desde el 3 se parte a contar los números del rango. Se codifica como: if i % 3 == 0. 
Luego, pido que se “impriman” los números que contiene el rango: print(i). De esta forma, puedo generar el listado desde el número 3 al 99.  

# Problema 3 
Entendemos la suma como a+b, y para que las personas puedan ingresar los números se pone el “input”, y luego la frase que queramos. De esta forma, la primera parte de la codificación queda a=float(input(“ingresa el primer número: ”)). Luego se repite lo mismo con b, y aludiendo al segundo número. Como el resultado debe ser categorizado en mayor a 100, menor a 100 o mayor a 150, se configura el código de manera que pueda leer el resultado e indicar en qué categoría encaja. Por ello, la primera categoría se codifica:
if suma < 100:
    print("menor a 100")
En el caso de la segunda, ponemos:
elif 100 <= suma < 150:
    print("mayor a 100")
Y para números más grandes a 150, le damos la instrucción: 
else:
    print("mayor a 150"). 
Por último, el programa es capaz de arrojar el resultado categorizado, según los números que haya ingresado el usuario. 

# Problema 4
El input es para pedir respuestas al usuario, por ello, en este caso, le pedimos que nos responda si es mayor de edad o no. Antes, eso si, ordenamos al programa que comience una evaluación del usuario, cosa de poder entregarle las respuestas que busca: def evaluar_usuario (). 
Tras esto, le pedimos que nos diga su edad, para poder entregarle la respuesta más adecuada: edad = int(input("¿Cuántos años tienes? ")). 
Ya tenemos la mitad de la categorización del usuario lista, por lo que ahora toca conocer su edad, entregamos la instrucción de que pregunte si le gusta la programación, haciendo una diferenciación para la respuesta si el número que entregó es menor a 18, o parte desde 18, por eso solo ocupamos un =, y no dos. Luego, entregamos las opciones para responder: 
le_gusta_programar = input("¿Te gusta la programación? (sí/no): ").strip().lower()
    if edad >= 18:
        if le_gusta_programar == "sí":
            print("¡Eres mayor de edad y te gusta la programación! ¡Sigue recorriendo el fascinante camino de la informática!.")
        elif le_gusta_programar == "no":
            print("Eres mayor de edad y no te gusta la programación.¡Corre! estás en el ramo equivocado")
        else:
            print("Respuesta no válida sobre si te gusta la programación.")
    else:
        if le_gusta_programar == "sí":
            print("¡Eres menor de edad y te gusta la programación! Sigue estudiando, ¡serás un gran computín!.")
        elif le_gusta_programar == "no":
            print("Eres menor de edad y no te gusta la programación. Explora otras áreas que puedan ser de tu interés")
        else:
            print("Respuesta no válida sobre si te gusta la programación.")
evaluar_usuario()

Dentro de los paréntesis indicamos la respuesta que buscamos entregar, de acuerdo a las alternativas que evaluamos más arriba. 




