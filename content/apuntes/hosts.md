+++
title = 'Hosts Virtuales'
date = 2023-09-25T10:08:10+02:00
+++

### Creacion de Host Virtuales

En este pequeña seccion os voy a expicar los pasos para poder crear Host Virtuales desde Linux utilizando Apache.

#### 1. Instalacion de Apache

Lo primero que haremos sera abrir el terminal de nuestra maquina. Se puede hacer de dos maneras:

Para la le damos a nuesmozillatra tecla de sistema y escribimos *'terminal'*.

Para la segunda hacemos la siguiente combinacion de teclas *'CTRL + ALT + T'*.


Para instalar Apache escribiremos la siguiente linea de codigo en nuestro terminal y le daremos a Enter.

{{< highlight lineNos="false" lineNoStart="1" type="py" >}}
sudo apt-get install apache2
{{< /highlight >}}

#### 2. Creacion del directorio para nuestro sitio Web

Para crear el directorio de tu sitio web, ejecuta los siguientes comandos:

{{< highlight lineNos="false" lineNoStart="1" type="py" >}}
cd /var/www/
{{< /highlight >}}

Esto lo que hara sera movernos al directorio *'www'*.

{{< highlight lineNos="false" lineNoStart="1" type="py" >}}
sudo mkdir /var/www/informatica
{{< /highlight >}}

Esto crea un nuevo directorio llamado "informatica" en la ubicación "/var/www/", que será el espacio para tu sitio web.

#### 3. Asignacion de permisos

El comando asignara permisos a nuestro usario:

{{< highlight lineNos="false" lineNoStart="1" type="py" >}}
sudo chown alumno:www-data /var/www/informatica -R
{{< /highlight >}}

1. **"sudo"** se utiliza para obtener privilegios de superusuario.
2. **"chown"** cambia el propietario y el grupo del directorio y sus contenidos.
3. **"alumno"** se establece como el nuevo propietario.
4. **"www-data"** se asigna como el nuevo grupo.
5. **"/var/www/informatica"** es la ubicación donde se aplican estos cambios.
6. **"-R"** hace que la acción sea recursiva, aplicándose a todos los archivos y subdirectorios dentro de "/var/www/informatica".

#### 4. Creacion de un archivo de Host Virtual.

Crearemos un archivo de host virtual en la carpeta de configuracion de Apache.

{{< highlight lineNos="false" lineNoStart="1" type="py" >}}
sudo nano /etc/apache2/sites-available/informatica.conf
{{< /highlight >}}

Y dentro de este archivo,  configurar el host virtual de esta manera:

{{< highlight lineNos="true" lineNoStart="1" hl_lines="2 3" type="py" >}}
<VirtualHost *:80>
    ServerName informatica.es
    DocumentRoot /var/www/informatica
    ErrorLog ${APACHE_LOG_DIR}/error.log
    CustomLog ${APACHE_LOG_DIR}/access.log combined
</VirtualHost>
{{< /highlight >}}


#### 5. Activacion del Host Virtual

Tendremos que activar el host virtual usando el comando *a2ensite*.

{{< highlight lineNos="false" lineNoStart="1" type="py" >}}
sudo a2ensite informatica.conf
{{< /highlight >}}

#### 6. Editacion del archivho hosts (opcional)

Ejecutaremos el comando:

{{< highlight lineNos="false" lineNoStart="1" type="py" >}}
sudo nano /etc/hosts
{{< /highlight >}}

Agragamos la siguiente linea:


{{< highlight lineNos="true" lineNoStart="1" type="py" >}}
127.0.0.1    informatica.es
{{< /highlight >}}


#### 7. Creacion de un fichero HTML 

Crearemos el fichero HTML añadiendole una linea de texto con el siguiente comando:

{{< highlight lineNos="false" lineNoStart="1" type="py" >}}
echo "<h1>Es sitio de la informática</h1>" >index.html
{{< /highlight >}}

#### 8. Probar el Host Virtual

Escribiremos en nuestro navegador *informatica.es*


![Imagen de nuestra pagina](/PaginaWeb.png)



