

<p align="center">  
  <h2 align="center">Unity3D- Bros </h2>

<p align="center">  
 Parte 1 de 3 Guia completa de instalacion en el sistema operativo MacOS   
 Instalacion y configuracion de la utilidad Rosseta Software traductor dinámico binario para Mac OS X  &  Xcode IDE entorno de desarollo  por medio de la linea de comandos

</p>  
    <p align="center">
    <a href="https://github.com/antz22/ultimate-guide-to-flutter/stargazers" alt="Stars">
        <img src="https://img.shields.io/github/stars/antz22/ultimate-guide-to-flutter?style=for-the-badge" /></a>
    <a href="https://github.com/antz22/ultimate-guide-to-flutter/network/members" alt="Forks">
        <img src="https://img.shields.io/github/forks/antz22/ultimate-guide-to-flutter?style=for-the-badge" /></a>
    <a href="https://github.com/Solido/awesome-flutter">
        <img alt="Awesome Flutter" src="https://img.shields.io/badge/Awesome-Flutter-blue.svg?longCache=true&style=for-the-badge" />
    </a>
    <a href="https://img.shields.io/badge/flutter-2.2-green" alt="Flutter">
        <img src="https://img.shields.io/badge/flutter-2.2-green?style=for-the-badge" /></a>
    <a href="https://img.shields.io/badge/dart-2.13-green" alt="Flutter">
        <img src="https://img.shields.io/badge/dart-2.13-green?style=for-the-badge" /></a>
  </p>


---

### Tabla de comtenido 

- [Rosseta Software](#rosseta-software)
- [Xcode Comand line](#xcode-comand-line)



##  Rosseta Software <img  src="https://s3-alpha.figma.com/hub/file/369556540/2b78f13e-cbc8-4e7f-95ad-c00d7c135305-cover"  alt="align"  width="35"  height="35" align="center"  href="https://cdn.iconscout.com/icon/free/png-256/free-rubygems-283026.png?f=webp"/>
> Rosetta es un traductor dinámico binario para Mac OS X que permite a muchas aplicaciones PowerPC correr en ciertas arquitecturas Intel de las computadoras Macintosh sin modificaciones
> para instalar el software Rosetta en macOS en español, sigue estos pasos:  


1. Abre la Terminal en tu Mac. Puedes encontrarla en la carpeta "Utilidades" dentro de "Aplicaciones" o utilizando Spotlight para buscarla.  
  
2. En la Terminal, ingresa el siguiente comando y presiona Enter para ejecutarlo:  
  
	```bash
	sudo softwareupdate --install-rosetta
	```



3. Es posible que se te solicite ingresar tu contraseña de administrador. Ingresa la contraseña y presiona Enter , este comando iniciará el proceso de descarga e instalación de Rosetta en tu Mac.  
  
5. Espera a que se complete la descarga e instalación de Rosetta. Puede llevar un tiempo dependiendo de la velocidad de tu conexión a Internet.  

6. Acepta la lincencia del uso de rosseta software en tu  equipo con el siguiente comando:
	```bash
	sudo softwareupdate --install-rosetta --agree-to-license
	```
 

7. Una vez que la instalación esté completa, podrás utilizar aplicaciones y software diseñado para arquitecturas de procesador diferentes en tu Mac.  
 



###  Rosseta software Comand line
> Rosetta es un traductor dinámico binario para Mac OS X que permite a muchas aplicaciones PowerPC correr en ciertas arquitecturas Intel de las computadoras Macintosh sin modificaciones

-  Instale todas las actualizaciones de software disponibles
	```bash
	sudo softwareupdate -ia
	```
- lista las versiones de rosseta software

	```bash
	sudo softwareupdate --list
	```

- Descarga una versión específica de macOS:

	```bash
	sudo softwareupdate --fetch-full-installer --full-installer-version 10.15.4
	```
-  Activa Rosetta:
	```bash
	sudo softwareupdate --schedule on
	```
	or 
	```bash
	 sudo sysctl -w kern.exec.archhandler.powerpc=/usr/libexec/oah/RosettaNonGrata  
	```

- Desactiva Rosseta
	```bash
	sudo softwareupdate --schedule off
	```
	or 

	```bash
	 sudo sysctl -w kern.exec.archhandler.powerpc=/usr/libexec/oah/RosettaNonGrata
	```

	Con estos comandos, habrás instalado el software Rosetta en tu Mac con macOS en español. Ahora podrás ejecutar aplicaciones y software que no estén diseñados específicamente para el chip M1 de Apple.

	- [x] Rosseta Software esta instalado en el sistema en tu sistema macOS.


## Xcode Comand line <img  src="https://upload.wikimedia.org/wikipedia/en/5/56/Xcode_14_icon.png"  alt="align"  width="35"  height="35" align="center"  href="https://cdn.iconscout.com/icon/free/png-256/free-rubygems-283026.png?f=webp"/>

Xcode es un entorno de desarrollo integrado para macOS que contiene un conjunto de herramientas creadas por Apple destinadas al desarrollo de software para macOS, iOS, watchOS y tvOS.


### Requerimientos del sistema 
> -   `clang`  - C/C++/Objective-C source code into an executable program
>-   `gcc`  - the GNU compiler
>-   `git`  - the save-as-you-go version control system

	


1. Abre la App Store en tu Mac.
2. Busca "Xcode" en la barra de búsqueda.
3. Haz clic en el resultado de búsqueda que corresponda a "Xcode" y selecciona la opción de descarga.
4. Espera a que se complete la descarga e instalación de Xcode desde la App Store.
5. Abre la aplicación "Terminal" en tu Mac. Puedes encontrarla en la carpeta "Utilidades" dentro de la carpeta "Aplicaciones".
6. En la Terminal, escribe el siguiente comando y presiona Enter:
   
	```bash
	sudo Xcode-select --install
	```

7. Se abrirá una ventana emergente que te pedirá confirmar la instalación de las herramientas de línea de comandos de Xcode. Haz clic en "Instalar" y 
![](https://mac.install.guide/assets/images/ruby/install-Xcode-CLT.png)

8. sigue las instrucciones que aparezcan en pantalla.
9. Espera a que se complete la instalación de las herramientas de línea de comandos. Puede llevar algunos minutos.
10. Una vez finalizada la instalación, ya tendrás Xcode Command Line Tools configurado en tu Mac.

![](https://mac.install.guide/assets/images/ruby/install-Xcode-CLT-progress.png)




#### Verificar la instalación de las herramientas de línea de comandos de Xcode



Comprueba que haya instalado correctamente las herramientas de línea de comandos de Xcode:
```bash
sudo xcode-select -p
```

- Deberías ver lo siguiente:
  
  > /Library/Developer/CommandLineTools


```bash
sudo xcodes update
```

- [x] Ahora puedes utilizar las herramientas de línea de comandos de Xcode en tu sistema macOS.

<!--stackedit_data:
eyJoaXN0b3J5IjpbMjEzMDcwNjcyN119
-->