![Imagen del proyecto](https://github.com/eduardofierropro/SASS-y-SCSS-Aumenta-tu-nivel-como-Frontend/blob/main/assets/home1.png)

# SASS: Mixins, variables, Nesting Flex, Grid y Media Queries

Este es el repositorio de código sobre la serie de vídeos hablando sobre SASS y SCSS donde hemos hablado de:

* Variables 
* Mixins 
* Mixins como Neomorfismo, Flex o Media
* Crea tu propio Mixin 
* Anidación y Selector & 

Si te ha gustado o te ha servido coméntalo en un directo o sígueme por Twitch y Youtube 😊

[![Youtube](https://img.shields.io/static/v1?label=&message=ver%20playlist&color=FF0000&logo=youtube&logoColor=white&style=for-the-badge)](https://www.youtube.com/watch?v=-VJfeNL-VH0&list=PLJpymL0goBgFAUYDei7CoJCiHjcmgioUt)

## 💅 Todos los vídeos de SASS

| Nombre | Youtube |
|--|--|
|Variables en SASS|[![Youtube](https://img.shields.io/static/v1?label=&message=ver%20video&color=FF0000&logo=youtube&logoColor=white&style=for-the-badge)](https://youtu.be/eoAwVWeQf6U)|
|Mixins en SASS|[![Youtube](https://img.shields.io/static/v1?label=&message=ver%20video&color=FF0000&logo=youtube&logoColor=white&style=for-the-badge)](https://youtu.be/-VJfeNL-VH0)|
|Mixins MUY ÚTILES en SASS|[![Youtube](https://img.shields.io/static/v1?label=&message=ver%20video&color=FF0000&logo=youtube&logoColor=white&style=for-the-badge)](https://youtu.be/h3yS1RuIKz4)|
|Crea tu propio Mixin en SASS|[![Youtube](https://img.shields.io/static/v1?label=&message=ver%20video&color=FF0000&logo=youtube&logoColor=white&style=for-the-badge)](https://youtu.be/56QVDvj9dHw)|
|Anidación y Selector & en SASS|[![Youtube](https://img.shields.io/static/v1?label=&message=ver%20video&color=FF0000&logo=youtube&logoColor=white&style=for-the-badge)](https://youtu.be/56QVDvj9dHw)|

<!-- ## 👨🏻‍🏫 Apuntes de SASS

### ¿Qué es Sass vs CSS?
* CSS nos permite aplicar estilo al HTML
* SASS es un lenguaje que se convierte (compila) en CSS
* SCSS es un lenguaje que se convierte (compila) en CSS

Por lo tanto... ¿qué se entiende cuando decimos Sass?: **SASS es un lenguaje que se convierte *(compila)* en CSS**

### ¿Cómo se usa Sass?
Creas un archivo de SASS y lo conviertes *(compilas)* con herramientas.

### ¿Cómo se puede compilar Sass?
Puedes hacerlo de múltiples formas:
    
* Herramientas como Prepros 🚨 MUY FÁCIL 👉 [https://youtu.be/tArtLYlq9ws](https://youtu.be/tArtLYlq9ws)
* Consola con NodeJS
* Sistemas de Bundling como Webpack
* Sistemas de Task Runner como Grunt

#### ¿Cómo escribir variables en SASS?
Recuerda que :
* Declaramos(creamos) la variable
* Usamos la variable

>    🚨 Puedes ponerle el nombre que quieras pero usa "snake-case"
>    
>    🚨 Si no sabes de nomenclaturas 👉 https://youtu.be/lhEJkeCJ3As
 

```scss

$negro : red; // Declaramos la variable

a{
    color: $negro; // 👈 Usamos la variable en una propiedad
}
p{
    background-color: $negro; // 👈 Usamos la variable en una propiedad
}
```

### ¿Qué pasa si tengo muchas variables? 

```scss
$color-negro    : black;
$color-blanco   : white;
$fuente-normal  : Verdana;
$fuente-titulo  : Helvetica;
/* 👆 Aquí tenemos muchas variables y tenemos que repetir "color-", "fuente-" */

header{
    color       : $color-negro ;
    font-family   : $fuente-normal;
}
h1{
    background  : $color-blanco;
    font-family   : $fuente-titulo;
}
```

Vamos a ser organizados y guardar todas las variables en una lista de variables.
* Una lista de variables es un Array.
* Usaremos map-get() para usar las variables 
```scss
$colores: (
    "negro"  : black,
    "blanco" : white,
);
$fuentes : (
    "normal"  : Verdana,
    "titulo" : Helvetica
);

header{
    color         : map-get( $colores , "negro"  ) ;
    font-family   : map-get( $fuentes , "normal" ) ;
}
h1{
    background    : map-get( $colores , "blanco" ) ;
    font-family   : map-get( $fuentes , "titulo" ) ;
}

```

<!-- 
## 🔴 Vídeos relacionados con las metodologías

| Nombre | Youtube |
|--|--|
|Reset CSS: Teoría|[![Youtube](https://img.shields.io/static/v1?label=&message=ver%20video&color=FF0000&logo=youtube&logoColor=white&style=for-the-badge)](https://youtu.be/bXqPNoYFK8w)|
|Reset PRO: Código|[![Youtube](https://img.shields.io/static/v1?label=&message=ver%20video&color=FF0000&logo=youtube&logoColor=white&style=for-the-badge)](https://youtu.be/Foieq2jTajE)|
|Nomenclaturas CSS|[![Youtube](https://img.shields.io/static/v1?label=&message=ver%20video&color=FF0000&logo=youtube&logoColor=white&style=for-the-badge)](https://youtu.be/lhEJkeCJ3As)|
|Metodologías CSS|[![Youtube](https://img.shields.io/static/v1?label=&message=ver%20video&color=FF0000&logo=youtube&logoColor=white&style=for-the-badge)](https://youtu.be/f0LpZoyY1gE)|
|Arquitecturas CSS|[![Youtube](https://img.shields.io/static/v1?label=&message=ver%20video&color=FF0000&logo=youtube&logoColor=white&style=for-the-badge)](https://youtu.be/tUldrlfIGb4)|
|Cómo aplicar BEM en HTML y CSS|[![Youtube](https://img.shields.io/static/v1?label=&message=ver%20video&color=FF0000&logo=youtube&logoColor=white&style=for-the-badge)](https://youtu.be/NucZM0GMRi4)|
|Cómo aplicar SUITCSS en HTML y CSS|[![Youtube](https://img.shields.io/static/v1?label=&message=ver%20video&color=FF0000&logo=youtube&logoColor=white&style=for-the-badge)](https://youtu.be/Vdmof9VSiEo)| -->

 
## 💻 Otros repositorios y vídeos relacionados

En estos repositorios tendrás acceso a todas las versiones de cada módulo creadas con diferentes tecnologías como HTML, SCSS, TS, Angular, ReactJS...
Para que puedas practicar con un código básico.

| Nombre | Playlist | Repositorio | 
|--|--|--|
|Menú Responsive |[![Youtube](https://img.shields.io/static/v1?label=&message=ver%20en%20playlist&color=FF0000&logo=youtube&logoColor=white&style=for-the-badge)](https://www.youtube.com/playlist?list=PLJpymL0goBgFA5iTweWRejUhBP9TSSNnw)|[![github](https://img.shields.io/static/v1?label=&message=ver%20repo&color=171515&logo=github&logoColor=white&style=for-the-badge)](https://github.com/eduardofierropro/eduardofierropro-Como-crear-un-menu-hamburguesa-horizontal)|
<!-- |Slider con HTML, CSS y JS |[![Youtube](https://img.shields.io/static/v1?label=&message=ver%20en%20playlist&color=FF0000&logo=youtube&logoColor=white&style=for-the-badge)](XXXX)|[![github](https://img.shields.io/static/v1?label=&message=ver%20repo&color=171515&logo=github&logoColor=white&style=for-the-badge)](XXXX)|
|Carrousel con HTML, CSS y JS |[![Youtube](https://img.shields.io/static/v1?label=&message=ver%20en%20playlist&color=FF0000&logo=youtube&logoColor=white&style=for-the-badge)](XXXX)|[![github](https://img.shields.io/static/v1?label=&message=ver%20repo&color=171515&logo=github&logoColor=white&style=for-the-badge)](XXXX)|
|Lightbox con HTML, CSS y JS |[![Youtube](https://img.shields.io/static/v1?label=&message=ver%20en%20playlist&color=FF0000&logo=youtube&logoColor=white&style=for-the-badge)](XXXX)|[![github](https://img.shields.io/static/v1?label=&message=ver%20repo&color=171515&logo=github&logoColor=white&style=for-the-badge)](XXXX)| -->

## 👨🏻‍🏫 Eduardo Fierro Pro
 
¡Qué pasa cruck! Soy profesor de programación tanto en escuelas como en Bootcamps y en mis tiempos libres programo por Twitch y en Youtube.

[![Youtube](https://img.shields.io/static/v1?label=&message=youtube&color=FF0000&logo=youtube&logoColor=white&style=for-the-badge)](https://youtube.com/EduardoFierroPro?sub_confirmation=1)
[![twitch](https://img.shields.io/static/v1?label=&message=twitch&color=6441a5&logo=twitch&logoColor=white&style=for-the-badge)](https://twitch.tv/eduardofierropro)
[![tiktok](https://img.shields.io/static/v1?label=&message=tiktok&color=ff0050&logo=tiktok&logoColor=white&style=for-the-badge)](https://www.tiktok.com/@eduardofierro.pro?)
[![instagram](https://img.shields.io/static/v1?label=&message=instagram&color=5B51D8&logo=instagram&logoColor=white&style=for-the-badge)](https://instagram.com/eduardofierro.pro)
[![linkedin](https://img.shields.io/static/v1?label=&message=linkedin&color=0e76a8&logo=linkedin&logoColor=white&style=for-the-badge)](https://www.linkedin.com/in/eduardofierropro)
[![discord](https://img.shields.io/static/v1?label=&message=discord&color=7289da&logo=discord&logoColor=white&style=for-the-badge)](https://discord.gg/t4Txush)
[![twitter](https://img.shields.io/static/v1?label=&message=twitter&color=1DA1F2&logo=twitter&logoColor=white&style=for-the-badge)](https://twitter.com/edfierropro)
[![github](https://img.shields.io/static/v1?label=&message=github&color=171515&logo=github&logoColor=white&style=for-the-badge)](https://github.com/eduardofierropro)
[![colaboración](https://img.shields.io/static/v1?label=&message=MIS%20CURSOS&color=blue&logo=teach&logoColor=white&style=for-the-badge)](http://colaboracion.eduardofierro.pro)


## 📄 Licencia 

MIT Public License v3.0
No puede usarse comercialmente
