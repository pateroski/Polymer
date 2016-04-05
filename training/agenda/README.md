# Polymer training

## Ejercicio 1: Creación de una agenda

Se trata de realizar una agenda que utilice la API: https://randomuser.me/ y nos permita utilizando componentes como **iron-ajax**, **paper-card**, **paper-button**, **iron-icon**,..., mostrar una serie de datos de cada usuario, como la foto, su nombre y el e-mail

### Scaffolding, instalación de herramientas y dependencias:
*(Se parte de **npm** como dependencia ya resuelta)*
1. Instalamos **bower**: ```$ npm install -g bower```
2. Instalamos **polyserve**: ```$ npm install -g polyserve```
3. Creamos el directorio donde vamos a crear la aplicación "agenda": ```$ mkdir agenda```
4. Inicializamos el árbol de dependencias de la aplicación con los valores por defecto: ```$ bower init```
5. Instalamos las dependencias de la aplicación:
```
$ bower install --save Polymer/Polymer
$ bower install --save PolymerElements/iron-ajax
$ bower install --save PolymerElements/paper-button
$ bower install --save PolymerElements/paper-card
$ bower install --save PolymerElements/paper-input
$ bower install --save PolymerElements/iron-icons
```
### Diseño de la aplicación

Existen 2 componentes:

* **contacts-app**: Este componente se encarga de realizar una petición mediante el componente **iron-ajax** a la API y a su vez, hace uso del componente **contact-card**, qué representa la información que deseamos reflejar de la lista de resultados que es devuelta. Para indicar el número de elementos que deseamos mostrar disponemos de un **input**.

* **contact-card**: Este componente se encarga de mostrar la información que está asociada a cada resultado de la API que hemos realizado en el compomente **contacts-app**. Para el layout contenedor de la información a mostrar utiliza **paper-card**. Además dentro de éste utilizamos componentes como **paper-button** y **iron-icon**, que ilustran la funcionalidad de envío de un e-mail.

### Ejecución de la aplicación
1. Instalamos las depedencias necesarias de bower: ```$ bower install```
2. Ejecutamos **polyserve** para servir la aplicación, bajo el directorio **agenda**: ```~/agenda$ polyserve```
3. La **ruta por defecto** donde se sirve es: ```http://localhost:8080/components/agenda/index.html```

####Contribuidores

* [Jon Rojí](https://github.com/jroji)
* [Andrés Reyes](https://github.com/p4ter0ski)
