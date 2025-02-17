# Trabajo Práctico 2 - FastAPI

## Descripción
Este proyecto implementa dos APIs simples utilizando FastAPI como parte del trabajo práctico 2 para LEAD University. Las funcionalidades incluyen:
- **POST /usuarios/**: Crear un usuario con nombre, correo y username.
- **GET /usuarios/**: Obtener la lista de usuarios creados.
- **GET /usuarios/{user_id}**: Obtener un usuario específico por su ID.

El proyecto utiliza un sistema de versionamiento en Git y GitHub con las ramas principales:
- `main`
- `staging`
- `develop`
- `feature-post-user` para la implementación de la funcionalidad POST.

---

## Requisitos
- Python 3.x
- FastAPI
- Uvicorn

Instala los paquetes necesarios con:
```bash
pip install fastapi uvicorn
```

---

## Ejecución
Para ejecutar el servidor, utiliza el siguiente comando:
```bash
uvicorn nombre_del_archivo:api --reload
```
Reemplaza `nombre_del_archivo` con el nombre del archivo Python.

Luego, ve a `http://127.0.0.1:8000/docs` para probar los endpoints utilizando la interfaz interactiva de Swagger.

---

## Endpoints
- `POST /usuarios/` - Crea un usuario con un nombre, correo y username.
- `GET /usuarios/` - Obtiene la lista de usuarios registrados.
- `GET /usuarios/{user_id}` - Obtiene un usuario específico por su ID.

---

## Versionamiento en Git
El proyecto utiliza el siguiente flujo de trabajo en Git:
- Se crean ramas `main`, `staging` y `develop`.
- Se desarrolla cada funcionalidad en ramas de características (`feature-*`) y luego se fusionan en este orden:
  1. `feature-*` → `develop`
  2. `develop` → `staging`
  3. `staging` → `main`

Para subir el proyecto a GitHub, utiliza:
```bash
git remote add origin https://github.com/tu_usuario/nombre_repositorio.git
git push origin main staging develop
```

---

## Autor
Trabajo realizado para el curso del Prof. Jorge Zapata en LEAD University por Jason Barrantes.

