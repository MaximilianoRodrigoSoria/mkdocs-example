<p align="center">
<a href="https://www.linkedin.com/in/soriamaximilianorodrigo/" target="_blank" rel="noopener noreferrer">
<img width="100%" height="100%" src="docs/images/banner.gif" alt="Linkedin"></a></p>


<p align="center">
  <a href="#"><img src="https://img.shields.io/badge/Mkdocs-brightgreen" alt="Spring Boot"></a>
  <a href="#"><img src="https://img.shields.io/badge/chat-on%20Discord-7289da.svg?sanitize=true" alt="Chat"></a>
  <a href="#"><img src="https://img.shields.io/badge/Docker-orange" alt="Chat"></a>
</p>

<br>
<br>
<p align="center">
</p>


## 🚀 Introduction

This project aims to generate documentation from static pages created with Mark Down. The project is built with Mkdocs and Mkdocs Material. The project is a simple example of how to create a documentation site using Mkdocs.

## 🔨 Build and Run

## Prerequisites

Ensure you have the following installed on your system:

- Docker
- Python 3

## Steps

### 1. Clone the Repository

Clone your Mkdocs repository to your local machine:

```bash
git clone https://github.com/MaximilianoRodrigoSoria/mkdocs-example.git
```
```
cd mkdocs-example

pip install mkdocs
```

### 2. Build the Project

Navigate to the root directory of your project and execute the following Python command to build the project:
```
mkdocs serve
```

### 3. Access the API
Access the main page of the documentation generated with Mkdocs by entering the following URL in your browser:

> http://127.0.0.1:8000/


### 3. Buid the Project

```
mkdocs build
```

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


---
## 📜 License

[Apache 2.0](http://springdoc.org)

<br/>

### ⭐ Autor
<br>

> ‍💻 **Name:** Maximiliano Rodrigo Soria
>
> 📧 **Email:** MaximilianoRodrigoSoria@gmail.com
>
> 🏠 **From:** Florencio Varela, Alpino
>
> 💼 **Linkedin:** [SoriaMaximilianoRodrigo](https://www.linkedin.com/in/soriamaximilianorodrigo/)
>
> 💬 **Chat:**  [Inicia un chat](https://wa.me/1127043256) 
