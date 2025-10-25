# Repaso Linux

[TOC]

## Capítulo 2 - Ficheros y Directorios (parte I)

Directorios más importantes de un sistema Linux

![image-20250925170254615](./Repaso%20Linux.assets/image-20250925170254615.png)

### Comandos 

- **pwd**: comando que dice al usuario donde se encuentra.

- **ls**: muestra el contenido del directorio actual. por defecto, los archivos ocultos no los muestra.

- **cd**: permite cambiar de directorio. Si se utiliza sin argumento cambia al directorio de trabajo personal. Si s usa seguido de una ruta, cambia al directorio indicado.

- **mkdir**: crea directorios.

- **touch**: permite crear un fichero vacío.

- **ee**: editor de textos muys simple.

- **apt-get**: instala y desintala programas.

- **man**: muestra ayuda sobre un determinado comando.

  

## Ejercicios del capítulo 2

- Muestra del contenido del directorio actual.

![image-20250925171506077](./Repaso%20Linux.assets/image-20250925171506077.png)

```bash
ls
```



- Muestra el contenido del directorio que está justo a nivel superior.

![image-20250925171903743](./Repaso%20Linux.assets/image-20250925171903743.png)

```bash
sudo su
cd ..
ls
```

```bash
ls ..
```



- ¿En qué día de la semana naciste?, utiliza la instrucción cal para averiguarlo.

![image-20250929161634180](./Repaso%20Linux.assets/image-20250929161634180.png)

```bash
cal -d 2005-10
```



- Muestra los archivos del directorio /bin

![image-20250925172229488](./Repaso%20Linux.assets/image-20250925172229488.png)

```bash
cd /bin
ls
```



- Suponiendo que te encuentras en tu directorio personal (/home/nombre), muestra un listado del contenido de /usr/bin a) con una sola línea de comando, b) moviéndote paso a paso por los directorios y c) con dos líneas de comandos.

a. 

<img src="./Repaso%20Linux.assets/image-20250925172505532.png" alt="image-20250925172505532" style="zoom:50%;" />

```bash
ls /usr/bin
```

​	b. <img src="./Repaso%20Linux.assets/image-20250929162146560.png" alt="image-20250929162146560" style="zoom:50%;" />

```bash
cd /usr
cd /bin
ls -la
```



- Muestra todos los archivos que hay en /etc y todos los que hay dentro de cada subdirectorio, de forma recursiva (con un solo comando).

![image-20250929155757234](./Repaso%20Linux.assets/image-20250929155757234.png)

```bash
ls /etc
```

- Muestra todos los archivos del directorio /usr/X11R6/bin ordenados por tamaño (de mayor a menor). Sólo debe aparecer el nombre de cada fichero, sin ninguna otra información adicional.

no existe la carpeta.

![image-20250929163322813](./Repaso%20Linux.assets/image-20250929163322813.png)

```bash
ls /usr/X11R6/bin
```



- Muestra todos los archivos del directorio /etc ordenados por tamaño (de mayor a menor) junto con el resto de características, es decir, permisos, tamaño, fechas de la última modificación, etc. El tamaño de cada fichero debe aparecer en un formato “legible”, o sea, expresado en Kb, Mb, etc.

<img src="./Repaso%20Linux.assets/image-20250929165342325.png" alt="image-20250929165342325" style="zoom:80%;" />

```bash
ls -lhs /etc
```



- Crea el directorio *gastos* dentro del directorio personal. 

```bash
cd /usr
mkdir gastos
```



- ¿Qué sucede si se intenta crear un directorio dentro de /etc?

<img src="./Repaso%20Linux.assets/image-20251002160812334.png" alt="image-20251002160812334" style="zoom:100%;" />



## Capítulo 3 - Ficheros y Directorios (parte II)



<img src="./Repaso%20Linux.assets/image-20251002160216680.png" alt="image-20251002160216680" style="zoom:50%;" />

## Ejercicios del capítulo 3

- Muestra todos los archivos del directorio /usr/bin que empiecen por la letra j.

![image-20251002162742487](./Repaso%20Linux.assets/image-20251002162742487.png)

- Crea un fichero vacío con nombre “*?Hola caracola?*”. ¿Se puede? En caso de que se pudiera, ¿sería recomendable poner nombres así? Razona la respuesta.

Si se puede a pesar de que no sea nada recomendado. Para empezar al tener un nombre compuesto (dos palabras) y encima tiene caracteres especiales (?) en algunos ordenadores podrían no poder buscar el directorio.

![image-20251002163300277](./Repaso%20Linux.assets/image-20251002163300277.png)

- Muestra los archivos del directorio /bin que terminen en n.

  ![image-20251002170115497](./Repaso%20Linux.assets/image-20251002170115497.png)

## Capítulo 4 - Grupos, Usuarios y Permisos

### Superusuario

Superusuario (administrador del sistema o simplemente root): usuario especial que tiene privilegios para cambiar la configuración, borrar y crear ficheros en cualquier directorio, crear nuevos grupos y usuarios.

> IMPORTANTE: ES PELIGROSO TRABAJAR COMO SUPERUSUARIO, SE PUEDE DAÑAR EL SISTEMA DE FORMA IRREVERSIBLE EL LECTOR DEBE ESTAR SEGURO DE LO QUE HACE CUANDO TRABAJE COMO SUPER USUARIO.

### Permisos

la información sobre grupos, usuarios y permisos se puede obtener mediante el comando ls junto la opción -l.

<img src="./Repaso%20Linux.assets/image-20251002163551921.png" alt="image-20251002163551921" style="zoom:50%;" /> 

<img src="./Repaso%20Linux.assets/image-20251002163612719.png" alt="image-20251002163612719" style="zoom:50%;" />

### Gestión de grupos

los comandos `groupadd`, `groupdel` y `groupmod` permiten crear, borrar y modificar grupos.

### Gestión de usuarios

la gestión de usuarios exige que los comandos se ejecuten con los privilegios del administrador. Se puede escribir `sudo` antes de cada comando, o se puede hacer lo siguiente: 

```bash
sudo bash
```

### Cambio de privilegios

El comando `chmod` sirve para cambiar los permisos de uno o varios ficheros. Esos permisos que pueden ver con ls -l.

<img src="./Repaso%20Linux.assets/image-20251002172219677.png" alt="image-20251002172219677" style="zoom:67%;" />

<img src="./Repaso%20Linux.assets/image-20251002163652354.png" alt="image-20251002163652354" style="zoom:50%;" />



