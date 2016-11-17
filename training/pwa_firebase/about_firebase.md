## Firebase y PWA: ToDo App

**¡Importante!:** es necesario seguir las instrucciones indicadas en el codelab para finalizar correctamente el ejercicio

### Codelabs
* [PWA y Firebase](https://codelabs.developers.google.com/codelabs/polymer-firebase-pwa/index.html#0)

### ¿Qué es Firebase?
* [Videos de introducción](https://www.youtube.com/watch?v=O17OWyx08Cg&list=PLl-K7zZEsYLmOF_07IayrTntevxtbUxDL)
* [Firecasts](https://www.youtube.com/watch?v=k1D0_wFlXgo&list=PLl-K7zZEsYLmnJ_FpMOZgyg6XcIGBu2OX)
* [Consola de gestión](https://console.firebase.google.com/)
* [Documentación](https://firebase.google.com/docs/web/setup)
* [Comandos de firebase](https://firebase.google.com/docs/cli/)

### Desarrollo del Codelab

#####Componentes de todo-app (lógica de presentación)
* [\<na-toolbar\>\</na-toolbar\>](https://github.com/polymerlabs/note-app/blob/master/common/note-app/na-toolbar.html)
* [\<na-login\>\</na-login\>](https://github.com/polymerlabs/note-app/blob/master/common/note-app/na-login.html)
* [\<paper-fab\>\</paper-fab\>](https://github.com/Polymerelements/paper-fab)
* [\<na-editor\>\</na-editor\>](https://github.com/polymerlabs/note-app/blob/master/common/note-app/na-editor.html)
* [\<na-note\>\</na-note\>](https://github.com/PolymerLabs/note-app-elements/blob/master/na-note.html)

#####Componentes de firebase usados (modelo de datos)
* [\<firebase-app\>\</firebase-app\>](https://elements.polymer-project.org/elements/polymerfire?active=firebase-app)
* [\<firebase-auth\>\</firebase-auth\>](https://elements.polymer-project.org/elements/polymerfire?active=firebase-auth)
* [\<firebase-document\>\</firebase-document\>](https://elements.polymer-project.org/elements/polymerfire?active=firebase-document)
* [\<firebase-query\>\</firebase-query\>](https://elements.polymer-project.org/elements/polymerfire?active=firebase-query)
* [\<app-indexeddb-mirror\>\</app-indexeddb-mirror>](https://elements.polymer-project.org/elements/app-storage?active=app-indexeddb-mirror)


### Learning outcomes:

#####1. Manifest.json
* [Generador manifest.json](https://app-manifest.firebaseapp.com/)
* [Documentación W3C](https://www.w3.org/TR/appmanifest/)


#####2. Service Worker
* [¿Qué es un service worker?](https://developers.google.com/web/fundamentals/primers/service-worker/)
* [Implementación paso a paso](https://www.smashingmagazine.com/2016/02/making-a-service-worker/)
* [Documentación W3C](https://www.w3.org/TR/service-workers/)
* [sw-toolbox](https://googlechrome.github.io/sw-toolbox/)

#####3. Platinum-sw (web component for service workers config)
* [platinum-sw](https://github.com/PolymerElements/platinum-sw)
* [\<platinum-sw-register\>](https://elements.polymer-project.org/elements/platinum-sw?active=platinum-sw-register)
* [\<platinum-sw-cache\>](https://elements.polymer-project.org/elements/platinum-sw?active=platinum-sw-cache)

#####4. firebase app (web component for firebase integration)
* [firebase-elements](https://elements.polymer-project.org/elements/polymerfire)
* [firebase usage](https://github.com/firebase/polymerfire)
