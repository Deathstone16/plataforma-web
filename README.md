# Turnario

Landing page B2B responsive para presentar un sistema ficticio de gestión de turnos dirigido a profesionales y centros pequeños.

## Tecnologías

- Astro
- TypeScript
- Tailwind CSS
- Phosphor Icons
- Manrope Variable, servida localmente

## Requisitos

- Node.js 20.19.1 o superior
- npm 9.6.5 o superior

## Instalación

```bash
npm install
```

Creá el archivo local de variables de entorno a partir del ejemplo:

```bash
cp .env.example .env
```

La variable pública demostrativa es:

```env
PUBLIC_APP_NAME=Turnario
```

No guardes credenciales ni información sensible en variables con el prefijo `PUBLIC_`, porque quedan disponibles en el sitio generado.

## Desarrollo local

```bash
npm run dev
```

El servidor de desarrollo informará la dirección local, normalmente `http://localhost:4321`.

## Validación y build

```bash
npm run check
npm run build
```

El build estático se genera en `dist/`.

Para revisar el resultado de producción localmente:

```bash
npm run preview
```

## Despliegue

### Vercel

1. Subí el proyecto a GitHub.
2. Importá el repositorio en Vercel.
3. Agregá `PUBLIC_APP_NAME` en las variables del proyecto.
4. Vercel detectará Astro y ejecutará `npm run build`.

### Netlify

- Build command: `npm run build`
- Publish directory: `dist`
- Agregá `PUBLIC_APP_NAME` en la configuración de variables de entorno.

## Alcance de la demostración

- No procesa pagos.
- No almacena datos de pacientes.
- Los precios, testimonios y contactos son ficticios.
- Los botones de contacto utilizan direcciones de ejemplo.
