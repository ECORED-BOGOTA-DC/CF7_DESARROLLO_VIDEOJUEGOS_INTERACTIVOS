<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    .titulo-principal.color-acento-contenido
      .titulo-principal__numero
        span 1
      h1 Metodología RITE
    .row.justify-content-center 
      .col-lg-10
        .bloque-texto-g.color-acento-contenido.p-3.p-sm-4.p-md-5
          .bloque-texto-g__img(
            :style="{'background-image': `url(${require('@/assets/curso/tema1/1.png')})`}"
          )
          .bloque-texto-g__texto.p-4
            p.mb-0 Las siglas RITE significan Rapid Iterative Testing Evaluation, es decir testeo rápido iterativo de evaluación. Por consiguiente, la metodología RITE consiste en un método para evaluar el desarrollo de un proyecto a través de ciclos rápidos de ejecución hasta alcanzar el resultado final, a estos ciclos se les llama iteraciones. 
              br
              br
              | Cada iteración representa un bloque de tareas que se realizan, se prueban y evalúan hasta lograr el perfeccionamiento del producto deseado.
        .tarjeta.color-primario.p-3.mb-5.mt-5
          .row.justify-content-around.align-items-center
            .col-3.col-sm-2.col-lg-1
              img(src="@/assets/curso/tema1/i1.svg")
            .col
              .row.justify-content-between.align-items-center
                .col.mb-3.mb-sm-0
                  h3.mb-1 Iterativo e incremental
                  p.text-small Existe el método iterativo y el iterativo incremental los que se pueden observar en el video sobre este concepto.
                .col-sm-auto
                  a.boton.color-acento-botones.texto-blanco(:href="obtenerLink('downloads/prueba.pdf')" target="_blank")
                    span Ver video
                    i.fas.fa-file-download
    p.mt-4 De acuerdo con lo anterior, en el método iterativo para llevar a cabo un proyecto primero se define el concepto y alcance de este, después se desglosan las tareas que se realizarán en todo el proceso de desarrollo donde cada iteración es la construcción de una parte del concepto, ejecutándose y evaluándose repetidas veces si es necesario y al final se integran las partes construidas hasta lograr el concepto que se ha diseñado del producto final.
    .col-lg-12.mt-4
      .cajon.color-acento-contenido.p-4.mb-4
        p En el método iterativo e incremental se parte de la necesidad que se tiene y se estructura un proyecto definiendo tareas que se van ejecutando en cada iteración y evaluándose para aproximarse paulatinamente (incrementalmente) a lo que será el producto final como solución al problema identificado.
    .row.justify-content-center.mt-4 
      .col-lg-10
        .row 
          .col-lg-6   
            p En el desarrollo de videojuegos el método que se utiliza es el iterativo incremental y en cada iteración se ejecuta una tarea que se iterará o repetirá probándose hasta que se pueda avanzar a la siguiente que será un progreso respecto a la iteración anterior; es decir, el producto va aproximándose a lo que se desea de él y se puede testear o probar cada iteración con el usuario para obtener la retroalimentación necesaria e ir perfeccionándose.
            p Lo anterior quiere decir que dentro del equipo desarrollador del videojuego se debe contar con un integrante que haga las veces de tester o testeador que:
          .col-lg-6
            img(src="@/assets/curso/tema1/2.png")
    .col-sm.mb-5.mb-sm-0.mt-5
      ol.lista-ol--cuadro.lista-ol--separador
        li 
          .lista-ol--cuadro__vineta
            span a
          | Verifica constantemente las mecánicas que se van creando.
        li 
          .lista-ol--cuadro__vineta
            span b
          | Hace los ajustes necesarios y los valida de nuevo.
        li 
          .lista-ol--cuadro__vineta
            span c
          | Vuelve a realizar las mejoras documentando los fallos o errores con los cambios que se van llevando a cabo en el diseño o en la programación. 
        li 
          .lista-ol--cuadro__vineta
            span d
          | Aproxima cada producto parcial a lo que finalmente se desea obtener. 
    separador
    #t_1_1.titulo-segundo.color-acento-contenido
      h2 1.1 Herramienta de testeo en Unity
    p El software de videojuegos de Unity posee herramientas que pueden ayudar a testear las iteraciones para detectar los errores que se producen cuando se están ejecutando o desarrollando tareas en el videojuego, ya sea cuando se están escribiendo líneas de código o cuando se están llevando a cabo acciones con el menú para crear las escenas y mecánicas del videojuego.
    img(src="@/assets/curso/tema1/3.png")
    p.mt-4 Existen testeos rápidos que están incorporados en el software cuando se instala. Al conocer los errores que se producen en las iteraciones, el desarrollador puede tomar la decisión adecuada para dar solución; por ejemplo, corregir la sintaxis de programación necesaria o importar los archivos (asset) de formatos permitidos para incorporar en la escena.
    .row.mt-4
      .col-lg-4
        .row.align-items-center
          .col-2
            img(src="@/assets/curso/tema1/i2.svg")
          .col-10
            h3.mb-0 Mensajes de error en la consola
    p.mt-4 La consola es una pestaña que se encuentra dentro de la ventana de proyectos y es allí donde se van almacenando los mensajes de error al realizar iteraciones que ocasionen conflictos en la ejecución del videojuego. Estos mensajes permiten realizar acciones correctivas al diseñador para poder avanzar a otra fase de iteración. 
    p En la imagen se observan cuatro mensajes de error en la consola; errores que se han cometido en la manipulación del programa, por ejemplo:
    .row.justify-content-center 
      .col-lg-8
        ImagenInfografica.color-secundario.mb-5
          template(v-slot:imagen)
            figure
              img(src='@/assets/curso/tema1/4.svg', alt='Texto que describa la imagen')

          .tarjeta.color-secundario.p-3(x="2%" y="74%" numero="")
            p Significa que se  está intentando importar un activo que contiene un administrador de juegos global, lo cual no está permitido. Los activos son archivos con formatos específicos que permiten ser copiados en el juego.
          .tarjeta.color-secundario.p-3(x="2%" y="80%" numero="")
            p Significa que se  está intentando importar un activo que contiene un administrador de juegos global, lo cual no está permitido. Los activos son archivos con formatos específicos que permiten ser copiados en el juego.
          .tarjeta.color-secundario.p-3(x="2%" y="85%" numero="")
            p Quiere decir que hay una expresión que comienza con mayúsculas y/o minúsculas (nombre de ruta, base de datos de activos): es decir que se escribió una secuencia de comandos incorrecta en la sintaxis.
          .tarjeta.color-secundario.p-3(x="2%" y="91%" numero="")
            p Se está sugiriendo que se están copiando archivos con una ruta única generada no válida.
    p Esta herramienta permite identificar los fallos está contenida en el software, es de rápido testeo para probar el funcionamiento del juego no solo para el desarrollador, sino para el usuario, puesto que informa exactamente qué está sucediendo cuando se ejecutan sus diferentes mecánicas.
    separador
    #t_1_2.titulo-segundo.color-acento-contenido
      h2 1.2 Herramienta de testeo incorporada a Unity  
    p Existen herramientas de testeo que se pueden importar al software y que en el momento de la instalación no son incorporadas. Las hay de descarga gratuita y también de pago que se incorporan al software en forma de assets o componentes que se integran en el menú del programa, para ser utilizadas en la identificación de incoherencias y fallos presentados en el desarrollo o rodaje de las escenas del videojuego. Cabe anotar que no se necesita ser un experto programador para utilizar estos componentes, puesto que son de fácil manejo y de ellos se encuentra documentación que explica la dinámica de uso.
    .row.mt-4
      .col-lg-3
        .row.align-items-center
          .col-2
            img(src="@/assets/curso/tema1/i2.svg")
          .col-9
            h3.mb-0 Unity Test Tool 
    p.mt-5 Este componente o asset permite realizar un testeo o evaluación rápida de las funcionalidades que se van incorporando al juego. Es una herramienta que se debe integrar desde la opción de Asset Store del menú de Unity ya que una vez se instala el programa no es importada de la nube automáticamente.
    p Pasos para incorporar esta herramienta dentro del programa de Unity:
    .tarjeta.tarjeta--gris.p-4
      PasosB.color-acento-botones

        .row.justify-content-center(titulo="")
          .col-lg-11
            .row
              .col-md-6.mb-4.mb-md-0
                p Hacer clic en el menú Window->Asset Store  y el programa se direcciona a la URL https://www.assetstore.unity3d.com/en/#!/content/13802.
                p En la ventana de la escena aparece la página de UnityAssetStore y en el buscador se debe escribir “Unity Test Tools”.
                .mb-3

                  a.boton.me-3.indicador__container(
                    :href="obtenerLink('downloads/prueba.pdf')"
                    target="_blank"
                    type="application/pdf"
                    @mouseover="mostrarIndicador = false"
                  )
                    span Ampliar imagen
                    i.fas.fa-file-download
                    .indicador--click(v-if="mostrarIndicador")

              .col-md-6
                figure
                  img(src='@/assets/curso/tema1/5.png', alt='Texto que describa la imagen')

        .row.justify-content-center(titulo="")
          .col-lg-11
            .row
              .col-md-6.mb-4.mb-md-0
                p Luego aparecen los asset gratuitos y seleccionar uno de ellos, en este caso se seleccionará la herramienta BDD Test:
                .mb-3

                  a.boton.me-3.indicador__container(
                    :href="obtenerLink('downloads/prueba.pdf')"
                    target="_blank"
                    type="application/pdf"
                    @mouseover="mostrarIndicador = false"
                  )
                    span Ampliar imagen
                    i.fas.fa-file-download
                    .indicador--click(v-if="mostrarIndicador")

              .col-md-6
                figure
                  img(src='@/assets/curso/tema1/6.png', alt='Texto que describa la imagen')
        .row.justify-content-center(titulo="")
          .col-lg-11
            .row
              .col-md-6.mb-4.mb-md-0
                p Hacer clic en la opción Download para proceder a la descarga de la herramienta de testeo.
                .mb-3

                  a.boton.me-3.indicador__container(
                    :href="obtenerLink('downloads/prueba.pdf')"
                    target="_blank"
                    type="application/pdf"
                    @mouseover="mostrarIndicador = false"
                  )
                    span Ampliar imagen
                    i.fas.fa-file-download
                    .indicador--click(v-if="mostrarIndicador")

              .col-md-6
                figure
                  img(src='@/assets/curso/tema1/7.png', alt='Texto que describa la imagen')
        .row.justify-content-center(titulo="")
          .col-lg-11
            .row
              .col-md-6.mb-4.mb-md-0
                p Después que el programa hace la descarga, aparece la siguiente pantalla y se debe hacer clic en el botón Import que aparece en la esquina inferior derecha de la ventana.
                .mb-3

                  a.boton.me-3.indicador__container(
                    :href="obtenerLink('downloads/prueba.pdf')"
                    target="_blank"
                    type="application/pdf"
                    @mouseover="mostrarIndicador = false"
                  )
                    span Ampliar imagen
                    i.fas.fa-file-download
                    .indicador--click(v-if="mostrarIndicador")

              .col-md-6
                figure
                  img(src='@/assets/curso/tema1/8.png', alt='Texto que describa la imagen')
        .row.justify-content-center(titulo="")
          .col-lg-11
            .row
              .col-md-6.mb-4.mb-md-0
                p Inmediatamente el componente se adiciona al programa Unity y, específicamente, al proyecto que se esté trabajando. En la ventana de proyecto se observa el componente de testeo adicionado para hacer las pruebas rápidas en las escenas y mecánicas del juego.
                .mb-3

                  a.boton.me-3.indicador__container(
                    :href="obtenerLink('downloads/prueba.pdf')"
                    target="_blank"
                    type="application/pdf"
                    @mouseover="mostrarIndicador = false"
                  )
                    span Ampliar imagen
                    i.fas.fa-file-download
                    .indicador--click(v-if="mostrarIndicador")

              .col-md-6
                figure
                  img(src='@/assets/curso/tema1/9.png', alt='Texto que describa la imagen')
        .row.justify-content-center(titulo="")
          .col-lg-11
            .row
              .col-md-6.mb-4.mb-md-0
                p Cuando se realiza cualquier acción en Unity por ejemplo, insertar un objeto a una escena, la herramienta Unity Test Tools se adiciona a este y analiza cualquier error en él o en la acción de copiarlo en la ventana de la escena.  Por ejemplo, a continuación la acción que se va a realizar es arrastrar con el mouse el Sprite 3 que es un objeto de fondo de la ventana de Project a la ventana de la escena:
                .mb-3

                  a.boton.me-3.indicador__container(
                    :href="obtenerLink('downloads/prueba.pdf')"
                    target="_blank"
                    type="application/pdf"
                    @mouseover="mostrarIndicador = false"
                  )
                    span Ampliar imagen
                    i.fas.fa-file-download
                    .indicador--click(v-if="mostrarIndicador")

              .col-md-6
                figure
                  img(src='@/assets/curso/tema1/10.png', alt='Texto que describa la imagen')
        .row.justify-content-center(titulo="")
          .col-lg-11
            .row
              .col-md-6.mb-4.mb-md-0
                p Inmediatamente se activó la herramienta de testeo y mostró el siguiente mensaje en la ventana de la escena: All Compiller errors have to be fixed before you can enter play mode
                p La acción no se pudo realizar ya que la escena se encontraba en modo de reproducción y el objeto no se puede compilar o procesar a nivel de software. Los botones encerrados en el círculo son los que indican el modo play o modo pausa, en el momento de copiar el elemento se encontraba en modo play.
                .mb-3

                  a.boton.me-3.indicador__container(
                    :href="obtenerLink('downloads/prueba.pdf')"
                    target="_blank"
                    type="application/pdf"
                    @mouseover="mostrarIndicador = false"
                  )
                    span Ampliar imagen
                    i.fas.fa-file-download
                    .indicador--click(v-if="mostrarIndicador")

              .col-md-6
                figure
                  img(src='@/assets/curso/tema1/11.png', alt='Texto que describa la imagen')
    .row.justify-content-center.mt-4
      .col-lg-10
        .tarjeta.color-primario.p-3.mb-5.mt-5
          .row.justify-content-around.align-items-center
            .col-3.col-sm-2.col-lg-1
              img(src="@/assets/curso/tema1/i3.svg")
            .col
              .row.justify-content-between.align-items-center
                .col.mb-3.mb-sm-0
                  h3.mb-1 Unity Test Tools
                  p.text-small Para una mayor comprensión y profundización de las herramientas de testeo, se recomienda la siguiente lectura complementaria:
                .col-sm-auto
                  a.boton.color-acento-botones.texto-blanco(:href="obtenerLink('downloads/prueba.pdf')" target="_blank")
                    span Ver video
                    i.fas.fa-file-download


</template>

<script>
export default {
  name: 'Tema1',
  components: {},
  data: () => ({
    // variables de vue
  }),
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
  updated() {
    this.$aosRefresh()
  },
}
</script>

<style lang="sass"></style>
