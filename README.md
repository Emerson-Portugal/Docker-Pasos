# Introduccin a Docker

> Docker es una plataforma de contenerización de código abierto. Permite a los desarrolladores empaquetar aplicaciones en contenedores: componentes ejecutables estandarizados que combinan el código fuente de la aplicación con las bibliotecas del sistema operativo (SO) y las dependencias necesarias para ejecutar dicho código en cualquier entorno.

## Imagenes en Docker

> Para listar las imagenes descargas

```
docker images
```
> Para descargar images
```
docker pull "imagen"
```
> Para descargar una version de la imagen
```
docker pull "image":"version"
```
> Para eliminar una imagen 
```
docker image rm "imagen"
```

## Contenedores en Docker Parte1

> Para listar los contenedores activos
```
docker ps
```

> Para listar todos los contenedores
```
docker ls -a
```

> Para crear un contenedor
```
docker create "contenedor"
``` 

> Para iniciar un contenedor
```
docker start "contenedor"
```

> Para pausar un contenedor
```
docker stop "contenedor"
``` 

> Para eliminar un contenedor
```
docker rm "name_defecto"
```

## Contenedores en Docker parte2

> Aqui podemos poner el nombre al contenedor
```
docker create --name "tu_nombre" "imagen"
```
> Empezar el contenedor
```
docker start "tu_nombre"
```
> Creamos un contenedor con puerto, nombre y distro
```
docker create -p"puesto_pc":"puerto_docker" --name "tu_nombre" "imagen"
```
> Para comprobar si el contenedor esta activo
```
docker logs "tu_nombre"
```

>>> Este Es el comando TOP, para descargar, crear y ejecutar
```
docker run -d --name "tu_nombre" -p"puerto_pc":"puerto_docker" "imagen"
```