# 🔖 Strapi Tienda de Guitarras

Se utilizo strapi para facilitar la parte de desarrollo del backend. Para usar en proyecto de [remix.js](https://github.com/josmova/TiendaGuitarrasBasicRemixJs) y [next.js](https://github.com/josmova/TiendaGuitarrasBasicNextJs) en frontend.

Aquí pequeña información de que es strapi:
Strapi es el principal CMS sin interfaz de código abierto. Es 100% JavaScript y totalmente personalizable. Strapi es un CMS sin cabeza de código abierto que brinda a los desarrolladores la libertad de elegir sus herramientas y marcos favoritos y permite a los editores administrar y distribuir su contenido utilizando el panel de administración de su aplicación.

Para más informaición de: [strapi](https://strapi.io/)

## 📃 Tecnologías Utilizadas

| Tecnología                           | Versión |
| :----------------------------------- | :------ |
| `strapi`                             | 4.4.5   |
| `@strapi/provider-upload-cloudinary` | 4.4.5   |

## 📖 Características

- **Crear tablas** Se crean las tabals de forma gráfica
- **Agregar contenido** Poder Crear contenido
- **Manejar Roles** Roles y permisos apra creación de tablas, contenido y etc.
- **Nota** Se pueden hacer muchas cosas de manera fácil, ver documentación de strapi.
- **Cloudinary:** Se almacenan las imágenes

📇 Se puede ver algunas imagenes de ejemplo

![Strapi-Login](/public/img/login.png)
![Strapi-TablaGuitarras](/public/img/ContentTypeGuitar.png)
![Strapi-TablaPost](/public/img/ContentTypePost.png)
![Strapi-ContenidoGuistarras](/public/img/ContentGuitar.png)
![Strapi-ContenidoPost](/public/img/ContentPost.png)

## 🚀 Comenzando

Este proyecto se realizo como backend para los siguientes proyectos:

**Tienda de Guitarras Basic con Next.js**

- [TiendaGuitarrasBasicNextJs](https://github.com/josmova/TiendaGuitarrasBasicNextJs)

**Tienda de Guitarras Basic con Remix.js**

- [TiendaGuitarrasBasicRemixJs](https://github.com/josmova/TiendaGuitarrasBasicRemixJs)

La configuración de la DB se uso postgreSQL y debes configurar el archivo **database.js**, que se encuentra en la carpeta **config**

```JavaScript
module.exports = ({ env }) => ({
  connection: {
    client: "postgres",
    connection: {
      host: env("DATABASE_HOST", "127.0.0.1"),
      port: env.int("DATABASE_PORT", 5432),
      database: env("DATABASE_NAME", "DATABASE"),
      user: env("DATABASE_USERNAME", "USER"),
      password: env("DATABASE_PASSWORD", "PASSWORD"),
      ssl: env.bool("DATABASE_SSL", false),
    },
  },
});

```

> **Nota:** Se requiere una cuenta en [**Cloudinary**](https://cloudinary.com/)

Aquí en el siguiente archivo **.env** que son la variables de entorno poner sus claves:

```
CLOUDINARY_NAME="CLOUDINARY_NAME"
CLOUDINARY_KEY="CLOUDINARY_KEY"
CLOUDINARY_SECRET="CLOUDINARY_SECRET"
```

## 👩‍💻 Instalación

Instalacións StrapiBasico-TiendaGuitarras con npm:

```bash
  cd strapibasico-tiendaguitarras
  npm install
```

Luego ejecutar el siguiente comando:

```bash
  npm run develop
```

## 📋 Documentación

-Para más informaición de: [strapi](https://strapi.io/)

-Para más informaición de: [@strapi/provider-upload-cloudinary](https://strapi.io/)

## 👽 Autor

[![portfolio](https://img.shields.io/badge/Mi_portafolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://josemontiel.netlify.app/)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/josemontielmv/)

> @Josmova ( Jose Montiel )
