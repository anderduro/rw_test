# Guía para ejecutar MariaDB con Docker Compose

Esta guía te ayudará a ejecutar un servidor de base de datos MariaDB utilizando Docker Compose.

## Requisitos previos

Antes de comenzar, asegúrate de tener instalado Docker Desktop en tu sistema. Puedes descargarlo e instalarlo desde [el sitio web oficial de Docker](https://www.docker.com/products/docker-desktop).

## Configuración

1. **Descarga el archivo `docker-compose.yml` y `variables.env`**:

   Descarga ambos archivos desde el repositorio o copia su contenido y guárdalo en tu sistema.

2. **Edita el archivo `variables.env`**:

   Abre el archivo `variables.env` en un editor de texto y personaliza las variables según tus preferencias. Puedes cambiar la contraseña de root, el nombre de la base de datos, el nombre de usuario y la contraseña.

3. **Navega hasta el directorio donde guardaste los archivos**:

   Abre la terminam y utiliza el comando `cd` para navegar hasta el directorio de los archivos `docker-compose.yml` y `variables.env`.

4. **Ejecuta el comando Docker Compose**:

   Ejecuta el siguiente comando en tu terminal para iniciar el contenedor de MariaDB:

   ``` docker-compose up -d ```

   Esto creará y ejecutará el contenedor de MariaDB en segundo plano.

5. **Conecta a la base de datos**:

Utiliza tu cliente de base de datos favorito, como MySQL Workbench o DBeaver, para conectarte a la base de datos MariaDB. Utiliza las siguientes credenciales de conexión:

- **Host**: `localhost` o la dirección IP.
- **Puerto**: `3306`
- **Usuario**: El nombre de usuario que especificaste en `variables.env`.
- **Contraseña**: La contraseña que especificaste en `variables.env`.
- **Base de datos**: El nombre de la base de datos que especificaste en `variables.env`.
