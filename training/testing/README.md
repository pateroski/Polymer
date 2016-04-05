# Polymer training

## Ejercicio complementario: testing unitario

### Introducción

En este ejercicio vamos a implementar tests unitarios para la aplicación agenda, con el objetivo de familiarizarnos con las tecnologías de TDD asociadas al framework.

Las tecnologías puestas en juego para la realización de los tests son:

* **web component tester**: es un entorno de testing E2Eque permite lanzar los tests tanto de forma local como de forma remota cada uno de nuestros componentes.
* **Mocha**: se trata de un framework que nos permite realizar testing unitario, destacando el testing de llamadas asíncronas.
* **Sinon**: es una librería que nos permite implementar stubs, mocks y spies en cualquier framework de testing.
* **Chai**: es otra librería que permite introducir aserciones del estilo *expect(), assert() y should()*

### Herramientas y estructura
1. Instalamos
2. Instalamos **web-component-tester** : ```$ bower install --save Polymer/web-component-tester ```
3. Creamos una carpeta tests, que contendrá los tests que vamos a realizar: ```$ mkdir test```
4. Esta carpeta contendrá un fichero html por componente, **componente.html**, así como un fichero **index.html** en el que se  le especifica a **web-component-tester** qué tests unitarios debe de ejecutar.

### Tests unitarios con Polymer

Los tests unitarios se implementan en ficheros **html**. La estructura de éstos ficheros se muestra a continuación:

```html
<!doctype html>
<html>
  <head>
    <meta charset="utf-8">
    <script src="../bower_components/webcomponentsjs/webcomponents-lite.js"></script>
    <script src="../bower_components/web-component-tester/browser.js"></script>
    <!-- Importación del elemento a testear -->
    <link rel="import" href="../seed-element.html">
  </head>
  <body>
    <!-- Definición de los test-fixtures del componente -->
    <test-fixture id="seed-element-fixture">
      <template>
        <seed-element>
          <h2>seed-element</h2>
        </seed-element>
      </template>
    </test-fixture>
    <!-- Definición de las diferentes suites de tests -->
    <script>
      suite('<seed-element>', function() {
        var myEl;
        setup(function() {
          myEl = fixture('seed-element-fixture');
        });
        test('defines the "author" property', function() {
          assert.equal(myEl.author.name, 'Dimitri Glazkov');
        });
      });
    </script>
  </body>
</html>
```
Explicamos paso a paso, lo que se encuentra en cada una de las partes del fichero:

1. **Importación del componente**:
