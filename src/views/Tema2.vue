<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    .titulo-principal.color-acento-contenido
      .titulo-principal__numero
        span 2
      h1 Modelos de iteración
    p Como se mencionó antes, las iteraciones son paquetes de tareas que se reprocesan hasta lograr el perfeccionamiento de un producto, por consiguiente un modelo iterativo según Cockburn, mencionado por Letelier (2013), corresponde a una metodología de re-trabajo para lograr mejorar un producto, donde cada iteración contiene un conjunto de actividades con el objetivo de entregar parte de las funcionalidades del producto al usuario. 
    .row.justify-content-center.mt-4 
      .col-lg-6
        .titulo-sexto.color-acento-contenido
          h5 Figura 1
          span  Iteración incremental
        img(src="@/assets/curso/tema2/1.svg")
    p.mt-3 Entonces, en una primera iteración se entrega una parte de la funcionalidad del producto, en una segunda iteración se entrega la parte que falta de la funcionalidad y en una tercera se puede entregar una nueva, es decir cada iteración se aproxima al producto final.
    .col-lg-12
      .cajon.color-secundario.p-4.mb-4
        p A este modelo también se le denomina incremental, puesto que se van obteniendo resultados parciales que al sumarse completan el producto final. Los usuarios van obteniendo beneficios de manera incremental a medida que se completan las tareas que deben incluir las pruebas, los ajustes y la documentación generada en cada proceso de entrega, esto quiere decir que no se deja para lo último la verificación de que el producto cumpla con los requisitos del proyecto.
    p.mt-4 Para citar un ejemplo sencillo de este modelo, en el desarrollo del juego se puede planificar que dos imágenes en escena, una quede en el fondo y la otra en el primer plano:
    ol.lista-ol--cuadro.mt-4
        li 
          .lista-ol--cuadro__vineta
            span a
          | El primer producto es colocar las imágenes en una escena; esta entrega consiste en dos iteraciones donde se realiza el mismo proceso: 
    p.mt-4 Cuando se crea un perfil de la aplicación, hay algunas cosas que puede hacer para garantizar la coherencia entre las sesiones de creación de perfiles y para asegurarse de que los procesos que utiliza Unity no afecten los datos de creación de perfiles:
    .tabla-b.color-acento-contenido.mb-5
      .tabla-b__header
        .row 
          .col-lg-6
            h4.mb-0.text-white Iteración 1

            h4.mb-0.text-white  para insertar fondo en ventana de escena
          .col-lg-6
            h4.mb-0.text-white Iteración 2
            h4.mb-0.text-white  para insertar superhéroe en ventana de escena
      table
        tr
          th •   Ubicarse en la ventana de proyecto.
          th •   Ubicarse en la ventana de proyecto.
        tr
          th •   Abrir carpeta de asset fondos.
          th •   Abrir carpeta de asset fondos.
        tr
          th •   Seleccionar el fondo y arrástralo a la ventana de la escena.
          th •   Seleccionar el superhéroe y arrástralo a la ventana de la escena.
    .row.mt-4.justify-content-center 
      .col-lg-10
        p.mb-0 Obsérvese que en la ventana de jerarquía (parte izquierda) aparecen en orden de jerarquía las dos imágenes:
        p.mb-0 Primero el fondo - surface2-animation_0 
        p Segundo el superhéroe - 5a0c3f295a997e1c2cea1158.png      
        img(src="@/assets/curso/tema2/2.png")
        .col-lg-12.mt-4 
          .cajon.color-secundario.p-4.mb-4
            p Estas iteraciones corresponden a la primera entrega incremental.
    ol.lista-ol--cuadro.mt-4
        li 
          .lista-ol--cuadro__vineta
            span b
          | El segundo producto es colocar la imagen del superhéroe sobre el fondo; esta entrega se compone de dos iteraciones: 
    p.mt-4 Cuando se crea un perfil de la aplicación, hay algunas cosas que puede hacer para garantizar la coherencia entre las sesiones de creación de perfiles y para asegurarse de que los procesos que utiliza Unity no afecten los datos de creación de perfiles:
    img(src="@/assets/curso/tema2/3.svg")
    p.mt-3 Para obtener el producto final se llevaron a cabo 4 iteraciones incrementales puesto que se tuvieron que realizar cuatro tareas para conseguir lo que se deseaba en el proyecto.
    p Los beneficios del modelo de iteración incremental radican en que:
    .col-sm.mb-5.mb-sm-0
      ul.lista-ul--color
        li.mb-0
          i.fas.fa-brain
          | Se pueden tomar decisiones en cada iteración, por ejemplo cambiar de personaje, de fondo, la escala de las imágenes, la rotación o la posición.
        li.mb-0
          i.fas.fa-brain
          | El equipo desarrollador tiene la posibilidad de validar si lo que ha realizado era lo que el usuario esperaba y hacer los ajustes necesarios.
        li.mb-0
          i.fas.fa-brain
          | No es necesario realizar una recopilación detallada de la información del producto ya que por el camino pueden surgir nuevos conceptos y se pueden ir afinando detalles.
        li.mb-0
          i.fas.fa-brain
          | Desde el comienzo se pueden obtener resultados y el usuario puede ir probando la usabilidad del producto aunque este no esté terminado.
        li.mb-0
          i.fas.fa-brain
          | Después de cada iteración se puede obtener el feedback del usuario y hacer los ajustes requeridos.  
        li.mb-0
          i.fas.fa-brain
          | Debido a que el proyecto se evalúa después de cada iteración, se minimizan los riesgos y se optimizan los recursos, puesto que los fallos son detectados y superados a tiempo.
        li.mb-0
          i.fas.fa-brain
          | El proyecto se puede planificar de manera más acertada en los tiempos de ejecución, ya que se conoce con exactitud el avance de cada fase y por consiguiente proyectar su finalización.
        li.mb-0
          i.fas.fa-brain
          | Se minimiza el número de errores y se incrementa la calidad del producto.
        li.mb-0
          i.fas.fa-brain
          | Cada iteración entrega unos resultados concretos para el proyecto y el usuario de tal manera que se obtienen funcionalidades gradualmente y no hasta el final.
    p.mt-5 Algunos de los modelos iterativos que se están utilizando en este momento son: Proceso Unificado Racional (RUP), Programación Externa y SCRUM.
    separador
    #t_2_1.titulo-segundo.color-acento-contenido
      h2 2.1 Proceso Unificado Racional - PUR
    p El Proceso Unificado Racional – PUR es una metodología de desarrollo de software que se basa en componentes e interfaces para analizar, diseñar, codificar, implementar, probar y documentar sistemas orientados a objetos y se vale para ello de un Lenguaje Unificado de Modelado - UML.
    separador
    #t_2_3.titulo-segundo.color-acento-contenido
      h2 2.3 Scrum
    p Es una metodología de trabajo en equipo para el desarrollo de un proyecto. El término fue extraído del deporte Rugby en el que un número de jugadores de cada equipo hace una formación fija para entrar a disputar la tenencia del balón y cada vez que este sale del juego se hace un nuevo Scrum o formación. Esta metodología fue desarrollada por Nonaka y Takeuchi en 1986 para agilizar el desarrollo de productos comerciales en cualquier sector de la economía. Es aplicable en la industria tecnológica para el desarrollo de software de diferentes categorías entre ellas los videojuegos.
    h5.mt-4 Elementos Scrum:
    TabsA.color-acento-contenido.mb-5
      .tarjeta.color-secundario.p-4(titulo="Equipo de trabajo")
        h4 Equipo de trabajo
        p Está conformado por el cliente o dueño del producto, el Scrum manager o gestionador del proyecto, el equipo Scrum que desarrolla el producto, los stakeholders o asesores del proyecto (internos o externos) y los usuarios que realizan las pruebas del producto.
      .tarjeta.color-secundario.p-4(titulo="Pila de producto")
        h4 Pila de producto
        p Es la lista priorizada de requisitos para la elaboración del producto, en la que puede intervenir todo el equipo para su elaboración, pero solo el cliente y el director del equipo es responsable de decidir sobre ella.
      .tarjeta.color-secundario.p-4(titulo="Artefactos")
        h4 Artefactos
        p Están representados por la información clave generada en el proceso de desarrollo del producto; entre la que se encuentra la pila de producto, la planificación de la pila y la retrospectiva.
      .tarjeta.color-secundario.p-4(titulo="Flujo de actividades")
        h4 Flujo de actividades
        p Es la lista de tareas de iteración que se deben ejecutar para el desarrollo de la pila del sprint.
      .tarjeta.color-secundario.p-4(titulo="Fases")
        h4 Fases
        p Corresponde a las diferentes etapas del proceso que se lleva a cabo para obtener el producto final.
    .row.mt-4
      .col-lg-7
        .row.align-items-center
          .col-1
            img(src="@/assets/curso/tema1/i2.svg")
          .col-11
            h3.mb-0 Fases para el desarrollo de un videojuego en el modelo Scrum
    p.mt-4 Este componente o asset permite realizar un testeo o evaluación rápida de las funcionalidades que se van incorporando al juego. Es una herramienta que se debe integrar desde la opción de Asset Store del menú de Unity ya que una vez se instala el programa no es importada de la nube automáticamente.
    p Pasos para incorporar esta herramienta dentro del programa de Unity:
    .row.mt-4
      .col-lg-3
        .row.align-items-center.mt-4
          .col-2
            img(src="@/assets/curso/tema2/4.svg")
          .col-10
            h5.mb-0 Planificación de la iteración
    .row.mb-5.mt-5
      .col-md-6.col-lg.mb-5.mb-lg-0
        .tarjeta-avatar
          img(src='@/assets/curso/tema2/c1.svg' alt='AvatarTop')
          .tarjeta.color-acento-contenido
            .p-4
              p.text-center En la Planificación de la iteración el equipo desarrollador selecciona los requisitos de la lista que el cliente elaboró, los prioriza y despeja las dudas, realiza una lista de las tareas que se van a llevar a cabo en la iteración.

      .col-md-6.col-lg.mb-5.mb-lg-0
        .tarjeta-avatar
          img(src='@/assets/curso/tema2/c2.svg' alt='AvatarTop')
          .tarjeta.color-acento-contenido
            .p-4
              p.text-center Planifica el tiempo de las tareas; el cual es generalmente de una semana (1) por actividad hasta completar un máximo de cuatro (4) por iteración es decir 30 días.

      .col-md-6.col-lg.mb-5.mb-lg-0
        .tarjeta-avatar
          img(src='@/assets/curso/tema2/c3.svg' alt='AvatarTop')
          .tarjeta.color-acento-contenido
            .p-4
              p.text-center Se organizan en parejas o en las personas que sean necesarias para completarla.
    .row.mt-4
      .col-lg-3
        .row.align-items-center.mt-4
          .col-2
            img(src="@/assets/curso/tema2/4.svg")
          .col-10
            h5.mb-0 Sincronizaciones diarias
    p.mt-4 De acuerdo con las respuestas proporcionadas por los integrantes del equipo el Scrum, el manager (gestionador del proyecto) debe encargarse de hacer la inspección de los obstáculos y hacer las adaptaciones necesarias para eliminarlos, garantizando que el equipo pueda realizar las actividades para terminar la iteración.
    p En Sincronizaciones diarias el equipo realiza reuniones diarias normalmente de 15 minutos frente a un tablero para autoevaluarse frente a los avances en la tarea planteándose las siguientes preguntas:
    .row.justify-content-center 
      .col-lg-8
        .row.mt-4.color1.p-2
          p.text-center.mb-0 ¿Qué he hecho desde la última reunión de sincronización para aportar al cumplimiento de la tarea?
        .row.mt-4.color2.p-2
          p.text-center.mb-0 ¿Qué voy a hacer a partir de este momento para ayudar al equipo a cumplir el objetivo de la tarea?
        .row.mt-4.color3.p-2
          p.text-center.mb-0 ¿Qué obstáculos me impiden colaborar con el trabajo en equipo para conseguir el objetivo?
    .row.mt-4
      .col-lg-2
        .row.align-items-center.mt-4
          .col-3
            img(src="@/assets/curso/tema2/4.svg")
          .col-9
            h5.mb-0 Retrospectiva
    .row.mb-5.mt-5
      .col-md-6.col-lg.mb-5.mb-lg-0
        .tarjeta-avatar
          img(src='@/assets/curso/tema2/c1.svg' alt='AvatarTop')
          .tarjeta.color-acento-contenido
            .p-4
              p.text-center El Scrum manager junto con el equipo realiza una retrospectiva del trabajo para identificar en que se puede mejorar la metodología y las técnicas utilizadas para incrementar la productividad.

      .col-md-6.col-lg.mb-5.mb-lg-0
        .tarjeta-avatar
          img(src='@/assets/curso/tema2/c2.svg' alt='AvatarTop')
          .tarjeta.color-acento-contenido
            .p-4
              p.text-center De acuerdo con las observaciones recibidas por el cliente se inspeccionan de nuevo los obstáculos que impiden la optimización del producto obtenido y se hacen las adaptaciones necesarias.

      .col-md-6.col-lg.mb-5.mb-lg-0
        .tarjeta-avatar
          img(src='@/assets/curso/tema2/c3.svg' alt='AvatarTop')
          .tarjeta.color-acento-contenido
            .p-4
              p.text-center En la Retrospectiva, es decir el día que se tiene previsto terminar la iteración, se hace nuevamente una reunión de 1 o 2 horas con el cliente para realizar una demostración del cumplimiento de los requisitos planteados inicialmente plasmados ahora sí en el producto incremental, resultado de la iteración completada.
    .row.mt-4
      .col-lg-7
        .row.align-items-center
          .col-1
            img(src="@/assets/curso/tema1/i2.svg")
          .col-11
            h3.mb-0 Características de Scrum
    p.mt-4 Este componente o asset permite realizar un testeo o evaluación rápida de las funcionalidades que se van incorporando al juego. Es una herramienta que se debe integrar desde la opción de Asset Store del menú de Unity ya que una vez se instala el programa no es importada de la nube automáticamente.
    p Pasos para incorporar esta herramienta dentro del programa de Unity:
    TabsA.color-acento-contenido.mb-5
      .tarjeta.color-secundario.p-4(titulo="Elaboración de pila de producto")
        h4 Elaboración de pila de producto
        p Se refiere a los requerimientos que el cliente hace al equipo desarrollador, los cuales son elaborados en forma de pila o lista de requisitos, que se deben priorizar para su desarrollo. 
      .tarjeta.color-secundario.p-4(titulo="Planificación flexible")
        h4 Planificación flexible
        p El cliente puede aumentar o cambiar los requisitos durante el proceso de desarrollo de cada iteración, esto significa que lo definido en un comienzo no se toma como una camisa de fuerza y el equipo debe estar en capacidad de dar respuesta a las nuevas necesidades.
      .tarjeta.color-secundario.p-4(titulo="Desarrollo incremental")
        h4 Desarrollo incremental
        p Las iteraciones se planifican con el cliente de tal manera que el resultado sea un producto incremental, es decir, una parte de este hasta obtener el resultado final. Una vez desarrolladas las funciones con las que se llevan a cabo operaciones, se presentan al cliente para que éste pueda probarlas y hacer el feedback inmediatamente. El equipo inspecciona y hace las adaptaciones si son necesarias antes de terminar la iteración.
    h4.mt-4 Ejemplo de Scrum
    p  El siguiente ejemplo es lo que se haría en la fase 1 de la situación planteada anteriormente sobre lo que se debe realizar en la o las iteraciones para que un usuario pueda ingresar a un videojuego.
    p En la siguiente tabla se observa que hay una sola iteración compuesta de seis (6) tareas a desarrollar, el equipo se puede repartir por parejas para ejecutar cada una de ellas. Cada pareja tiene determinados días para el desarrollo de la iteración.
    .tabla-b.color-acento-contenido.mb-5
      .tabla-b__header
        .row 
          .col-lg-2
            h4.mb-0.text-white Lista de requisitos
            h4.text-white priorizada
          .col-lg-4
            h4.mb-0.text-white Lista de tareas de la iteración

          .col-lg-6
            h4.mb-0.text-white Planificación de iteración
      table
        tr
          th Entrar al juego.
          th 1. Codificación de Login/Logout (entrada/ salida).
          th Equipo:   2 personas desarrollan.<br>Tiempo:  5 días.<br>Producto: interfaz (pantalla) de ingreso al juego, menú de inicio de sesión, alternativas de Login y Logout.
        tr
          th Hacer registro.
          th 2. Codificación de formulario para registro de datos y alias.
          th Equipo:   2 personas desarrollan.<br>Tiempo:  5 días.<br>Producto: formulario para registro de datos, con nombre, apellido, alias, edad, contraseña.
        tr
          th Colocar alias.
          th 3. Elaboración de base de datos de consulta de alias.
          th Equipo:   2 personas desarrollan.<br>Tiempo:  5 días.<br>Producto: formulario para registro de datos, con nombre, apellido, alias, edad, contraseña.
        tr
          th Empezar a jugar.
          th 4. Diseño de funciones del juego. <br>5. Codificación de instrucciones para activar funciones iniciales en la interfaz inicial del usuario.
          th Equipo:   2 personas desarrollan.<br>Tiempo:  5 días.<br>Producto: diseño funciones del juego.<br><br>Equipo:   2 personas desarrollan.<br>Tiempo:  7 días.<br>Producto: funciones de la interfaz del usuario activadas.
        tr
          th Interrumpir el juego.
          th 6. Codificación de instrucciones para parar las funciones que se estén ejecutando y guardar la memoria donde quedaron para cuando se reinicie el juego.
          th Equipo:   2 personas desarrollan.<br>Tiempo:  7 días.<br>Producto: función de interrupción del juego activada.
        tr
          th Salir.
          th Codificación de Login/Logout (entrada/ salida) ya se hizo en la tarea 1.
          th Producto: función salir activada por el usuario cuando desee abandonar el juego.
    p Si se quiere profundizar en estos temas, se recomienda la siguiente lectura complementaria:
    .row.justify-content-center.mt-4
      .col-lg-10
        .tarjeta.color-primario.p-3.mb-5.mt-5
          .row.justify-content-around.align-items-center
            .col-3.col-sm-2.col-lg-1
              img(src="@/assets/curso/tema1/i3.svg")
            .col
              .row.justify-content-between.align-items-center
                .col.mb-3.mb-sm-0
                  h3.mb-1 Lecturas de consulta
                  p.text-small Proyectos ágiles.org. (s.f). Desarrollo iterativo e incremental.
                  p.text-small Pérez, O (2011). Cuatro enfoques metodológicos para el desarrollo de software.

                .col-sm-auto
                  a.boton.color-acento-botones.texto-blanco(:href="obtenerLink('downloads/prueba.pdf')" target="_blank")
                    span Enlace web
                    i.fas.fa-file-download    
                  .row.mt-4
                    .col-sm-auto
                      a.boton.color-acento-botones.texto-blanco(:href="obtenerLink('downloads/prueba.pdf')" target="_blank")
                        span Enlace web
                        i.fas.fa-file-download   



</template>

<script>
export default {
  name: 'Tema2',
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

<style lang="sass">

.tarjeta.color-acento-contenido
  background-color: #E1DDFC
</style>
