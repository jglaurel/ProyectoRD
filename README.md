## `Terminal`
- Esto solo se ejecuta al crear el entorno
- Abre una terminal en la carpeta del proyecto y ejecuta:
### `Crear entorno`
- Abre una terminal en la carpeta del proyecto y ejecuta:
```terminal
docker build -t diplomado-env .
```
cambiar el nombre "diplomado" por el que se prefiera

- Una vez construida la imagen, puedes correr el contenedor con:
```terminal2
docker run -p 8888:8888 -v ${PWD}:/workspace diplomado-env
```
y eso es todo

## Limpiar cache
por si ocupa mucho espacio
```cache
RUN pip install --no-cache-dir -r requirements.txt