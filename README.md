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
Captura de Pantalla
[url=https://postimg.cc/Lqgr2WJ7][img]https://i.postimg.cc/Lqgr2WJ7/Telefono-1.jpg[/img][/url]
[url=https://postimg.cc/G45W0RmG][img]https://i.postimg.cc/G45W0RmG/Telefono-2.jpg[/img][/url]
[url=https://postimg.cc/VJ6xHvmz][img]https://i.postimg.cc/VJ6xHvmz/Telefono-3.jpg[/img][/url]
### 2. Tablet (ancho entre 601px y 1024px)
```css
@media only screen and (min-width: 601px) and (max-width: 1024px) {
    .logo {
        height: 60px;
        padding-left: 56px; 
    }
    .row {
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
    }

    .card {
        width: 100; 
        margin-bottom: 20px; 
    }
}
```
Captura de Pantalla
[url=https://postimg.cc/14018bv1][img]https://i.postimg.cc/14018bv1/Tablet.jpg[/img][/url]

###3.Computadoras de Escritorio

Captura de Pantalla
[url=https://postimg.cc/s1zDHY8y][img]https://i.postimg.cc/s1zDHY8y/Escritorio-1.jpg[/img][/url]
[url=https://postimg.cc/YGcT9xgS][img]https://i.postimg.cc/YGcT9xgS/Escritorio-2.jpg[/img][/url]
