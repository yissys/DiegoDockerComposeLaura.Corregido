# 🚀 Personal Blog - Django & Docker Deployment

Este repositorio contiene un sistema de blog desarrollado con **Django**, diseñado para ser desplegado en entornos de producción mediante una arquitectura de contenedores robusta y escalable.

## 🏗️ Arquitectura del Proyecto

El proyecto utiliza una arquitectura de **Proxy Inverso** para separar la lógica de negocio del servicio de archivos estáticos:

* **Django + Gunicorn**: El motor de la aplicación corre sobre Gunicorn, un servidor WSGI de alto rendimiento.
* **Nginx**: Actúa como servidor web frontal, gestionando el tráfico en el puerto 80 y sirviendo archivos estáticos/media directamente.
* **Docker Compose**: Orquestra la comunicación entre los servicios y gestiona los volúmenes compartidos.

## 🛠️ Tecnologías Utilizadas

* **Framework**: Django 5.x
* **Contenedores**: Docker & Docker Compose
* **Servidor Web**: Nginx (Alpine)
* **WSGI**: Gunicorn
* **Base de Datos**: SQLite (desarrollo) / PostgreSQL (preparado para producción)

---

## 🚀 Guía de Instalación y Despliegue

### 1. Clonar el repositorio
```bash
git clone [https://github.com/tu-usuario/personal_blog.git](https://github.com/tu-usuario/personal_blog.git)
cd personal_blog-main
