# 🚀 Getting started with Strapi CMS

Este proyecto es un CMS (Content Management System) basado en [Strapi](https://strapi.io), diseñado para gestionar contenido de manera eficiente y flexible. Incluye una estructura modular que permite la personalización y escalabilidad según las necesidades del negocio.

## 📂 Estructura del proyecto

El proyecto está organizado de la siguiente manera:

- **config/**: Contiene configuraciones clave del proyecto, como la base de datos, plugins, middlewares y el servidor.
- **database/**: Incluye las migraciones necesarias para la base de datos.
- **public/**: Archivos públicos como `robots.txt` y directorios de carga.
- **src/**: Código fuente principal del CMS, dividido en:
  - **admin/**: Configuración y personalización del panel de administración.
  - **api/**: Módulos de API organizados por entidades como `sales-point`, `sales-zone` y `seller-profile`. Cada módulo incluye:
    - **content-types/**: Esquemas de datos.
    - **controllers/**: Lógica de controladores.
    - **routes/**: Definición de rutas.
    - **services/**: Lógica de negocio.
  - **extensions/**: Extensiones personalizadas para ampliar la funcionalidad de Strapi.
- **types/**: Tipos generados automáticamente para garantizar la consistencia del código.

## 📋 Colecciones principales

Este CMS incluye las siguientes colecciones principales:

### 1. **Sales Point**

- **Descripción**: Representa los puntos de venta donde se realizan transacciones.
- **Campos principales**:
  - Nombre del punto de venta.
  - Ubicación.
  - Identificador único.
- **Funcionalidades**:
  - Gestión de puntos de venta.
  - API para crear, leer, actualizar y eliminar puntos de venta.

### 2. **Sales Zone**

- **Descripción**: Define las zonas de ventas asignadas a diferentes puntos de venta.
- **Campos principales**:
  - Nombre de la zona.
  - Región geográfica.
  - Relación con puntos de venta.
- **Funcionalidades**:
  - Gestión de zonas de ventas.
  - API para operaciones CRUD.

### 3. **Seller Profile**

- **Descripción**: Contiene información sobre los vendedores asociados a los puntos de venta.
- **Campos principales**:
  - Nombre del vendedor.
  - Información de contacto.
  - Relación con zonas de ventas.
- **Funcionalidades**:
  - Gestión de perfiles de vendedores.
  - API para operaciones CRUD.

## 🚀 Comandos principales

### `develop`

Inicia la aplicación Strapi con autoReload habilitado. [Aprende más](https://docs.strapi.io/dev-docs/cli#strapi-develop)

```bash
npm run develop
# o
yarn develop
```

### `start`

Inicia la aplicación Strapi con autoReload deshabilitado. [Aprende más](https://docs.strapi.io/dev-docs/cli#strapi-start)

```bash
npm run start
# o
yarn start
```

### `build`

Compila el panel de administración. [Aprende más](https://docs.strapi.io/dev-docs/cli#strapi-build)

```bash
npm run build
# o
yarn build
```

## ⚙️ Despliegue

Strapi ofrece múltiples opciones de despliegue, incluyendo [Strapi Cloud](https://cloud.strapi.io). Consulta la [documentación de despliegue](https://docs.strapi.io/dev-docs/deployment) para encontrar la mejor solución para tu caso de uso.

```bash
yarn strapi deploy
```

## 📚 Recursos adicionales

- [Centro de recursos](https://strapi.io/resource-center) - Centro de recursos de Strapi.
- [Documentación oficial](https://docs.strapi.io) - Documentación oficial de Strapi.
- [Tutoriales](https://strapi.io/tutorials) - Lista de tutoriales creados por el equipo y la comunidad.
- [Blog de Strapi](https://strapi.io/blog) - Blog oficial con artículos del equipo y la comunidad.
- [Changelog](https://strapi.io/changelog) - Actualizaciones del producto, nuevas características y mejoras generales.

## ✨ Comunidad

- [Discord](https://discord.strapi.io) - Únete a la comunidad de Strapi, incluyendo el equipo principal.
- [Foro](https://forum.strapi.io/) - Discute, haz preguntas, muestra tu proyecto y obtén retroalimentación.
- [Awesome Strapi](https://github.com/strapi/awesome-strapi) - Lista curada de recursos relacionados con Strapi.

---

<sub>🤫 Psst! [Strapi está contratando](https://strapi.io/careers).</sub>
