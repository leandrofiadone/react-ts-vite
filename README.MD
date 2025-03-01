
# package.json Boilerplate for Vite + React TypeScript Project

Este boilerplate es una configuración básica para un proyecto de frontend utilizando Vite, React, TypeScript y Sass. Incluye las dependencias necesarias para trabajar con React, React Router y herramientas de desarrollo como ESLint y TypeScript.

## Descripción

Este proyecto está diseñado como un punto de partida para aplicaciones de frontend modernas utilizando Vite como el bundler, React para la interfaz de usuario, y TypeScript para un desarrollo más robusto con tipado estático.

## Estructura del Proyecto

El proyecto tiene la siguiente estructura básica:

```
my-project/
├── src/              # Código fuente del proyecto
├── public/           # Archivos públicos como index.html
├── .eslintrc.json    # Configuración de ESLint
├── package.json      # Dependencias y scripts de Node.js
├── tsconfig.json     # Configuración de TypeScript
└── vite.config.ts    # Configuración de Vite
```

## Dependencias

El proyecto incluye las siguientes dependencias:

### Dependencias principales:

- `@types/react-router-dom`: Tipos de TypeScript para `react-router-dom`.
- `axios`: Cliente HTTP para hacer solicitudes.
- `react`: Biblioteca principal para construir interfaces de usuario.
- `react-dom`: Para interactuar con el DOM de React.
- `react-router-dom`: Librería para el enrutamiento en aplicaciones React.
- `sass`: Preprocesador CSS para escribir estilos más fáciles de mantener.

### Dependencias de desarrollo:

- `@eslint/js`: Configuración de ESLint para proyectos de JavaScript.
- `@types/react`: Tipos de TypeScript para `react`.
- `@types/react-dom`: Tipos de TypeScript para `react-dom`.
- `@vitejs/plugin-react`: Plugin oficial de React para Vite.
- `eslint`: Herramienta para identificar y corregir problemas en el código.
- `eslint-plugin-react-hooks`: Linter para asegurar buenas prácticas con los hooks de React.
- `eslint-plugin-react-refresh`: Plugin de ESLint para habilitar la integración con React Fast Refresh.
- `globals`: Definiciones de variables globales para Node.js y el navegador.
- `typescript`: Compilador de TypeScript.
- `typescript-eslint`: Soporte de ESLint para TypeScript.
- `vite`: Bundler y servidor de desarrollo rápido para proyectos de frontend.

## Scripts

El archivo `package.json` incluye los siguientes scripts preconfigurados:

- `dev`: Inicia el servidor de desarrollo utilizando Vite.
- `build`: Ejecuta la compilación de TypeScript y luego construye el proyecto con Vite.
- `lint`: Ejecuta ESLint para verificar el código y detectar errores de estilo.
- `preview`: Muestra una vista previa del proyecto compilado usando Vite.

## Instalación

Para instalar las dependencias del proyecto, ejecuta:

```bash
npm install
```

## Configuración de TypeScript

Este proyecto está configurado para utilizar TypeScript. Asegúrate de tener un archivo `tsconfig.json` en la raíz del proyecto con las siguientes configuraciones mínimas:

```json
{
  "compilerOptions": {
    "target": "ESNext",
    "module": "ESNext",
    "moduleResolution": "node",
    "jsx": "react-jsx",
    "strict": true,
    "esModuleInterop": true,
    "skipLibCheck": true,
    "forceConsistentCasingInFileNames": true
  },
  "include": ["src/**/*"],
  "exclude": ["node_modules"]
}
```

## Configuración de ESLint

Este proyecto incluye ESLint para mantener la calidad del código. Asegúrate de tener el archivo `.eslintrc.json` configurado con las reglas que desees. Un ejemplo básico sería:

```json
{
  "extends": ["eslint:recommended", "plugin:react/recommended", "plugin:react-hooks/recommended"],
  "parserOptions": {
    "ecmaVersion": 2020,
    "sourceType": "module",
    "jsx": true
  },
  "plugins": ["react", "react-hooks"],
  "rules": {
    "react/react-in-jsx-scope": "off",
    "react/prop-types": "off"
  }
}
```

## Uso

1. Iniciar el servidor de desarrollo:

```bash
npm run dev
```

2. Construir el proyecto para producción:

```bash
npm run build
```

3. Ejecutar el proyecto en modo previsualización después de construirlo:

```bash
npm run preview
```

4. Ejecutar ESLint para verificar la calidad del código:

```bash
npm run lint
```

## Contribución

Si deseas contribuir a este proyecto, por favor abre un issue o envía un pull request.

## Licencia

Este proyecto está bajo la Licencia ISC. Consulta el archivo `LICENSE` para más detalles.