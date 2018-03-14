# catastro-import

Clonar el repositorio.

```
git clone https://github.com/OSM-es/catastro-import.git
cd catastro-import
```

Colocar los archivos a publicar para el Gestor de Tareas siguiendo esta estructura.

```
MMMMM (código de municipio)  
  |  
  |- *.gz         ... Archivos de tareas  
  |- address.osm  ... Archivo de enlaces a imágenes
```

Añadir los archivos y subir al servidor.

```
git add <MMMMM>
git commit -m "MMMMM Nombre del municipio"
git push origin master
```

Es necesario recibir previamente permisos para poder subir archivos.

Si tienes que hacer algún cambio o subir nuevos municipios, primero actualiza el repositorio.

```
git pull
```
