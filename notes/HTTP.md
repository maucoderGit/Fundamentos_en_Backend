# El lenguaje que habla a internet: HTTP

**H**ype/r**t**ext **T**ransfer **P**rotocol o Protocolo de Transferencia de Hipertexto. De que se trata todo este protocolo, *¿qué es HTTP?*

Pero antes de ahondar o conocer un poco más de HTTP, quiero que conozcas dos conceptos: Cliente y Servidor.

Nosotros en internet tenemos dos partes que siempre se comunican, Los clientes y los servidores:

- Los **Clientes**: Que son estos dispositivos que se concectan y tienes al alcance de tu mano.

- Un **Servidor** es una computadora que esta encendida las 24 horas del día y se mantiene conectada con tu cliente.

Cuando tu navegas a través de la web, haces peticiones(**"Requests"**) a un servidor, el cual te da una respuesta(**"Response"**) que trae en ella la página web.

Ese el recorrido que hace un cliente y servidor, hace una petición y el servidor a través de una API, devuelve la información.

Veamos como se ve una petición y una respuesta:

```http
    # Request
    
    GET / HTTP/1.1
    Host: developer.mozilla.org
    Accept-language: fr

    # Response

    HTTP/1.1 200. OK
    DATE: Sat, 09 Oct 2010 14:20:02 GTM
    Server: Apache
    Last-Modified: Tue, 01 Dec 2009 20:18:22 GTM
    ETag: "51142bc1-7449-479b05b2891b"
    Accept-Ranges: bytes
    Content-Length: 29789
    Content-Type: text/html
```

- A estas variables por asi decirles, se les llamaran cabeceras o Headers, y así se conforma una petición con protocolo HTTP.

- El método en este caso es GET, lo podemos ver encima de la cabecera, pero tenemos muchos otros como PULL, GET, etc...

- El servidor al recibir esta petición tambien contestara con HTTP, pero con un Response.

- También tenemos el status code, que en este caso es el 200, significa que todo esta OK y la respuesta del servidor funciona correctamente.

- Podemos ver información adicional de la respuesta como la fecha, el tipo de respuesta, la cantidad de bytes, etc...

Pero ¿por qué llamamos protocolo a este proceso? pués se le llama así debido a que es un conjunto de reglas que sirven para comunicar dos partes, es decir, si le pedimos a la computadora que llame al servidor, simplemente no podra ir y decir, "Pana, traeme el servidor", la computadora necesita un idioma especifico al cual traducir en código maquína.
