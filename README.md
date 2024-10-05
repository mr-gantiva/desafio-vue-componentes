# Proyecto Vue - Cédula de Identidad Chilena

Este es un proyecto de ejemplo utilizando Vue 3 para mostrar una representación visual de una cédula de identidad chilena. El proyecto incluye datos ficticios y usa imágenes como la bandera de Chile y la foto de una persona.

## Características

- Visualización de una cédula de identidad chilena.
- Animación de la cédula al cargar utilizando AOS (Animate On Scroll).
- Componentes y assets organizados dentro de carpetas.
- Estilos personalizados para la maquetación de la cédula.
  
## Tecnologías Utilizadas

- **Vue 3**: Framework frontend.
- **AOS (Animate On Scroll)**: Librería para añadir animaciones al desplazarse.
- **SCSS**: Preprocesador CSS para los estilos personalizados.
- **Assets**: Imágenes estáticas como la bandera de Chile y una foto.

## Demo

Puedes ver el demo en vivo aquí: [Ver Demo](https://mr-gantiva.github.io/desafio-vue-componentes/)



## Instalación

1. Clonar el repositorio:

    ```bash
    git clone https://github.com/tu-usuario/proyecto-cedula-vue.git
    ```

2. Instalar dependencias:

    ```bash
    npm install
    ```

3. Iniciar la aplicación:

    ```bash
    npm run serve
    ```

La aplicación estará disponible en `http://localhost:8080`.

## Estructura del Proyecto

- `components/datos.js`: Contiene los datos ficticios de la persona que se muestran en la cédula.
- `assets/chile_bandera.png`: Imagen de la bandera de Chile.
- `assets/foto_elon.jpg`: Imagen de la persona en la cédula.
- `App.vue`: El componente principal que incluye la estructura de la cédula.

## Captura de Pantalla

![Captura de la Cédula](./assets/screenshot.png)

## Personalización

Para cambiar los datos de la persona o las imágenes:

1. Modifica los datos en `components/datos.js`.
2. Sustituye las imágenes en la carpeta `assets`.

## Contribución

Las contribuciones son bienvenidas. Siéntete libre de abrir un *issue* o enviar un *pull request*.

## Licencia

Este proyecto está licenciado bajo la Licencia MIT.
