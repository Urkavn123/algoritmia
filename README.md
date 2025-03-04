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
    leer numero
    leer total_positivos
    leer total_negativos
    total_positivos <- 0 
    total_negativos <- 0
    numero <- -6
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
    leer x
    leer y
    leer z
    x <- 8
    y <- 4
    z <- 5
    si x > y Y z < 20 entonces
       mostrar "ingresar un valor para p"
       si_no
       leer p
    fin_si
fin
    
