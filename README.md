explicacion del taller guiado
 # ejercicio 1
 1 frase = input("Escribe una frase: ")
 Esta linea pide al usuario que escriba un frase. 

La función input() detiene el programa y espera que el usuario escriba algo y presione Enter.

lo que el usuario escribe se guarda en variable frase

2 total_caracteres = len(frase)
len() es una función que cuenta cuántos caracteres hay en la cadena de texto frase.

Incluye letras, números, espacios, signos, etc.

El resultado se guarda en la variable total_caracteres.

3 espacios = frase.count(" ")
Aquí usamos el método .count(" ") para contar cuántos espacios hay dentro de la frase.

Se cuentan solo los espacios en blanco " ", no otros caracteres.

4 print(f"La frase tiene {total_caracteres} caracteres en total.")
Muestra el total de caracteres, usando una f-string (f"") para insertar el valor de total_caracteres directamente en el texto.

5 print(f"La frase tiene {espacios} espacios.")
Hace lo mismo que la línea anterior, pero muestra la cantidad de espacios encontrados.

# ejercicio 2
1 nombre = input("Escribe tu nombre completo: ")
en esat linea le pide al usuario que ingrise su nombre 
La función input() detiene el programa y espera que el usuario escriba algo y presione Enter.
2 if if nombre.replace(" ", "").isalpha():
nombre.replace(" ", "") elimina para afectar la validacion
isalpha() comprueba que todos los caracteres restantes sean letras
3 print("El nombre es válido.")
 Muestra este mensaje si el nombre solo tiene letras y comienza con mayúsculas.
4 else:
        print("El nombre debe comenzar con mayúscula.")
  si el nombre no tiene letras pero esta bien capitalizado, muestra este mensaje 
5 else:
    print("El nombre solo debe contener letras.")
  Si el nombre contiene números, símbolos u otros caracteres no válidos, muestra este mensaje.

# ejercicio 3
1 palabra = input("Escribe una palabra: ")
  pide e usuario que escriba una palabra y la gguarda en la variable palabra
2 invertida = palabra[::-1
  Usa slicing ([::-1]) para invertir el texto
 Esto significa: recorre la cadena desde el final hasta el inicio, paso -1

Ejemplo:
Si el usuario escribe "python",
palabra[::-1] será "nohtyp"

# ejercicio 4 
1 frase = input("Escribe una frase: ")
 Pide al usuario que escriba una frase y la guarda en la variable frase.
2 frase_cifrada = frase.replace("a", "*").replace("e", "*").replace("i", "*").replace("o", "*").replace("u", "*")
  renplasa  todas las vocales minúsculas por * usando el método .replace()
  Cada .replace("vocal", "*") sustituye una vocal por el asterisco
3 frase_cifrada = frase_cifrada.replace("A", "*").replace("E", "*").replace("I", "*").replace("O", "*").replace("U", "*")
  Ahora hace lo mismo con las vocales mayúsculas, reemplazándolas por 
4 p rint(f"La frase cifrada es: {frase_cifrada}")
  Muestra el resultado con las vocales cifradas en pantalla usando una f-string
  Ejemplo:
Entrada: Hola Mundo
Salida: H*l* M*nd*

# ejercicio 5 
1 frase = input("Escribe una frase: ")
Solicita al usuario que escriba una frase y la guarda en la variable frase
2 a = frase.count("a") + frase.count("A")
Cuenta cuántas veces aparece la letra "a" (tanto minúscula como mayúscula) en la frase
3 e = frase.count("e") + frase.count("E")
  i = frase.count("i") + frase.count("I")
  o = frase.count("o") + frase.count("O")
  u = frase.count("u") + frase.count("U")
4 print(f"La frase tiene {total_vocales} vocales.")
Muestra el resultado al usuario con una f-string, insertando el número total de vocales

#ejercicio 6
1 telefono = input("Escribe un número de teléfono de 10 dígitos: ")
Pide al usuario que escriba un número de teléfono y lo guarda como texto en la variable telefono
2 if len(telefono) == 10 and telefono.isdigit():
    Verifica dos cosas:
  1 Que el número tenga exactamente 10 caracteres
  2 Que todos sean dígitos (sin letras, espacios ni símbolos)

3 telefono_formateado = f"({telefono[:3]}) {telefono[3:6]}-{telefono[6:]}"
Usa slicing para dividir el número y lo formatea:

telefono[:3] → primeros 3 dígitos
telefono[3:6] → siguientes 3
telefono[6:] → últimos 4
Luego lo une en el formato (XXX) XXX-XXXX usando una f-string

# ejercicio 7 
1 palabra = input("Escribe una palabra: ").lower()
Pide al usuario que escriba una palabra
lower() convierte todo el texto a minúsculas, para que no afecte si el usuario mezcla mayúsculas
2 invertida = palabra[::-1]
Usa slicing para invertir la palabra.
[::-1] significa: recorre la cadena desde el final hasta el inicio (paso -1)
4 print("La palabra es un palíndromo.")
Si son iguales, la palabra es un palíndromo (se lee igual al derecho y al revés)
