# Clústeres de Base de Datos

## Objetivo de la práctica:
Al finalizar la práctica, serás capaz de:
1.	Se va a desarrollar un nuevo sitio web para una tienda de música en línea. 

- Crea un nuevo clúster llamado edbdata con propiedad del usuario enterprisedb.
- Inicia tu clúster edbdata 
- Recarga tu clúster utilizando la utilidad pg_ctl y la función pg_reload_conf()
- Deten tu cluster edbdata en modo rápido (fast mode).


## Objetivo Visual 


![diagrama1](../images/img1.png)

## Duración aproximada:
- 60 minutos.

## Tabla de ayuda:

| Usuario | Password | 
| --- | --- | 
| root | root| 
## Instrucciones 

### Tarea 1. 

1.	Iniciar sesión como usuario root o sudo
2.	Crea el directorio edbdata. Escribe  

```bash
sudo mkdir /edbdata  
```
3.	Cambia la propiedad del directorio al usuario enterprisedb. Escribe:

```bash
sudo chown -R enterprisedb:enterprisedb/edbdata   
```
 <img src="../images/04/01.jpg" width="500" >

 4.	Iniciar session como enterprisedb escribe:

```bash
su – enterprisedb
```

5.	Crea e inicializa el clúster. Escribe: 

```bash
initdb -D /edbdata -W 
```
Luego introduce dos veces la contraseña del superusuario de la base de datos (es decir, la contraseña de enterprisedb).
 <img src="../images/04/02.jpg" width="500" >


6.	Cambia el puerto. Escribe:

```bash
vi /edbdata/postgresql.conf  
```
luego presiona la tecla Insert

<img src="../images/04/03.jpg" width="500" >

7. Cambia  port = 5433 (Recuerda descomentar la linea)
   
<img src="../images/04/04.jpg" width="500" >



### Tarea 2. Descripción de la tarea a realizar.
Paso 1. Debe de relatar el instructor en verbo infinito, claro y conciso cada actividad para ir construyendo paso a paso en el objetivo de la tarea.

Paso 2. <!-- Añadir instrucción -->

Paso 3. <!-- Añadir instrucción -->

### Resultado esperado
En esta sección se debe mostrar el resultado esperado de nuestro laboratorio
![imagen resultado](../images/img3.png)
