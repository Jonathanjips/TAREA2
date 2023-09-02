c++

#include <iostream>

int main() {
    int opcion;
    std::cout << "Seleccione una opción:" << std::endl;
    std::cout << "1. Patrón 1" << std::endl;
    std::cout << "2. Patrón 2" << std::endl;
    std::cout << "3. Patrón 3" << std::endl;
    std::cout << "4. Patrón 4" << std::endl;
    std::cout << "Ingrese su opción: ";
    std::cin >> opcion;

    char asterisco = '*';

    if (opcion == 1) {
        for (int i = 1; i <= 5; i++) {
            for (int j = 1; j <= i; j++) {
                std::cout << asterisco;
            }
            std::cout << std::endl;
        }
    } else if (opcion == 2) {
        for (int i = 1; i <= 5; i++) {
            for (int j = 1; j <= 5; j++) {
                if (j <= 5 - i) {
                    std::cout << ' ';
                } else {
                    std::cout << asterisco;
                }
            }
            std::cout << std::endl;
        }
    } else if (opcion == 3) {
        for (int i = 1; i <= 5; i++) {
            for (int j = 1; j <= 5; j++) {
                if (j < i) {
                    std::cout << ' ';
                } else {
                    std::cout << asterisco;
                }
            }
            std::cout << std::endl;
        }
    } else if (opcion == 4) {
        for (int i = 1; i <= 5; i++) {
            for (int j = 1; j <= 5; j++) {
                if (j <= 5 - i + 1) {
                    std::cout << asterisco;
                } else {
                    std::cout << ' ';
                }
            }
            std::cout << std::endl;
        }
    } else {
        std::cout << "Opción no válida" << std::endl;
    }

    return 0;
}


-----------------------------------------------------------------------------------------------------

Python

# Solicitar al usuario un número entero positivo
numero = int(input("Por favor, ingresa un número: "))

if numero <= 0:
    print("El número deseado.")
else:
    print("Selecciona el tipo de triángulo rectángulo que deseas ver:")
    print("1. Triángulo de lado izquierdo")
    print("2. Triángulo de lado derecho")
    print("3. Triángulo de lado superior")
    print("4. Triángulo de lado inferior")
    
    opcion = int(input("Ingresa el número de la opción que deseas: "))
    
    if opcion == 1:
        for i in range(1, numero + 1):
            for j in range(1, i + 1):
                print("*", end="")
            print()
    elif opcion == 2:
        for i in range(1, numero + 1):
            for j in range(1, numero - i + 1):
                print(" ", end="")
            for j in range(1, i + 1):
                print("*", end="")
            print()
    elif opcion == 3:
        for i in range(numero, 0, -1):
            for j in range(1, i + 1):
                print("*", end="")
            print()
    elif opcion == 4:
        for i in range(1, numero + 1):
            for j in range(1, i + 1):
                print("*", end="")
            print()
    else:
        print("Opción no válida. Por favor, selecciona una opción válida del 1 al 4.")


        ----------------------------------------------------------------------------
        seudocodigo  

        Algoritmo Main
    Definir opcion como Entero
    Escribir "Seleccione una opción:"
    Escribir "1. Patrón 1"
    Escribir "2. Patrón 2"
    Escribir "3. Patrón 3"
    Escribir "4. Patrón 4"
    Escribir "Ingrese su opción: "
    Leer opcion

    Definir asterisco como Carácter

    Si opcion == 1 Entonces
        Para i desde 1 hasta 5 con paso 1 Hacer
            Para j desde 1 hasta i con paso 1 Hacer
                Escribir asterisco
            Fin Para
            Escribir ""
        Fin Para
    Sino Si opcion == 2 Entonces
        Para i desde 1 hasta 5 con paso 1 Hacer
            Para j desde 1 hasta 5 con paso 1 Hacer
                Si j <= 5 - i Entonces
                    Escribir " "
                Sino
                    Escribir asterisco
                Fin Si
            Fin Para
            Escribir ""
        Fin Para
    Sino Si opcion == 3 Entonces
        Para i desde 1 hasta 5 con paso 1 Hacer
            Para j desde 1 hasta 5 con paso 1 Hacer
                Si j < i Entonces
                    Escribir " "
                Sino
                    Escribir asterisco
                Fin Si
            Fin Para
            Escribir ""
        Fin Para
    Sino Si opcion == 4 Entonces
        Para i desde 1 hasta 5 con paso 1 Hacer
            Para j desde 1 hasta 5 con paso 1 Hacer
                Si j <= 5 - i + 1 Entonces
                    Escribir asterisco
                Sino
                    Escribir " "
                Fin Si
            Fin Para
            Escribir ""
        Fin Para
    Sino
        Escribir "Opción no válida"
    Fin Si

Fin Algoritmo
