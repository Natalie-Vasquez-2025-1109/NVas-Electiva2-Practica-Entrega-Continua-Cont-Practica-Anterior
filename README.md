# Practica Entrega Continua - Cont Practica Anterior

Aplicacion web Hola Mundo en Python (Flask), empaquetada con Docker y desplegada automaticamente con GitHub Actions.

## Flujo automatizado

Cada push a la rama main ejecuta el workflow `.github/workflows/deploy.yml`, que:

1. Construye la imagen Docker de la aplicacion.
2. Sube la imagen a Docker Hub.
3. Dispara el despliegue en Render.

## Enlaces

- Render: https://nvas-electiva2-practica-entrega-continua.onrender.com/
- Imagen en Docker Hub: https://hub.docker.com/r/naki028/nvas-electiva2-practica-entrega-continua-cont-practica-anterior

## Estructura

- `app.py`: aplicacion Flask.
- `requirements.txt`: dependencias.
- `Dockerfile`: definicion de la imagen.
- `.github/workflows/deploy.yml`: pipeline de GitHub Actions.

## Secrets requeridos en GitHub

- `DOCKERHUB_TOKEN`
- `RENDER_API_KEY`
- `RENDER_SERVICE_ID`
