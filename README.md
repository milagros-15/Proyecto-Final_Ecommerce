# Proyecto Final: Ecommerce (FullStack)
--Sabrina

Sabrina es una aplicación full-stack completa para comprar ropa en línea. Con una interfaz intuitiva y amigable, los usuarios pueden navegar y buscar sus productos favoritos fácilmente. Además, tienen la opción de aplicar filtros para una búsqueda más específica y eficiente. La aplicación cuenta con 25 páginas, que incluyen las fundamentales como Inicio, Productos con un catálogo de productos, Carrito y un exclusivo Panel de Control (Dashboard) accesible solo para administradores. El Panel de Control brinda acceso a diversas estadísticas, tablas de pedidos, productos y usuarios, permitiendo a los administradores realizar operaciones como eliminación, actualización y creación.


--Características
* Disfruta de un diseño fluido e intuitivo que mejora la experiencia de compra para los usuarios.
* Explora una extensa gama de productos en distintas categorías.
* Encuentra fácilmente tus productos favoritos utilizando filtros de búsqueda avanzados, haciendo que el proceso de compra sea eficiente y placentero.
* Experimenta un proceso de pago sin complicaciones con pasos claros y fáciles de seguir, garantizando una transacción fluida.
* Completa transacciones de forma fluida con métodos de pago integrados como PayPal y MercadoPago, brindando a los usuarios flexibilidad y comodidad.
* Obtén acceso exclusivo a un panel de control integral con estadísticas detalladas, tablas y herramientas de gestión para pedidos, productos y usuarios.
* Benefíciese de un sólido sistema de autenticación de usuarios con seguridad basada en tokens, garantizando la protección de los datos del usuario.
* Refuerza la seguridad del usuario con la verificación por correo electrónico, añadiendo una capa adicional de autenticidad al proceso de registro.
* Experimenta tranquilidad con la función de recuperación de contraseña. Los usuarios pueden restaurar o restablecer fácilmente sus contraseñas a través de un correo electrónico seguro enviado por la aplicación, garantizando un proceso de recuperación sin problemas.
* La aplicación utiliza Cloudinary para el almacenamiento en la nube de las imágenes de los productos.
Disfruta de un diseño responsive que se adapta a diferentes dispositivos, brindando una experiencia óptima en computadoras de escritorio, tabletas y dispositivos móviles.


--Tecnologías utilizadas

Backend
* Node.js: Un entorno de ejecución para llevar a cabo código JavaScript en el servidor.
* Express: Un framework para Node.js que simplifica la creación de APIs sólidas.
* Express Async Handler: Una utilidad para manejar excepciones en los controladores de rutas asíncronas.
* MongoDB: Una base de datos NoSQL basada en un modelo de datos de documentos utilizada para almacenar y recuperar datos.
* Mongoose: Una biblioteca ODM (Mapeo de Datos de Objetos) para MongoDB y Node.js.
* Mongoose Paginate: Soporte de paginación para Mongoose.
* Dotenv: Un módulo sin dependencias para cargar variables de entorno.
* Bcryptjs: Una biblioteca para cifrar contraseñas.
* JWT: Una biblioteca para generar y verificar Tokens Web JSON (JWT).
* NodeMailer: Una biblioteca de Node.js para enviar correos electrónicos.
* Cors: Middleware para habilitar el intercambio de recursos entre distintos orígenes (CORS) en aplicaciones Express.
* Multer: Middleware para el manejo de datos de form/multipart, utilizado en la aplicación para cargar archivos de imágenes.
* Cloudinary: Servicio basado en la nube para gestionar y distribuir imágenes y videos.
* MercadoPago: Integración para manejar pagos utilizando Mercado Pago.

Frontend
* React: Una biblioteca de JavaScript para crear interfaces de usuario interactivas.
* TypeScript: Un superconjunto de JavaScript que agrega tipos estáticos y otras funciones a la sintaxis del lenguaje.
* Sass: Un preprocesador de CSS que proporciona funciones adicionales y una sintaxis más legible.
* Axios: Una biblioteca popular para realizar solicitudes HTTP.
* ReactQuery: Biblioteca versátil que simplifica la gestión, almacenamiento en caché, sincronización y actualización de datos asíncronos. Solución esencial para la obtención de datos en aplicaciones web, agilizando el proceso de manejo del estado del servidor con facilidad.
* ChartJs: Biblioteca de JavaScript que facilita la creación de gráficos interactivos y visualmente atractivos.
* Redux: Un contenedor de estado predecible para gestionar el estado de una aplicación JavaScript.
* React Router Dom: Es una biblioteca para la navegación declarativa y dinámica en aplicaciones React, que permite gestionar rutas y vistas de manera eficiente.
* React Toastify: Es una biblioteca que facilita la creación de notificaciones interactivas y personalizables para React.
* React Helmet Async: Es una biblioteca de React que te permite gestionar de manera fácil y dinámica los elementos del encabezado del documento (head), como títulos, metaetiquetas y otros elementos, de forma asíncrona para mejorar el rendimiento de la aplicación.
* React Infinite Scroll Component: Es un componente de React que facilita la implementación del desplazamiento infinito, cargando automáticamente más contenido a medida que el usuario se acerca al final de la página.
* Swiper: Biblioteca de deslizadores táctiles, diseñada para crear experiencias de desplazamiento suaves y receptivas en interfaces de usuario.
* Material UI: Un popular framework de interfaz de usuario (UI) para React basado en los principios de Material Design.
* PayPal: Integración oficial de PayPal para React.


--Estructura del proyecto

Backend
* src/controllers: Dentro de este directorio, encontrarás los controladores responsables de manejar la lógica empresarial y las operaciones relacionadas con diferentes recursos. Por ejemplo, product.controller.ts, order.controller.ts y user.controller.ts.
* src/data: Contiene archivos de datos utilizados en la aplicación, como productos y usuarios de ejemplo.
* src/models: Este directorio contiene los modelos que definen las estructuras de datos utilizadas dentro del backend. Cada archivo de modelo, como orderModel.ts, productModel.ts, userModel.ts y request.ts, describe la estructura y propiedades de diferentes entidades de datos.
* src/routes: Contiene archivos que definen las rutas de la API y sus controladores correspondientes.
* src/utilities: Contiene utilidades y funciones auxiliares utilizadas en la aplicación.

Frontend
* src/assets: Contiene activos estáticos como imágenes e iconos utilizados en la aplicación.
* src/components: Contiene componentes reutilizables utilizados en diferentes partes de la aplicación.
* src/hooks: Contiene hooks personalizados responsables de encapsular y gestionar lógica compleja utilizada en varias secciones. Los hooks están estratégicamente divididos en tres archivos separados:
      * userHooks.ts: Este archivo incluye hooks personalizados relacionados con funcionalidades relacionadas con el usuario. Encapsula lógica como autenticación de usuario, registro y cualquier otra operación específica del usuario.

      * productHooks.ts: Este archivo contiene hooks relacionados con funcionalidades relacionadas con productos. Puede incluir lógica para recuperar, crear, actualizar o eliminar datos de productos.

      * orderHooks.ts: Este archivo contiene hooks relacionados con funcionalidades relacionadas con pedidos. Esto puede incluir lógica para recuperar el historial de pedidos, crear nuevos pedidos, eliminar o actualizar los existentes.

* src/models: Contiene interfaces o tipos de TypeScript utilizados para definir estructuras de datos.
* src/pages: Contiene todas las páginas dentro de la aplicación. Cada página tiene su carpeta dedicada con el mismo nombre, la cual tiene su archivo correspondiente (.tsx) y posiblemente directorios adicionales, como una carpeta "components" que contiene componentes utilizados solo en esa página.
* src/redux: Este directorio está dedicado a gestionar los estados y reductores de la aplicación mediante Redux.
* src/services: El directorio de servicios encapsula archivos esenciales de servicio, como apiClient.ts, que es responsable de interactuar con la API del backend. Es el se configura Axios para realizar solicitudes HTTP al servidor correspondiente (local durante el desarrollo o el servidor implementado en producción). Además, incluye un interceptor para adjuntar el token de autorización del usuario a los encabezados de las solicitudes salientes si el usuario está autenticado.
* src/styles: Contiene archivos de estilo Sass para cada página de la aplicación. La mayoría de las páginas tienen su propio archivo Sass, excepto en casos donde los estilos son compartidos (por ejemplo, LoginPage.tsx y RegisterPage.tsx comparten AuthenticatedPages.scss).
* src/utilities: Contiene utilidades y funciones auxiliares utilizadas en la aplicación.
