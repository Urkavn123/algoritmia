Actividades del libro de Fundamentos de programacion 4ta Edición Luis Joyanes Aguilar
4.1 
a)
Algoritmo Angulo_90_grados
var
    Entero: angulo
inicio
    leer angulo
    angulo <- 70
    si angulo == 90 entonces
       mostrar "El ángulo es un ángulo recto"
    si_no
        mostrar "El ángulo no es un ángulo recto"
    fin_si 
fin    
![image](https://github.com/user-attachments/assets/7fba8913-d78d-433e-a3f8-e48427f16524)
B)
Algoritmo temperatura_superior_100_grados
var
    Entero: temperatura
inicio
     leer temperatura
     temperatura <- 90
     si temperatura == 100 entonce
         mostrar "por encima del punto de ebullición del agua"
     si_no 
         mostrar "por debajo del punto de ebullición del agua"
     fin_si
fin
![Captura de pantalla 2025-03-04 180351](https://github.com/user-attachments/assets/17da2aec-6d25-455e-ac7c-2632c81cf8fb)
C)
Algoritmo  el_número_es_positivo 
var 
    entero: total_positivos
    entero: total_negativos
    entero: numero
inicio
    total_positivos <- 0 
    total_negativos <- 0
    numero <- 3
    leer numero  
    
    si numero > 0 Entonces 
        total_positivos <- total_positivos + numero
    sino
        total_negativos <- total_negativos + numero
    fin_si
fin 
![Captura de pantalla 2025-03-04 175333](https://github.com/user-attachments/assets/dd6df818-416c-4c4e-809a-5b52050e0017)
d)
algoritmo leer_un_valor_para_p
var
    entero: x
    entero: y
    entero: z
    entero: p
inicio
    mostrar "ingrese el valor para x:"
    mostrar "ingrese el valor para y:"
    mostrar "ingrese el valor para z:"
    leer x
    leer y
    leer z
    si x > y Y z < 20 entonces
       mostr_ar "ingresar un valor para p"
    fin_si
![image](https://github.com/user-attachments/assets/8796869c-0217-4b20-a43e-f54d17829791)
e)
algoritmo leer_valor_para_tiempo
var 
    real: tiempo
    real: distancia
inicio
    mostrar "ingrese la distancia:"
    leer distancia
    si distancia > 20 y distancia < 35 entonces
       mostrar "ingrese un valor para tiempo:"
    si_no 
       mostrar "la distancia no esta en el rango permitido"
    fin_si
fin
![image](https://github.com/user-attachments/assets/f7b85e17-83f5-429d-82be-f1787a415ad4)
4.2
algoritmo programa
 Entero: num1
 Entero: num2
inicio
    mostrar "Ingrese el primer número: "
    leer num1
    mostrar "Ingrese el segundo número: "
    leer num2
    si num1 > num2 entonces
        mostrar "El primer número es el mayor."
    si_no
        si num1 < num2 entonces
            mostrar "El primer número es el más pequeño."
        si_no
            mostrar "Ambos números son iguales.
    fin_si
fin
4.3
algoritmo numero_central
entero: num1
entero: num2
entero: num3
entero: central
inicio
    mostrar "ingrese el primer número: "
    leer num1
    mostrar "ingrese el segundo número: "
    leer num2
    mostrar "ingrese el tercer número: "
    leer num3
    si (num1 > num2 y num1 < num3) o (num1 > num3 y num1 < num2) entonces
        central <- num1
    si_no
        si (num2 > num1 y num2 < num3) o (num2 > num3 y num2 < num1) entonces
            central <- num2
        si_no
            central <- num3
        fin si
fin
4.4
algoritmo raiz_cuadrada
real: numero
real: raiz
inicio
    mostrar "ingrese un numero"
    leer numero
    si numero >= 0 entonces
       raiz <- raiz_cuadrada(numero)
       mostrar "la raiz cuadrada es:" , raiz
    si_no
       mostrar "no se puede calcular la raiz cuadrada de un numero negativo"
    fin_si
fin
4.5
algoritmo par
entero num
inicio
    mostrar "ingrese un numero: " 
    leer num
    si num mod 2 == 0 entonces
       mostrar "el numero es par"
    si_no 
       mostrar "el numero no es par"
    fin_si
fin
4.6
algoritmo fecha 
entero:dia
entero: mes 
entero: año
inicio 
    mostrar "ingrese el dia: "
    leer dia
    mostrar "ingrese el mes: "
    leer mes 
    mostrar "ingrese el año: "
    si (mes == 1 o mes  == 3 o mes == 5 o mes == 7 o mes == 8 o mes == 10) y dia == 31 entonces
       dia <- 1
       mes <- mes + 1
    si_no 
       si (mes == 4 o mes == 6 o mes == 9 o mes == 11) y dia == 30 entonces 
          dia <- 1
          mes <- mes + 1
       si_no
          si mes == 2 entonces
             si (año mod 4 == 0 y año mod 100 ≠ 0) o (año mod 400 = 0) entonces 
                si dia == 29 y mes == 2 entonces
                   dia <- 1 
                   mes <- 3
                si_no 
                   dia <- dia + 1
                   fi_si
                fin_si
            si_no
                si mes == 12 y dia == 31 entonces
                   dia <- 1
                   mes <- 1 
                   año <- año + 1 
                si_no
                   dia <- dia + 1
                fin_si
            fin_si
        fin_si
    fin_si
    mostrar "la fecha del dua siguiente es: ", dia, "/", mes "/", "/" año
fin
4.7 
algoritmo peso_de_alumnos
enteros i
enteros n
inicio
    menos_40 <- 0
    entre_40_50 <- 0
    entre_50_60 <- 0
    mas_60 = 0
    mostrar "Ingrese la cantidad de alumnos:"
    para i = 1 hasta n hacer
        mostrar  "Ingrese el peso del alumno ", i, ":"
        leer peso
        
        si peso < 40 entonces
            menos_40 <- menos_40 + 1
        si_no
            si peso >= 40 y peso <= 50 entonces
                entre_40_50 <- entre_40_50 + 1
            si_no
                si peso > 50 y peso < 60 entonces
                    entre_50_60 <- entre_50_60 + 1
                si_no
                    mas_60 = mas_60 + 1
                fin si
            fin si
        fin si
    fin para
    mostrar "Estadística de pesos:"
    mostrar "Alumnos de menos de 40 kg: ", menos_40
    mostrar "Alumnos entre 40 y 50 kg: ", entre_40_50
    mostrar "Alumnos de más de 50 kg y menos de 60 kg: ", entre_50_60
    mostrar "Alumnos de más o igual a 60 kg: ", mas_60
fin
4.8
algoritmo numero_divisible
entero num1
entero num2
inicio
    mostrar "Ingrese el primer número:"
    leer num1
    mostrar "Ingrese el segundo número:"
    leer num2
    si num1 mod num2 == 0 entonces
        mostrar num2, " es divisor de ", num1
    si_no
        si num2 mod num1 == 0 entonces
            mostrar num1, " es divisor de ", num2
        si_no
            mostrar "Ninguno de los números es divisor del otro."
        fin si
    fin si
fin
4.9
algoritmo angulo_obtuso_y_agudo
entero angulo
inicio
    mostrar "Ingrese el valor del ángulo en grados:"
    leer angulo
    si angulo < 90 entonces
        escribir "El ángulo es agudo."
    si_no
        si angulo == 90 entonces
            escribir "El ángulo es recto."
        si_no
            escribir "El ángulo es obtuso."
        fin si
    fin si
fin
4.10
algoritmo calificacion
entero calificacion
inicio  
    mostrar "Ingrese la calificación numérica (0-100):"
    leer calificacion
    si calificacion >= 90 entonces
        mostrar "La calificación en letra es: A"
    si_no
        si calificacion >= 80 entonces
            mostrar "La calificación en letra es: B"
        si_no
            si calificacion >= 70 entonces
                mostrar "La calificación en letra es: C"
            si_no
                si calificacion >= 69 entonces
                    mostrar "La calificación en letra es: D"
                si_no
                    mostrar "La calificación en letra es: F"
                fin si
            fin si
        fin si
    fin si
fin
