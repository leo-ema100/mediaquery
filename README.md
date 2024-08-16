# Documentación de Media Queries y Diseño Responsivo

Este proyecto implementa un diseño web responsivo utilizando media queries en CSS. El diseño se adapta a diferentes tamaños de pantalla, proporcionando una experiencia de usuario optimizada en dispositivos móviles, tabletas y computadoras de escritorio.

## Estructura de la Página

1. *Encabezado (Header)* :
   - Incluye un logotipo y un menú de navegación.
   - El logotipo está ubicado a la izquierda y el menú de navegación a la derecha en pantallas grandes.
   - Para dispositivos moviles o Tablet cuenta con menú de navegación de hamburguesa y a la par el logo.

2. *Bloque de Contenido Principal (Main)* :
   - Contiene un título y un párrafo de introducción.
   - El contenido está centrado y se ajusta según el tamaño de la pantalla.

3. *Sección de Tarjetas de Contenido (Section)* :
   - Tres tarjetas que contienen informacion de personajes del videojuego Valorant.
   - Las tarjetas se organizan en columnas que varían según el dispositivo.

4. *Pie de Página (Footer)* :
   - Contiene enlaces a redes sociales de Valorant.

## Media Queries Implementadas

Estos codigos se encuentran en el archivo css, utilizando como Framework Materialize gracias a esto muchos elementos ya estén optimizados para adaptarse automáticamente a pantallas pequeñas sin necesidad de muchas modificaciones adicionales. Por tal razon en el meda queries para Móvil solo se modifico el logo, pero para Tablet se modifico otras opciones.

### 1. Móviles (ancho máximo de 600px):

```css
@media only screen and (max-width: 600px) {
    .logo {
        height: 50px;
        padding-left: 56px; 
    }
}
```
- Captura de Pantalla

![Telefono 1](https://github.com/user-attachments/assets/c5ad3f02-f00d-44f5-9d9e-d3a028b011fc)

![Telefono 2](https://github.com/user-attachments/assets/fb27c838-4ee4-4ca5-883c-ed16a9be2cc6)

![Telefono 3](https://github.com/user-attachments/assets/e8b72748-e5b5-4982-9c8c-2a39bc8364c8)

### 2. Tablet (ancho entre 601px y 1024):

```css
@media only screen and (min-width: 601px) and (max-width: 1024px) {
    .logo {
        height: 60px;
        padding-left: 56px; 
    }
    .row {
        display: flex;
        flex-wrap: wrap;
        flex-flow: row wrap;
        justify-content: space-between;
    }
    .col {
        flex: 0 0 calc(60% - 20px);
        max-width: calc(50% - 10px);
        margin-bottom: 40px;
    }

    h1 {
        font-size: 250%
    }

    p {
        font-size: 120%
    }

    h2 {
        font-size: 230%;
    }
}
```
- Captura de Pantalla

![image](https://github.com/user-attachments/assets/97cd90c2-0d65-4ede-8dd1-2e5f09583596)
![image](https://github.com/user-attachments/assets/307af218-124a-486a-9403-555d1c8aa7bc)

### 3. Computadoras de Escritorio

- Captura de Pantalla
![Escritorio 1](https://github.com/user-attachments/assets/1c18d96d-2e5c-48b0-a39e-1458c5d03ddd)
![Escritorio 2](https://github.com/user-attachments/assets/7cf5d000-55d2-421a-8688-e247960658d1)
