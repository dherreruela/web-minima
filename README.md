# web-minima

Web estática mínima: fondo verde con el texto **HOLA** centrado.

## Archivos

- `index.html` — la página.
- `Dockerfile` — imagen nginx que sirve `index.html` en el puerto 80.
- `docker-compose.yml` — para levantarlo en local.

## Probar en local

```bash
docker compose up --build
# abrir http://localhost:80
```

O sin Docker, simplemente abrir `index.html` en el navegador.

## Desplegar en Dokploy

1. Crear una aplicación nueva (**Application**) en Dokploy.
2. Fuente: este repositorio Git (o subir los archivos).
3. Build Type: **Dockerfile**.
4. Puerto de la aplicación: **80**.
5. Asignar el dominio y desplegar.
