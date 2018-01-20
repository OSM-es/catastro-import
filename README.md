# catastro-import

Se recomienda clonar el repositorio con la opción -n para no descargar los 
archivos generados por otros usuarios.

```
git clone -n https://github.com/OSM-es/catastro-import.git
cd catastro-import
```

Colocar los archivos a publicar para el Gestor de Tareas siguiendo esta estructura.

```
MMMMM (código de municipio)  
  |  
  |- *.gz            ... Archivos de tareas  
  |- address.geojson ... Archivo de enlaces a imágenes
```

Añadir los archivos y subir al servidor. Es importante indicar los archivos en 
el commit para no eliminar los que hayan subido otros usuarios.

```
git add <MMMMM>
git commit -m "MMMMM Nombre del municipio" MMMMM/*
git push -f
```

Es necesario recibir previamente permisos para poder subir archivos.
