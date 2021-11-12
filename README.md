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

| REQUERIMIENTOS DE EMULACIÓN DE PROGRAMA|
|-|
|<img src="https://blog.codemagic.io/uploads/2020/04/extensions.png" >|

- **Requerimientos de Docker**
  - Ejecutar el siguiente comando en CMD para Docker Image de Flutter y AndroidSDK

  ```shell
  docker pull matspfeiffer/flutter
  ```

  ### Ejecucion del Programa:

  En primer lugar deben descargar el programa desde este repositorio de Github, extraerlo y luego abrirlo en VSCode. Si descargaron correctamente los **requerimientos de emulación de programa**, debe aparecer un símbolo de Remote Development <img src="https://ms-vscode-remote.gallerycdn.vsassets.io/extensions/ms-vscode-remote/vscode-remote-extensionpack/0.21.0/1620755254563/Microsoft.VisualStudio.Services.Icons.Default" height="50px" width="50px"> en la esquina inferior izquierda de VSCode:  

| SÍMBOLO DE REMOTE DEVELOPMENT|
|-|
|<img src="https://blog.codemagic.io/uploads/2020/04/docker_1.png" >|