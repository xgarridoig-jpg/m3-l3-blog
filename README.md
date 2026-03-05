# Chilwe — Content Management System

![Python](https://img.shields.io/badge/Python-3.10%2B-blue?style=flat-square&logo=python&logoColor=white)
![Django](https://img.shields.io/badge/Django-4.x-092E20?style=flat-square&logo=django&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-14%2B-4169E1?style=flat-square&logo=postgresql&logoColor=white)

**Chilwe** es una aplicación web desarrollada con **Django** orientada a la gestión y publicación de contenido editorial.  
El proyecto implementa un modelo relacional para organizar **autores y artículos**, utilizando **PostgreSQL** como base de datos y el **ORM de Django** para la interacción con los datos.

La aplicación está construida siguiendo la arquitectura **MTV (Model–Template–View)** del framework y funciona como base para un sistema de publicación de contenido.

---

## Características

- Modelado relacional entre **autores y artículos**
- Gestión de contenido mediante **Django Admin**
- Generación automática de **slugs** para URLs
- Consultas a base de datos mediante **Django ORM**
- Organización modular del proyecto siguiendo convenciones de Django

---

## Stack tecnológico

- **Python**
- **Django**
- **PostgreSQL**
- **Django ORM**
- **Git**

---

## Arquitectura del proyecto

```

chilwe/
│
├── blog_platform/
│   ├── blog_platform/
│   │   ├── settings.py
│   │   ├── urls.py
│   │   └── ...
│   │
│   ├── blog/
│   │   ├── migrations/
│   │   ├── models.py
│   │   ├── views.py
│   │   ├── admin.py
│   │   ├── templates/
│   │   └── static/
│   │
│   └── manage.py
│
└── evidencias/

````

La aplicación principal es **blog**, donde se definen los modelos, vistas y lógica de negocio del sistema.

---

## Instalación y ejecución

Requisitos:

- Python 3
- PostgreSQL

### 1. Clonar repositorio

```bash
git clone https://github.com/xgarridoig-jpg/chilwe.git
cd chilwe
````

### 2. Crear entorno virtual

```bash
python -m venv venv
source venv/bin/activate

# Windows
venv\Scripts\activate
```

### 3. Instalar dependencias

```bash
pip install -r requirements.txt
```

### 4. Configurar PostgreSQL

Crear una base de datos y ajustar los parámetros de conexión en:

```
settings.py
```

### 5. Ejecutar migraciones

```bash
python manage.py makemigrations
python manage.py migrate
```

### 6. Ejecutar servidor

```bash
python manage.py runserver
```

Acceder a:

```
http://127.0.0.1:8000/
```

Panel administrativo:

```
http://127.0.0.1:8000/admin/
```

---

## Proyección del proyecto

La estructura actual permite extender el sistema hacia funcionalidades como:

* autenticación de usuarios
* categorización de contenido
* sistema de comentarios
* API para consumo externo

---

## Autora

**Ximena Garrido**
Backend Developer

Portafolio
[https://xgarridoig-jpg.github.io/](https://xgarridoig-jpg.github.io/)

LinkedIn
[https://www.linkedin.com/in/xpgarrido/](https://www.linkedin.com/in/xpgarrido/)


y dejar ese repo **muy sólido para reclutadores**.
```
