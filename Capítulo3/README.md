# Instalación de EDB Postgres Advanced Server

## Objetivo de la práctica:
Al finalizar la práctica, serás capaz de:
1.	Elegir la plataforma en la que deseas instalar EDB Postgres Advanced Server.
2.	Descargar el instalador de EDB Postgres Advanced Server desde el sitio web de EnterpriseDB correspondiente a la plataforma elegida.
3.	Preparar la plataforma para la instalación.
4.	Instalar EDB Postgres Advanced Server.
5.	Conéctar a EDB Postgres Advanced Server utilizando psql.


## Objetivo Visual 
Crear un diagrama o imagen que resuma las actividades a realizar, un ejemplo es la siguiente imagen. 

![diagrama1](../images/img1.png)


## Duración aproximada:
- 90 minutos.

## Tabla de ayuda:
Agregar una tabla con la información que pueda requerir el participante durante el laboratorio, como versión de software, IPs de servers, usuarios y credenciales de acceso.
| Contraseña | Correo | Código |
| --- | --- | ---|
| Netec2024 | edgardo@netec.com | 123abc |

## Instrucciones 
<!-- Proporciona pasos detallados sobre cómo configurar y administrar sistemas, implementar soluciones de software, realizar pruebas de seguridad, o cualquier otro escenario práctico relevante para el campo de la tecnología de la información -->
### Tarea 1. Instalación

1.	Crea el usuario enterprisedb.  Escriba lo siguiente:
  a.	Iniciar sesión como  root.  Escriba 
  ```shell
  su - root
  ``` 
  y luego ingrese la contraseña de root.
  
  Agregue usuario y password para enterprisedb
  
  ```shell
  useradd enterprisedb
  passwd enterprisedb
  ```	
  
  b.	Ingrese la contraseña edb y luego introduzcala nuevamente edb.
  
  ![01](../images/01/01.png)

2.	Inicie sesión en su entorno Linux como superusuario.
 
4.	Para instalar EDB Postgres Advanced Server mediante RPM, necesita el repositorio EPEL. Primero, instale el repositorio EPEL con el comando yum. Escriba:  

  ```shell
  su – root 
  ```
Y luego la contraseña de root

```shell
# yum install epel-release 
```
![02](../images/01/02.png)

4.	A continuación, abra una ventana del navegador y vaya a https://www.enterprisedb.com/downloads/edb-postgres-advanced-server   

- Producto = EDB Postgres Advanced Server.
- Versión = 13.0.
- Sistema operativo = Linux x86-64 & 32.
- Tipo = RPM.
- Cómo acceder = hacer clic en Access Repository.
- Inicie sesión o regístrese para obtener una cuenta de sitio web si se solicita.
  - Si ya tiene credenciales, utilízalas para iniciar sesión y acceder a yum.enterprisedb.com con el fin de descargar el repositorio RPM.
  - Si no tiene credenciales, regístrate y recibirás un correo electrónico de EnterpriseDB en tu dirección de correo electrónico registrada con las credenciales para acceder a yum.enterprisedb.com y descargar el repositorio RPM. 
 
5.	Ve a yum.enterprisedb.com . Si se te solicita, introduce tu nombre de usuario y contraseña y haz clic en edb-repo para descargar el repositorio RPM. 
 
6.	Ve a la carpeta Descargas. Escribe los siguientes comandos
```shell
cd /home/(username)/Downloads/  ls 
```
Podrás encontrar el archivo del RPM llamado edb-repo-latest.norach.rpm 

7.	Instala edb-repo-latest.noarch.rpm como usuario root. Escriba:

```shell
su – root 
```

y luego ingresa la contraseña de root 

```shell
rpm –ivh edb-repo-latest.noarch.rpm 
```

![03](../images/01/03.png)

### Tarea 2. Descripción de la tarea a realizar.
Paso 1. Debe de relatar el instructor en verbo infinito, claro y conciso cada actividad para ir construyendo paso a paso en el objetivo de la tarea.

Paso 2. <!-- Añadir instrucción -->

Paso 3. <!-- Añadir instrucción -->

### Resultado esperado
En esta sección se debe mostrar el resultado esperado de nuestro laboratorio
![imagen resultado](../images/img3.png)
