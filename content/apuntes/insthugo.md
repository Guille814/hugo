+++
title = 'Hugo'
date = 2023-09-25T10:08:10+02:00
+++

### Instalacion de Hugo 

En esta parte vamos a instalar y configurar Hugo, para utilizar uno de sus themes y crear nuestra propia pagina.

Hugo es una herramienta que nos ayuda a crear paginas estaticas facilmente a traves del lenguaje de Markdown.

#### 1. Instalar Hugo 
Lo primero que vamos a ahcer es instalar la herramienta Hugo en nuestro equipo. 

Para ello le damos a nuestra tecla de sistema y escribimos *'terminal'*.

Para la segunda hacemos la siguiente combinacion de teclas *'CTRL + ALT + T'*.


Para instalar Hugo escribiremos la siguiente linea de codigo en nuestro terminal y le daremos a Enter.

{{< highlight lineNos="false" lineNoStart="1" type="py" >}}
sudo snap install hugo
{{< /highlight >}}

#### 2. Creacion del directorio para nuestro proyecto

Una vez instalado Hugo, crearemos un directorio para alojar nuestro proyecto.

Para crear un directorio escribiremos el comando:

{{< highlight lineNos="false" lineNoStart="1" type="py" >}}
mkdir hugo
{{< /highlight >}}

Con ello, hemos creado un directorio llamado *hugo*. Ahora nos moveremos ahi para crear nuestro proyecto.

{{< highlight lineNos="false" lineNoStart="1" type="py" >}}
cd hugo
{{< /highlight >}}

#### 3. Creacion de nuestro Proyecto

Usaremos en comando *new* para crear el proyecto.

{{< highlight lineNos="false" lineNoStart="1" type="py" >}}
hugo new site <nombre_proyecto>
{{< /highlight >}}

#### 4. Instalacion de un tema

A traves de este [enlace](https://themes.gohugo.io/) podemos explorar y descargar cualquiera de los temas que nos proporcionan.

Una vez elegido el tema, desde nuestro entorno de preferencia, dentro de nuestro proyecto, moveremos la carpeta de *relear* dentro de la carpeta *themes*.

Despues desde nuestra consola nos moveremos dentro de la carpeta relear con el siguiente comando:

{{< highlight lineNos="false" lineNoStart="1" type="py" >}}
cd hugo/<nombre-proyecto>/themes/relearn
{{< /highlight >}}

Una vez ahi clonaremos dentro de ese directorio el theme de Hugo que hayamos elegido.

Suele haber un enlace a Git en cada uno de los temas. Una vez tengamos el enlace a Git lo cargaremos con este comando:

{{< highlight lineNos="false" lineNoStart="1" type="py" >}}
git clone <enlace-a-git>
{{< /highlight >}}

#### 5. Visualizar nuestro proyecto

Para visualizar nuestra pagina desde un navegador, deberemos posicionarnos desde nuestra consola en el directorio de nuestro proyecto, con el comando *cd*.

Una vez posicionados escribimos el siguiente comando:

{{< highlight lineNos="false" lineNoStart="1" type="py" >}}
hugo server &
{{< /highlight >}}

Este comando nos proporcionara una direccion localhost con un puerto, por el cual podemos visualizar nuestra pagina.

![imagen de hugo server](/hugoserver.png)



