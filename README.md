# catastro-import
Temporary container for Spanish Cadastre Buildings Import

Se recomienda clonar el repositorio con la opción -n para no descargar los 
archivos generados por otros usuarios.

'''
git clone -n https://github.com/OSM-es/catastro-import.git
cd catastro-import
'''

Colocar los archivos a publicar para el Gestor de Tareas siguiendo esta estructura.

```
MMMMM (código de municipio)  
  |  
  |- *.gz            ... Archivos de tareas  
  |- address.geojson ... Archivo de enlaces a imágenes
```

Añadir los archivos y subir al servidor

'''
git add <MMMMM>
git commit -m "MMMMM Nombre del municipio"
git push origin master
'''

Es necesario recibir previamente permisos para poder subir archivos.
