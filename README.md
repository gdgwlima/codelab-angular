# Codelab Angular & Firebase 
Build app using Angular and Firebase Hosting

Prerequisitos : 

- Uso de editor (VSCode o SublimeText)
- NodeJS

Luego, abrir la consola e instalar Angular CLI :

```sh
npm install -g @angular/cli
```
Al finalizar la instalación, crearemos un nuevo proyecto:

```sh
ng new demo-angular
cd demo-angular
```

Lo abrimos en nuestro browser( ejemplo http://localhost:4200/ ): 

```sh
ng serve
```

Para configurar Firebase a nuestra aplicación Angular,en la consola con la ruta de nuestro directorio ingresamos : 

```sh
npm install angularfire2 firebase --save
```
Ingresamos a la consola de Firebase (Login con Gmail) y creamos nuestra aplicación :

https://console.firebase.google.com/

En el archivo app.module.ts de nuestro proyecto, agregamos: 

```sh
import {AngularFireModule} from 'angularfire2';
```
Luego para agregar el JSON con la información de nuestro proyecto en la consola de Firebase,agregamos una constante :


En el Import agregamos : 
```sh
AngularFireModule.initializeApp(firebaseConfig)
```
