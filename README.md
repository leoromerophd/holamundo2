# Aplicación Ionic de Información de la Empresa

Este repositorio contiene un ejemplo mínimo de cómo crear una aplicación
utilizando [Ionic Framework](https://ionicframework.com/) para mostrar
información general de una empresa.

## Pasos básicos

1. Instalar la interfaz de línea de comandos de Ionic:
   ```bash
   npm install -g @ionic/cli
   ```
2. Crear un nuevo proyecto (por ejemplo `infoEmpresa`):
   ```bash
   ionic start infoEmpresa blank --type=angular
   ```
3. Entrar en la carpeta del proyecto y agregar una página llamada
   `info-general`:
   ```bash
   cd infoEmpresa
   ionic generate page pages/info-general
   ```
4. Editar `src/app/pages/info-general/info-general.page.html` para
   incluir los datos de tu empresa. Un ejemplo sencillo:
   ```html
   <ion-header>
     <ion-toolbar>
       <ion-title>Información de la Empresa</ion-title>
     </ion-toolbar>
   </ion-header>

   <ion-content class="ion-padding">
     <h2>Nombre de la Empresa</h2>
     <p>Breve descripción de la empresa.</p>
     <ion-list>
       <ion-item>
         <ion-label>Dirección</ion-label>
         <ion-text>Av. Principal 123</ion-text>
       </ion-item>
       <ion-item>
         <ion-label>Teléfono</ion-label>
         <ion-text>+34 000 000 000</ion-text>
       </ion-item>
       <!-- Agrega más información según sea necesario -->
     </ion-list>
   </ion-content>
   ```
5. Asegurarse de que la nueva página esté declarada en
   `src/app/app-routing.module.ts` para poder navegar hacia ella.
6. Ejecutar la aplicación de desarrollo:
   ```bash
   ionic serve
   ```

Con estos pasos tendrás una aplicación básica en Ionic que muestra la
información general de tu empresa. Desde aquí puedes personalizar el
estilo y agregar más funcionalidades según tus necesidades.

