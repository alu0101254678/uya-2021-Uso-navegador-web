# __*Usabilidad y Accesibilidad*__
## __*Uso del navegador para el desarrollo web*__
## __*Yago Pérez Molanes (alu0101254678@ull.edu.es)*__

### __Introducción y Objetivos__

En esta práctica se pretende conocer el uso del navegador para el desarrollo web, para ello nos vamos a basar
en el elemento *inspeccionar* sobre los navegadores *Google Chrome* y *Mozilla Firefox.*

La página web que vamos a utilizar es la de cita previa de salud de Canarias: <https://www3.gobiernodecanarias.org/citasalud/>

### __Mozilla Firefox__

![Imagen chrome.jpg](https://raw.githubusercontent.com/alu0101254678/uya-2021-Uso-navegador-web/main/img/firefox.png)

* Qué peticiones desencadena la consulta:

Cuando en la barra de búsqueda de un navegador, escribimos una dirección web, se realizan una serie de consultas o peticiones, a un servidor
que nos da las respuestas, fundamentalmente, se realizan peticiones *http*, de la capa de aplicación, lo que nos quiere decir, que se realiza
una consulta entre el cliente, neustro agente, que es el navegador, y el programa o los programas que se están ejecutando en el servidor.

EL objetivo principal, es obtener un recurso de la web, en este caso, es la página de inicio del servicio canario de la salud.

* Qué tipo de petición estás realizando:

La petición del recurso se está realizando con la petición Get, es decir, que el cliente *quiere* obtener un determinado recurso.

* Qué código de status devuelve:

Normalmente los códigos de estado indican si se ha obtenido algún recurso correctamente, o si ha ocurrido algún fallo, tanto en el servidor
como en el cliente,además de otros tipos.

En la captura posterior se muestran los códigos de estado, tenemos por un lado el código de error 200, que quiere decir, que se ha obtenido el recurso
necesario, y por otro lado, el código de error 304, que indica que un elemento, como una imagen o icono, ya se encontraba en el navegador, y por lo tanto
se encuentra *cacheado*, se trata de una redirección.

![Imagen peticiones http](https://github.com/alu0101254678/uya-2021-Uso-navegador-web/blob/main/img/captura_peticiones_http.png?raw=true)

* Qué DNS tiene el servidor:

El servidor DNS corresponde a *www3.gobiernodecanarias.org*

* Qué IP tiene el servidor:

La dirección IP que tiene el servidor es la *93.188.136.126*, además la comunicación se hace en el puerto *443*

En la captura posterior se encuentran los datos mencionados anteriormente.

![Imagen inspeccion cabecera](https://github.com/alu0101254678/uya-2021-Uso-navegador-web/blob/main/img/captura_cabeceras_inspeccion.png?raw=true)

* ¿La página tiene alguna cookie?¿Cuáles?

Como vemos en la captura anterior aparece una cookie en la cabecera de petición, que corresponde al identificador de sesión.

* ¿Qué idioma acepta?

Los idiomas que acepta son el español de España y el inglés estadounidense.

* Alguna línea de código JavaScript

```JavaScript
!function(n,t){"object"==typeof module&&"object"==typeof module.exports?module.expo
...
```

* Alguna línea de código de CSS que se aplique

Las siguientes líneas de código se aplican al cuerpo de la página web

```CSS
body {
    padding-top: 20px;
    padding-bottom: 20px;
    background: #eee;
    font-family: Segoe UI;

```

* Alguna línea de código HTML que se aplique

En la siguiente captura se muestran algunas líneas de código escrito en HTML, correspondientes a su estructura básica

![Imagen_HTML](https://github.com/alu0101254678/uya-2021-Uso-navegador-web/blob/main/img/captura_lineas_HTML.PNG?raw=true)

### __Google Chrome__

![Imagen Chrome](https://raw.githubusercontent.com/alu0101254678/uya-2021-Uso-navegador-web/main/img/chrome.jpg)

Las peticiones que desencadena la consulta son las mismas que ocurren con el navegador Firefox, sin embargo en esta ocasión 
la búsqueda se ha hecho por primera vez y no tenemos códigos de estado *304*

![Imagen no 304 Chrome](https://raw.githubusercontent.com/alu0101254678/uya-2021-Uso-navegador-web/main/img/captura_chrome_inspeccion_200.PNG)

El DNS del servidor y la dirección IP siguen siendo las mismas, ya que no varían aunque usemos otro navegador

En Google Chrome también se almacenan *Cookies*, como el identificador de sesión, como ocurría en Firefox, aunque su valor
es diferente

![Imagen Cookie Chrome](https://raw.githubusercontent.com/alu0101254678/uya-2021-Uso-navegador-web/main/img/captura_chrome_inspeccion_cookie.PNG)

* Alguna línea de código JavaScript que se aplique:

```JavaScript
!function(n, t) {
    "object" == typeof module && "object" == typeof module.exports ? module.exports = n.document ? t(n, !0) : function(n) {
        if (!n.document)
            throw new Error("jQuery requires a window with a document");
        return t(n)
    }
    : t(n)
}
```

* Alguna línea de código CSS que se aplique:

```CSS
:root {
    --blue: #007bff;
    --indigo: #6610f2;
    --purple: #6f42c1;
    --pink: #e83e8c;
    --red: #dc3545;
    --orange: #fd7e14;
    --yellow: #ffc107;
    --green: #28a745;
    --teal: #20c997;
    --cyan: #17a2b8;
    --white: #fff;
    --gray: #6c757d;
    --gray-dark: #343a40;
    --primary: #007bff;
    --secondary: #6c757d;
    --success: #28a745;
    --info: #17a2b8;
    --warning: #ffc107;
    --danger: #dc3545;
    --light: #f8f9fa;
    --dark: #343a40;
    --breakpoint-xs: 0;
    --breakpoint-sm: 576px;
    --breakpoint-md: 768px;
    --breakpoint-lg: 992px;
    --breakpoint-xl: 1200px;
    --font-family-sans-serif: -apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,"Helvetica Neue",Arial,"Noto Sans",sans-serif,"Apple Color Emoji","Segoe UI Emoji","Segoe UI Symbol","Noto Color Emoji";
    --font-family-monospace: SFMono-Regular,Menlo,Monaco,Consolas,"Liberation Mono","Courier New",monospace
}
```

* Alguna línea de código de HTML que se aplique:

```HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta name="description" content="">
    <meta name="author" content="">
    <link href="/citasalud/favicon.ico" rel="shortcut icon" type="image/x-icon" />
```









