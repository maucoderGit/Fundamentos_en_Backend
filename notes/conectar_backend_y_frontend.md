# ¿Como conectar Frontend y Backend?

La manera de conectar Frontend y Backend es a través de una API, que es una parte del backend que permite conectar al Frontend con el backend.

Y existen dos grandes estandares para construir las API's:

- **SOAP**: **S**imple **O**bject **A**ccess **P**rotocol
- **REST**: **Re**presentational **S**tate **T**ransfer

El primer Standart (SOAP), mediante un lenguaje llamado XML(Extensible Markup Lenguage), parecido a HTML, es un lenguaje de marcado que permiten mediante sintaxys especiales compartir información entre diferentes partes del Software.

```XML
    <?xml version="1.0">
    <note>
        <to>Miguel</to>
        <from>Facundo</from>
        <heading>Recordatorio</heading>
        <body>¡No olvides publicar el curso!</body>
    </note>
```

Pero SOAP ya ha quedado un poco en el olvido debido a que REST es mucho más superior a este Standart.

Y para usar REST en una API: Aplication Program Interface, necesitaremos confiar en otro lenguaje:

## JSON

JSON: JavaScript Object Notation, que no es nada más que un diccionario en Python, o un objeto en JavaScript.

```JSON
    {
        "usuario": "maucoder",
        "nombre": "Mauricio Gonzalez",
        "Twitter": "@Maucoder",
    }
```
