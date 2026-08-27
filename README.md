# web-minima

Web estática mínima: fondo verde con el texto **HOLA** centrado.

## Archivos

- `index.html` — la página.
- `default.conf` — config de nginx (escucha en el puerto 8200).
- `Dockerfile` — imagen nginx que sirve `index.html` en el puerto 8200.
- `docker-compose.yml` — para levantarlo en local.

## Probar en local

```bash
docker compose up --build
# abrir http://localhost:8200
```

O sin Docker, simplemente abrir `index.html` en el navegador.

## Desplegar en Dokploy

1. Crear una aplicación nueva (**Application**) en Dokploy.
2. Fuente: este repositorio Git (o subir los archivos).
3. Build Type: **Dockerfile**.
4. Puerto de la aplicación: **8200**.
5. Asignar el dominio y desplegar.
