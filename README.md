# web-minima

Web estática mínima servida con **Node.js** (sin dependencias): fondo verde con el texto **PISTON** centrado.

## Archivos

- `public/index.html` — la página.
- `server.js` — servidor HTTP de Node que sirve la carpeta `public/`.
- `package.json` — script `start` y versión de Node.

## Probar en local

```bash
npm start
# abrir http://localhost:3000
```

El puerto se puede cambiar con la variable de entorno `PORT`:

```bash
PORT=8080 npm start
```

## Desplegar en Dokploy

1. Crear una aplicación nueva (**Application**) en Dokploy.
2. Fuente: este repositorio Git.
3. Build Type: **Nixpacks** (detecta Node automáticamente y ejecuta `npm start`).
4. Puerto de la aplicación: **3000** (el que expone `server.js` por defecto).
   Si necesitas otro, define la variable de entorno `PORT` en **Environment**.
5. Asignar el dominio y desplegar.
