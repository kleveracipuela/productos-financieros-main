
Fue realizado con Angular 17.3 y TypeScript 5.4. Los estilos son SCSS escrito a mano, sin librerías de componentes ni frameworks de CSS.

## Requisitos

- Node.js 18 o superior 
- npm
- El backend del ejercicio corriendo en `http://localhost:3002`

## Cómo levantarlo

Primero el backend. Desde la carpeta `repo-interview-main`:
*************************
npm install
npm run start:dev
Queda escuchando en el puerto 3002.
*****************************************
Después el frontend, desde la carpeta de este proyecto:

npm install
npm start
```
Abrir `http://localhost:4200`.

`npm start` levanta `ng serve` con `proxy.config.json`, que redirige todo lo que empieza con `/api` hacia `http://localhost:3002`. Así se evita el problema de CORS sin tocar el backend. Si se corre `ng serve` directamente, sin el proxy, las llamadas a la API van a fallar.

**************************
Para generar el build:
npm run build
*****************************

## Pruebas unitarias

Las pruebas están con Karma + Jasmine, que es lo que trae Angular CLI por defecto.


