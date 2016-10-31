# Polymer training

Se trata de una serie de ejercicios cuyo objetivo es acercarnos la tecnologías puestas en juego a través de la librería de comonentes **Polymer**. Además se incluyen otros ficheros de documentación con el objeto de complementar información sobre Polymer y sobre las tecnologías puestas en juego.

### Scaffolding e instalación de herramientas:

1. Instalamos **bower**: ```$ npm install -g bower```
2. Instalamos **polyserve**: ```$ npm install -g polyserve```
3. Instalamos **web component tester**: ```npm install -g wct```
4. Creamos el directorio donde vamos a crear la aplicación: ```$ mkdir aplicación```
5. Inicializamos el árbol de dependencias de la aplicación con los valores por defecto: ```$ bower init```
6. Instalamos las dependencias del ejercicio en cuestión

### Dependencias

#### 1. Dependencias de la aplicación:

Estas son aquellas dependencias que son necesarias para la ejecución de la aplicación. Estas se pueden instalar:

```
$ bower install --save <dependencia>
```
ó
```
$ bower install -S <dependencia>
```
#### 2. Dependencias de desarrollo:

Estas son aquellas dependencias que han surgido en algún momento del desarrollo de la aplicación pero que no son necesarias para desplegar la aplicación. Estas se pueden instalar:

```
$ bower install --save-dev <dependencia>
```
ó
```
$ bower install -D <dependencia>
```

### Ejecución de la aplicación

1. Instalamos las depedencias necesarias de bower: ```$ bower install```
2. Ejecutamos **polyserve** para servir la aplicación, bajo el directorio **nombre_app**: ```~/nombre_app/$ polyserve```
3. La **ruta por defecto** donde se sirve es: ```http://localhost:8080/components/nombre_app/index.html```

* **Nota**: si se desea modificar el nombre de la ruta donde se ejecuta la aplicación podemos hacerlo modificando la clave **"name"** del fichero **bower.json**.


## Ejercicio 1: creación de una agenda

Se trata de realizar una agenda que utilice la API: https://randomuser.me/ y nos permita utilizando componentes como **iron-ajax**, **paper-card**, **paper-button**, **iron-icon**,..., mostrar una serie de datos de cada usuario, como la foto, su nombre y el e-mail.

### Dependencias

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

## Ejercicio 2: creación de un elemento custom - **toggle-icon**

Se trata de realizar un **elemento custom** que crearemos a partir de uno ya existente, en este caso, **iron-icon**. El objetivo es aprender a crear un elemento custom como la documentación asociada al mismo, utilizando para ello **iron-component-page** y **iron-demo-helpers**.

### Dependencias

Las **dependencias de aplicación** son las siguientes:
```
$ bower install --save Polymer/Polymer
$ bower install --save PolymerElements/iron-icon
```
Las **dependencias de desarrollo** son las siguientes:
```
$ bower install --save-dev iron-component-page
$ bower install --save-dev iron-icons
$ bower install --save-dev iron-demo-helpers
```

## Ejercicio 3: creación de una agenda con distintas vistas

Se trata de, siguiendo los mismos pasos que en el ejercicio 1, crear 2 vistas distintas para la generación de la misma agenda. Para una utilizaremos el componente **paper-card** y para la otra utilizaremos el compomente **paper-item**.

### Dependencias

Las **dependencias de aplicación** son las siguientes:

```
$ bower install --save Polymer/Polymer
$ bower install --save PolymerElements/iron-ajax
$ bower install --save PolymerElements/paper-button
$ bower install --save PolymerElements/paper-card
$ bower install --save PolymerElements/paper-input
$ bower install --save PolymerElements/paper-item
$ bower install --save PolymerElements/paper-icon-button
$ bower install --save PolymerElements/iron-image
```
## Ejercicio 4: creación de tests unitarios

Se trata de la implementación de tests unitarios sobre el **ejercicio 1**. El objetivo es utilizar el framework de Testing **MochaJS** y las aserciones de **ChaiJS** para la creación de tests.


## Ejercicio 5: inserción de la agenda utilizando psk

Se trata de integrar el **ejercicio 3** (agenda_lists) dentro **polymer starter kit**. Se trata de añadir una nueva sección del menú y una nueva template que integre dicho componente

* **Pasos**:
  * Descargar psk: ```git clone  git@github.com:PolymerElements/polymer-starter-kit.git```
  * Instalar polytool: ```npm install -g polytool```
  * bower install
  * polytool serve

## Ejercicio 6: construcción de un TODO app usando PWA y Firebase

* [PWA y Firebase](https://codelabs.developers.google.com/codelabs/polymer-firebase-pwa/index.html#0)

Se trata de implementar una aplicación para almacenar nuestras notas TODO como una PWA y con Firebase como base de datos en tiempo real, permitiendo autenticación de usuarios, datos de usuario offline y permitiendo que se comporte como una aplicación móvil instalable

####Contribuidores

* [Jon Rojí](https://github.com/jroji)
* [Andrés Reyes](https://github.com/p4ter0ski)
