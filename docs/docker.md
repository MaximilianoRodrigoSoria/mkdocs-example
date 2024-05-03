# 🐳 Dockerizacion

## Docker

Este proyecto se puede dockerizar para facilitar la distribución y ejecución de la documentación generada con Mkdocs.
Para ello puedes seguir los siguientes pasos.

### Dockerfile

Este archivo es necesario para construir la imagen de Docker que contendrá la documentación generada con Mkdocs. 

```Dockerfile
FROM squidfunk/mkdocs-material

COPY . /docs
WORKDIR /docs

```

##### 1. Construir la imagen

```bash
docker build -t mkdocs-example .
```

##### 2.Ejecutar el contenedor

```bash
docker run -p 8000:8000 mkdocs-example
```

##### 3.Acceder

```bash
http://localhost:8000
```


### Docker Compose

Tambien podemos acceder a la documentación con Docker Compose.

```yaml
version: '3'

services:
  mkdocs:
    build: .
    ports:
      - "9001:8000"
    volumes:
      - .:/docs

```

##### 1. Construir la imagen

```bash
docker-compose build
```

##### 2. Ejecutar el contenedor

```bash
docker-compose up -d
```

##### 3. Acceder

```bash
http://localhost:9001
```