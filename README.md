
# Ejercicios Parte 0 - Full Stack

En esta sección podras encontrar los diagramas de secuencia correspondientes a la parte 0 del curso.


0.5: Diagrama de aplicación de una sola página

sequenceDiagram
    participant browser
    participant server

    browser->>server : GET https://studies.cs.helsinki.fi/exampleapp/spa
    activate server
    server-->browser : HTML document
    deactivate server

    browser->>server : GET https://studies.cs.helsinki.fi/exampleapp/main.css
    activate server
    server-->browser : Archivo CSS
    deactivate server 

    browser->>server : GET https://studies.cs.helsinki.fi/exampleapp/spa.js
    activate server
    server-->browser : Archivo JavaScript
    deactivate server

    browser->>server : GET https://studies.cs.helsinki.fi/exampleapp/data.json
    activate server
    server-->browser : [{"content": "D:","date": "2025-03-18T19:47:58.516Z"}, ... ]
    deactivate server

    Note right of browser: El navegador ejecuta la función de llamada de las notas


![Img Ejercicio 0.5](https://raw.githubusercontent.com/kevinbzapata/part0/refs/heads/main/img/Ejercicio%200.5.png)

0.6: Nueva nota en diagrama de aplicación de una sola pagina

![Img Ejercicio 0.6](https://raw.githubusercontent.com/kevinbzapata/part0/refs/heads/main/img/Ejercicio%200.6.png)








