<div align="center">
  <h1>Sistemas Operacionales<br>Proyecto de Docker - Aplicación de Flutter</h1>
  <p align="center">
  </p>
</div>

En este repositorio se encuentra el proyecto del equipo Starfish, una aplicación de Flutter que se busca virtualizar desde el entorno facilitado por Docker. A lo largo de este archivo de texto se encuentra una guía/tutorial para que los usuarios de sistemas Windows puedan ejecutar nuestro proyecto y así poder calificarlo:

### Requerimientos del Programa:

**Nuestra proyecto de Docker simula el entorno de Flutter y AndroidSDK necesarios para la aplicación, no el emulador de Android en el que se debe ejecutar.**

- **Requerimientos de Emulación de Dispositivo:**
  - Instalación de Android Studio
  - Virtual Device desde Android Studio
  - **Virtual Device Recomendado:** Pixel XL
  - **System Image Recomendada:** Pie
  - **TUTORIAL PARA INSTALAR VIRTUAL DEVICE:** https://developer.android.com/studio/run/managing-avds?hl=es-419


- **Requerimientos de Emulación de Programa: (Instalar como extensiones en VSCode)**
  - Docker
  - Remote Development

| REQUERIMIENTOS DE EMULACIÓN DE PROGRAMA |
|-|
|<img src="https://blog.codemagic.io/uploads/2020/04/extensions.png" >|

- **Requerimientos de Docker**
  - Ejecutar el siguiente comando en CMD para Docker Image de Flutter y AndroidSDK

  ```shell
  docker pull matspfeiffer/flutter
  ```

### Ejecucion del Programa:

En primer lugar deben descargar el programa desde este repositorio de Github, extraerlo y luego abrirlo en VSCode. Si descargaron correctamente los **requerimientos de emulación de programa**, debe aparecer un símbolo de Remote Development <img src="https://ms-vscode-remote.gallerycdn.vsassets.io/extensions/ms-vscode-remote/vscode-remote-extensionpack/0.21.0/1620755254563/Microsoft.VisualStudio.Services.Icons.Default" height="12px" width="12px"> en la esquina inferior izquierda de VSCode:  

| SÍMBOLO DE REMOTE DEVELOPMENT |
|-|
|<img src="https://blog.codemagic.io/uploads/2020/04/docker_1.png" >|

Hacer click sobre el símbolo de Remote Development <img src="https://ms-vscode-remote.gallerycdn.vsassets.io/extensions/ms-vscode-remote/vscode-remote-extensionpack/0.21.0/1620755254563/Microsoft.VisualStudio.Services.Icons.Default" height="12px" width="12px"> y debe aparecer una barra de texto en la parte superior de VSCode. En esta barra deben seleccionar la opción **"Open Folden in Container..."**:

| OPEN FOLDER IN CONTAINER |
|-|
|<img src="https://i.stack.imgur.com/OSnHe.png" >|

Al seleccionar esta opción se va a abrir el explorador de archivos y deberán escoger la carpeta del proyecto **/docker-wassword** (La carpeta que se va a generar automáticamente al extraer el .zip del programa). Una vez seleccionada la carpeta hacer click en la opción **"Open"** del explorador de archivos y VSCode debe reiniciarse y comenzar a crear el contenedor de Docker automáticamente, **este proceso puede demorar unos minutos**. 

Mientras esperamos que VSCode termine de crear el contenedor de Docker vamos a abrir el Virtual Device que descargamos en Android Studio. Abrimos el AVD Manager, buscamos nuestro dispositivo virtual y lo iniciamos oprimiendo el botón <img src="https://cdn.iconscout.com/icon/free/png-256/play-next-forward-replay-arrow-32426.png" height="12px" width="12px">. Una vez que esté corriendo el Virtual Device nos debe quedar algo así:

| DISPOSITIVO VIRTUAL |
|-|
|<img src="https://studyviewer.com/wp-content/uploads/2019/07/android-emulator111111.jpg" >|

Cuando VSCode termine de crear el contenedor de Docker va a iniciar una **bash terminal** para nuestro contenedor. 

| BASH TERMINAL |
|-|
|<img src="https://blog.codemagic.io/uploads/2020/04/docker_4.png" >|

En el **bash terminal** vamos a revisar que todo esté funcionando correctamente. En primer lugar vamos a ejecutar el siguiente comando:

```shell 
flutter doctor 
```

Idealmente, deben aparecer los siguientes resultados:

| RESULTADOS DE FLUTTER DOCTOR |
|-|
|<img src="https://blog.codemagic.io/uploads/2020/04/docker_5.png" >|
