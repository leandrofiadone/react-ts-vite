# Guía para Configurar una Aplicación Full-Stack con TypeScript, React y Node.js

Esta guía explica los pasos para configurar tanto el frontend como el backend de una aplicación Full-Stack con TypeScript, React y Node.js.

## TS-React-Vite-Front-Boilerplate

1. **Crear la estructura del proyecto**:
   - `mkdir FullStackTS-GoogleAuth && cd FullStackTS-GoogleAuth && mkdir TS-Login-Front TS-Login-Back`

2. **Instalar React con Vite y TypeScript**:
   - `cd TS-Login-Front && npm create vite@latest . -- --template react-ts`
   - Esto configura un proyecto React con TypeScript usando Vite.

3. **Instalar dependencias adicionales**:
   - `npm install react-router-dom axios sass`
   - `npm install @types/react-router-dom`
   - Instala enrutamiento (`react-router-dom`), peticiones HTTP (`axios`), estilos (`sass`) y tipos para `react-router-dom`.