# Fundamentos

Aprendamos a trabajar con Bootstrap 5! realizando proyectos 🐱‍👤

## ¿Qué vamos a crear?

- [https://bootstrap-5-bluuweb.netlify.app/](https://bootstrap-5-bluuweb.netlify.app/)
- [Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7)

## Requisitos

- [Curso Fundamentos de HTML y CSS](https://www.youtube.com/watch?v=rr2H086z16s&list=PLPl81lqbj-4LKo66cEts5yC_AjOvqKptm)

## Viaja en el tiempo

En la descripción de video (Youtube) encontrarás el temario, si pinchas en los minutos podrás adelantar o retroceder el video 📺

## ¿Para qué sirve?

Bootstrap es una herramienta de trabajo para desarrolladores Front-end, contiene un conjunto de estilos CSS y script JS para desarrollar web a la velocidad de la luz.

<u>Caracteristicas:</u>

- Mobile First
- Compatibilidad con Sass
- Grid responsive
- Componentes (navbar, card, botones, etc) [Revisar aquí](https://getbootstrap.com/docs/5.0/getting-started/introduction/)
- Javascript plugins

## ¿La pregunta del millón?

- ¿Es recomendable aprender Bootstrap 5?
  Si necesitamos crear prototipos rápidos, hacer sitios web responsives visualmente decentes, es una buena alternativa. Sobretodo para los amantes de Javascript es una solución rápida a los diseños web.

## Desventajas, pero...

- <b>¿Con Bootstrap todos los sitios web son iguales?</b><br>
  Si utilizamos todos sus clases sin modificar nada, se verán todos nuestros proyectos parecidos, pero actualmente en la versión 5 es super sencillo personalizar los estilos, utilizando Sass. Si revisamos el proyecto a realizar, cambiamos los colores y tipografía 👏🏼

- <b>¿Mi CSS serán 60.000 líneas de código?</b><br>
  Si no optimizas Bootstrap se generará un archivo enorme, pero actualmente existe "purgecss" que nos ayuda a eliminar las clases CSS que no utilizamos. En el proyecto que realizaremos utilizaremos <b>menos de 400 líneas de CSS 😮</b>

- <b>¿Es difícil aprender Bootstrap 5?</b><br>
  Jugaremos al memorice... solo es cosa de aprende sus clases y ya. A medida que realizamos proyectos verás lo fácil de su implementación 😎

- <b>¿Diseños complejos se pueden realizar?</b><br>
  Con vanilla Bootstrap 5 se puede complicar la cosa si necesitamos un diseño altamente complejo, pero no está limitado a que puedas agregar tus propios estilos en CSS. En la práctica de hoy agregaremos nuestros propios estilos 🎉

- <b>¿Más deventajas?</b><br>
  Comparte tus opiniones (con amor y respeto 💙) en la caja de comentarios de Youtube, realizaré otro video leyendo todas sus sugerencias y dudas 🙌

## Herramientas

- [https://code.visualstudio.com/](https://code.visualstudio.com/)
- [https://nodejs.org/es/](https://nodejs.org/es/)
- [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)
- [Live Sass Compiler](https://marketplace.visualstudio.com/items?itemName=ritwickdey.live-sass)
- [Tema e iconos VSC](https://marketplace.visualstudio.com/items?itemName=sldobri.bunker)

## CDN

- [CDN](https://getbootstrap.com/docs/5.0/getting-started/introduction/)

La manera más sencilla de comenzar con Bootstrap es utilizar el CDN. Los archivos están alojados en un servidor externo.

```html
<link
  href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.0-beta1/dist/css/bootstrap.min.css"
  rel="stylesheet"
  integrity="sha384-giJF6kkoqNQ00vy+HMDP7azOuL0xtbfIcaT9wjKHr8RbDVddVHyTfAAsrekwKmP1"
  crossorigin="anonymous"
/>
```

## Breakpoints

- [breakpoints](https://getbootstrap.com/docs/5.0/layout/breakpoints/)

Hace referencia a los puntos de interrupción, dependiendo del tamaño del dispositivo que esté visitando nuestro sitio web.

## Container

- [containers](https://getbootstrap.com/docs/5.0/layout/containers/)

Se utiliza para alinear nuestro contenido, estableciendo un ancho determinado.

::: warning Importante
Al utilizar el sistema de columnas es necesario envolver todo en un container
:::

## Grid

- [grid](https://getbootstrap.com/docs/5.0/layout/grid/)

Bootstrap utiliza un sistema de 12 columnas (con Flexbox) para diseñar y distribuir elementos en su sitio web.

```html
<!DOCTYPE html>
<html lang="es">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Grid Fundamentos</title>
    <link
      href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.0-beta1/dist/css/bootstrap.min.css"
      rel="stylesheet"
      integrity="sha384-giJF6kkoqNQ00vy+HMDP7azOuL0xtbfIcaT9wjKHr8RbDVddVHyTfAAsrekwKmP1"
      crossorigin="anonymous"
    />
  </head>
  <body>
    <div class="container">
      <div class="row">
        <div class="col-1 border">1</div>
        <div class="col-1 border">1</div>
        <div class="col-1 border">1</div>
        <div class="col-1 border">1</div>
        <div class="col-1 border">1</div>
        <div class="col-1 border">1</div>
        <div class="col-1 border">1</div>
        <div class="col-1 border">1</div>
        <div class="col-1 border">1</div>
        <div class="col-1 border">1</div>
        <div class="col-1 border">1</div>
        <div class="col-1 border">1</div>
      </div>
    </div>
  </body>
</html>
```

Por ejemplo si necesitamos crear 3 columnas:

```html
<div class="row">
  <div class="col-4 border">4</div>
  <div class="col-4 border">4</div>
  <div class="col-4 border">4</div>
</div>
```

Si necesitamos 4 columnas:

```html
<div class="row">
  <div class="col-3 border">3</div>
  <div class="col-3 border">3</div>
  <div class="col-3 border">3</div>
  <div class="col-3 border">3</div>
</div>
```

Diferentes tamaños:

```html
<div class="row">
  <div class="col-6 border">6</div>
  <div class="col-3 border">3</div>
  <div class="col-3 border">3</div>
</div>
```

## Grid Responsive

La gracia es hacer sitios web responsives, y la gracia mayor es que con Bootstrap es muy sencillo.

[Breakpoint](https://getbootstrap.com/docs/5.0/layout/grid/#grid-options)

Agregando las opciones a la grid, podemos crear diseños responsives:

```html
<div class="row">
  <div class="col-12 col-sm-6 col-md-4 border">12 sm-6 md-4</div>
  <div class="col-12 col-sm-6 col-md-4 border">12 sm-6 md-4</div>
  <div class="col-12 col-sm-12 col-md-4 border">12 sm-6 md-4</div>
</div>
```

## Práctica

Teniendo en mente nuestro diseño final: [ver ejemplo](https://bootstrap-5-bluuweb.netlify.app/) Realizemos su estructura:

```html
<div class="container">
  <div class="row">
    <!-- Columna principal izquierda -->
    <div class="col-12 col-lg-9 bg-primary">
      <p>
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. Iusto ipsa
        quos fuga alias eligendi rerum neque? Sed in dolorem ratione numquam,
        magnam optio? Fugiat cum omnis, ipsum vel totam suscipit.
      </p>
    </div>

    <!-- Columna principal derecha -->
    <div class="col-12 col-lg-3 bg-secondary">
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Fuga eos
        voluptate dolorum sunt qui ipsa earum vel corrupti, dolorem, quidem
        temporibus placeat autem consectetur eaque sequi inventore! Eius,
        tenetur culpa.
      </p>
    </div>
  </div>
</div>
```

En el interior de la columna principal izquierda, creamos otros sistema de columnas.

```html
<!-- Columna principal izquierda -->
<div class="col-12 col-lg-9">
  <div class="row">
    <div class="col-12 col-lg-8 bg-success">
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Praesentium
        tempore unde voluptatum velit at, dolores iusto nesciunt exercitationem!
        Error porro iusto eius nam eligendi quod consequuntur asperiores aperiam
        aliquam cumque?
      </p>
    </div>
    <div class="col-12 col-lg-4 bg-primary">
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Omnis quasi
        ipsum tenetur dolorem dolor, fugiat enim libero nobis perferendis esse
        inventore, odit eveniet consectetur incidunt repellendus ab molestias
        sint adipisci.
      </p>
    </div>
    <div class="col-12 col-lg-4 bg-warning">
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Vel dolorum
        odit quas, fugit ea sunt veritatis commodi inventore omnis hic! Rerum
        similique voluptates aut esse repellendus perspiciatis? Molestias,
        reprehenderit aliquid?
      </p>
    </div>
    <div class="col-12 col-lg-8 bg-danger">
      <p>
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Nulla
        obcaecati deleniti quo repellat earum in accusantium veniam. Delectus
        iste dicta exercitationem. Impedit dolor, animi minima aperiam maiores
        illum est tempore?
      </p>
    </div>
  </div>
</div>
```

## Flexbox

- No sabes nada de Flexbox? [Aquí un tutorial](https://www.youtube.com/watch?v=TtgkU8LMGAc)
- [utilities/flex/](https://getbootstrap.com/docs/5.0/utilities/flex/)
- [utilities/sizing](https://getbootstrap.com/docs/5.0/utilities/sizing/)
- [min-width](https://getbootstrap.com/docs/5.0/layout/breakpoints/#min-width)

```html
<!DOCTYPE html>
<html lang="es">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Grid Fundamentos</title>
    <link
      href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.0-beta1/dist/css/bootstrap.min.css"
      rel="stylesheet"
      integrity="sha384-giJF6kkoqNQ00vy+HMDP7azOuL0xtbfIcaT9wjKHr8RbDVddVHyTfAAsrekwKmP1"
      crossorigin="anonymous"
    />

    <style>
    /* https://getbootstrap.com/docs/5.0/layout/breakpoints/#min-width */
      @media (min-width: 992px) {
        .alto-100 {
          height: 100vh;
        }
      }
    </style>
  </head>
  <body>
    <main
      class="container alto-100 bg-dark d-flex justify-content-center align-items-center"
    >
      <div class="row">
        <div class="col-12 col-lg-9">
          <div class="row">
            <div class="col-12 col-lg-8 bg-success">
              <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit.
                Praesentium tempore unde voluptatum velit at, dolores iusto
                nesciunt exercitationem! Error porro iusto eius nam eligendi
                quod consequuntur asperiores aperiam aliquam cumque?
              </p>
            </div>
            <div class="col-12 col-lg-4 bg-primary">
              <p>
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Omnis
                quasi ipsum tenetur dolorem dolor, fugiat enim libero nobis
                perferendis esse inventore, odit eveniet consectetur incidunt
                repellendus ab molestias sint adipisci.
              </p>
            </div>
            <div class="col-12 col-lg-4 bg-warning">
              <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Vel
                dolorum odit quas, fugit ea sunt veritatis commodi inventore
                omnis hic! Rerum similique voluptates aut esse repellendus
                perspiciatis? Molestias, reprehenderit aliquid?
              </p>
            </div>
            <div class="col-12 col-lg-8 bg-danger">
              <p>
                Lorem ipsum, dolor sit amet consectetur adipisicing elit. Nulla
                obcaecati deleniti quo repellat earum in accusantium veniam.
                Delectus iste dicta exercitationem. Impedit dolor, animi minima
                aperiam maiores illum est tempore?
              </p>
            </div>
          </div>
        </div>

        <div class="col-12 col-lg-3 bg-secondary">
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Fuga eos
            voluptate dolorum sunt qui ipsa earum vel corrupti, dolorem, quidem
            temporibus placeat autem consectetur eaque sequi inventore! Eius,
            tenetur culpa.
          </p>
        </div>
      </div>
    </main>
  </body>
</html>
```

## Card

- [components/card/](https://getbootstrap.com/docs/5.0/components/card/)
- [utilities/shadows/](https://getbootstrap.com/docs/5.0/utilities/shadows/)
- [utilities/spacing](https://getbootstrap.com/docs/5.0/utilities/spacing/#margin-and-padding)
- [utilities/borders](https://getbootstrap.com/docs/5.0/utilities/borders/)
- [utilities/colors](https://getbootstrap.com/docs/5.0/utilities/colors/)
- [content/typography](https://getbootstrap.com/docs/5.0/content/typography/)
- [utilities/text](https://getbootstrap.com/docs/5.0/utilities/text/)

Copiamos esto por cada Card y fijarse en la altura de ellas, como son diferentes todos los elementos agregamos `h-100`

```html
<article class="card shadow bg-success h-100">
  <div class="card-body">
    <div class="d-flex align-items-center mb-3">
      <img
        src="./images/image-daniel.jpg"
        alt=""
        class="rounded-circle border border-3 border-secondary"
      />
      <div class="ps-3">
        <h3 class="m-0 text-white h6">Daniel Clifford</h3>
        <p class="m-0 h6">lorem ipsum</p>
      </div>
    </div>
    <p class="text-white h6">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Eaque iusto
      voluptatibus quaerat? Eveniet, itaque ab cum voluptate non doloribus
      inventore ullam quos aperiam illo harum maiores? Ab dolorum eveniet
      deserunt.
    </p>
    <p class="text-dark fs-6 lh-1">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Necessitatibus,
      vero repellat! Quae, minima dolore laborum aut dolor nobis. Ducimus ipsam
      atque sint illo in excepturi aliquam minus tenetur odio distinctio.
    </p>
  </div>
</article>
```

Cambiando los fondos y agregando padding iguales `p-2`

```html
<body class="bg-secondary">
    <main class="container alto-100 d-flex justify-content-center align-items-center">
        
        <div class="row">

            <div class="col-12 col-lg-9"> 
                
                <div class="row">
                    <div class="col-12 col-lg-8 p-2">
                        <article class="card shadow bg-primary h-100">
                            ...
                        </article>
                    </div>
                    <div class="col-12 col-lg-4 p-2">
                        <article class="card shadow bg-success h-100">
                            ...
                        </article>
                    </div>
                    <div class="col-12 col-lg-4 p-2">
                        <article class="card shadow bg-light h-100">
                            ...
                        </article>
                    </div>
                    <div class="col-12 col-lg-8 p-2">
                        <article class="card shadow bg-dark h-100">
                            ...
                        </article>
                    </div>
                </div>
                
            </div>

            <div class="col-12 col-lg-3 p-2">
                <article class="card shadow bg-light h-100">
                    ...
                </article>
            </div>

        </div>

    </main>
</body>
```

## Personalización (Avanzado)
- Recomendable conocer los fundamentos de node.js [Tutorial aquí](https://www.youtube.com/watch?v=mG4U9t5nWG8&list=PLPl81lqbj-4IEnmCXEJeEXPepr8gWtsl6)
- [https://nodejs.org/es/](https://nodejs.org/es/)
- [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)
- [Live Sass Compiler](https://marketplace.visualstudio.com/items?itemName=ritwickdey.live-sass)

package.json
```
npm init -y
```

- [download](https://getbootstrap.com/docs/5.0/getting-started/download/)

```
npm install bootstrap@next
```

- [sass](https://getbootstrap.com/docs/5.0/customize/sass/)

Creamos una carpeta llamada ``sass/custom.scss``

```scss
@import "../node_modules/bootstrap/scss/bootstrap";
```

```html
<link rel="stylesheet" href="./css/custom.css">
```

## custom.scss
- [font](https://fonts.google.com/specimen/Barlow+Semi+Condensed?query=Barlow&selection.family=Barlow+Semi+Condensed:ital,wght@0,300;0,600;0,900;1,100&sidebar.open=true)

```html
<link rel="preconnect" href="https://fonts.gstatic.com">
<link href="https://fonts.googleapis.com/css2?family=Barlow+Semi+Condensed:ital,wght@0,300;0,600;0,900;1,100&display=swap" rel="stylesheet">
<link rel="stylesheet" href="./css/custom.css">
```

```scss
// Revisar el archivo node_modules\bootstrap\scss\_variables.scss
$primary:#733FC8;
$success: #49556B;
$dark: #18202D;
$secondary: #EDF2F8;

// Revisar el archivo node_modules\bootstrap\scss\_variables.scss
$font-family-sans-serif: 'Barlow Semi Condensed', sans-serif;

// https://getbootstrap.com/docs/5.0/layout/breakpoints/#min-width
@media (min-width: 992px) {
    .alto-100 {
        height: 100vh;
    }
}

.d-flex img{
    width: 50px;
}

// Agregar clase a la primera card
.quotation {
    background-image: url('../images/bg-pattern-quotation.svg');
    background-repeat: no-repeat;
    background-position: 85% top;
}

// Revisar el archivo node_modules\bootstrap\scss\_variables.scss
$container-max-widths: (
  sm: 540px,
  md: 720px,
  lg: 960px,
  xl: 960px,
  xxl: 960px
);

@import "../node_modules/bootstrap/scss/bootstrap";
```

## PurgeCSS
- [https://purgecss.com/](https://purgecss.com/)

```
npm i -g purgecss
```

```json
 "scripts": {
    "build": "purgecss --css css/custom.css --content index.html --output css/reducido.css"
  },
```

Reemplazar custom.css por:
```html
<link rel="stylesheet" href="./css/reducido.css">
```

:::warning
En caso de realizar algún cambio en nuestro archivo ``custom.scss`` se necesita realizar nuevamente el script `npm run build`
:::

## Muchas Gracias ❤
Si llegaste hasta acá, te doy las gracias por visualizar el video, puedes apoyar:

1. Regalame un like 👍
2. [No olvides Suscribirte al canal de Youtube 💙 click aquí 💙](https://bit.ly/3kLYAqr)
3. Déjame tu super comentario 😍
4. Comparte con amigos este tutorial 👏🏼
5. [¡No pares de aprender! Revisa más cursos y tutoriales aquí](https://bluuweb.github.io/)

Fin 🏄🏾‍♂️


