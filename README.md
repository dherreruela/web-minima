# web-minima

Web estática mínima servida con **Node.js** (sin dependencias): fondo verde con el texto **PISTON** centrado.

## Archivos

- `public/index.html` — la página.
- `server.js` — servidor HTTP de Node que sirve la carpeta `public/`.
- `package.json` — script `start` y versión de Node.

## Probar en local

```bash
npm start
# abrir http://localhost:8200
```

El puerto se puede cambiar con la variable de entorno `PORT`:

```bash
PORT=3000 npm start
```

## Desplegar en Dokploy

1. Crear una aplicación nueva (**Application**) en Dokploy.
2. Fuente: este repositorio Git.
3. Build Type: **Nixpacks** (detecta Node automáticamente y ejecuta `npm start`).
4. En **Environment**, definir `PORT` (por ejemplo `8200`) y en la pestaña de red/puertos
   mapear ese mismo puerto de la aplicación.
5. Asignar el dominio y desplegar.
