Diagrama de flujo para hallar una cantidad los numeros primos de una cantidad n
```mermaid
flowchart TD
    A["inicio"] --> B("Leer n")
    B --> C("n=cantidad de numeros que se quieren buscar")
    C --> D("Ciclo 1")
    D --> E("I desde 2 hasta n")
    E --> J("Empezar a probar cada numero desde 2 hasta n")
    J --> K("necesitamos algun tipo de contador que empiece desde 0 para al final ver su cantidad exacta de divisores")
    K --> L("Ciclo 2")
    L --> M("j desde 1 hasta i")
    M --> M1("j es el numero por el cual se va a dividir n y i el numero al cual estamos dividiendo")
    M1 -.-> Ñ("se va a mirar cuantos divisores tiene i dividiendolo entre todos los numeros desde i hasta el mismo")
    Ñ --> O("i/j=0=es divisible")
    O --> P("si si es divisible sumará +1 al contador")
    O --> Q("si no lo es sumará +0")
    P --> T("Este va a terminar cuando analice todos los casos para i")
    Q --> T
    T --> R("Si el contador es =2 este será primo")
    R --> S{si es primo se mostrará 'i=primo'}
    S --> U("se seguira su ciclo hasta llegar al n solicitado")
    U --> V("Fin")
