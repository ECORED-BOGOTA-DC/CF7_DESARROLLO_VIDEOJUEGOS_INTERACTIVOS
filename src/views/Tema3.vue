<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    .titulo-principal.color-acento-contenido
      .titulo-principal__numero
        span 3
      h1 Modelos de prueba de usabilidad
    p.mt-4 Probar la usabilidad de un proyecto, producto o, en este caso, un videojuego es, según Lorés (2006), evaluar que este tenga interacción con el usuario. Las pruebas de usabilidad comprenden la utilización de metodologías y técnicas para determinar en un producto su capacidad y facilidad de ser usado y así lograr una experiencia de usuario satisfactoria.
    .row 
      .col-lg-6
        img(src="@/assets/curso/tema3/1.png")

      .col-lg-6
        .bloque-texto-b.color-acento-contenido.p-4
          .bloque-texto-b__texto
            i.fas.fa-quote-left
            p.mb-0 Lorés se refirió a la definición que hace la ISO 98 sobre usabilidad como la medida en la que un producto puede ser usado por los usuarios para lograr sus objetivos con efectividad y eficiencia en un contexto específico, pero este término está ligado al de experiencia de usuario (UX) el cual, según la International Standard ISO 9241-210 (2010), tiene que ver con “las percepciones y respuestas de la persona, resultantes del uso y/ o uso anticipado de un producto, sistema o servicio”.

            i.fas.fa-quote-right      
        p.mt-2 En el proceso de diseño y desarrollo de videojuegos se debe evaluar permanentemente la experiencia del usuario al interactuar con el producto, de tal manera que llegue a tener plena satisfacción y de esta forma evitar rediseños posteriores que implique mayores recursos de los que se habían presupuestado.
    .row.justify-content-center.mt-4
      .col-lg-10
        .tarjeta.color-primario.p-3.mb-5.mt-5
          .row.justify-content-around.align-items-center
            .col-3.col-sm-2.col-lg-1
              img(src="@/assets/curso/tema3/c1.svg")
            .col
              .row.justify-content-between.align-items-center
                .col.mb-3.mb-sm-0
                  h3.mb-1 Pruebas de Usabilidad con Veronica Traynor
                  p.text-small Para lograr usabilidad y por consiguiente una UX satisfactoria en un videojuego se debe chequear entonces que la interacción del juego con el usuario fluya de manera natural, para ello se pueden hacer pruebas antes de empezar la fase de diseño y programación:
                .col-sm-auto
                  a.boton.color-acento-botones.texto-blanco(:href="obtenerLink('downloads/prueba.pdf')" target="_blank")
                    span Ver video
                    i.fas.fa-file-download        
    p.mt-3 El video refiere una prueba realizada individualmente a dos personas de edades diferentes en distintos momentos y de las cuales el diseñador ha observado y extraído los detalles respecto a las lógicas mentales que utilizan la una y la otra para realizar la misma acción.
    p En las pruebas de usabilidad se observan aspectos del usuario y del sistema. En los usuarios se observa la forma en que este usa el producto para conseguir el objetivo y en el sistema la respuesta que provee el programa ante las interacciones que el usuario realiza con el producto. 
    p Lorés (2006) ha clasificado en modelos o metodologías la forma de evaluar la usabilidad y dentro de ellas menciona técnicas que se pueden utilizar para probarla:
    .row.justify-content-center.mt-4
      .col-lg-6    
        .titulo-sexto.color-acento-contenido
          h5 Figura 2
          span   Pruebas de usabilidad en videojuegos
        img(src="@/assets/curso/tema3/2.svg")      
    p.mt-3 En la figura anterior se observan claramente tres modelos o metodologías de prueba de usabilidad los que, a su vez, poseen técnicas que se pueden aplicar para probar el producto.
    separador
    #t_3_1.titulo-segundo.color-acento-contenido
      h2 3.1 Modelo de inspección 
    p Esta metodología comprende un conjunto de técnicas que se evalúan y se enfocan en la interfaz del usuario (UI), es decir se basa en los puntos de interacción y comunicación del usuario con los aspectos de visualización. En el caso del videojuego se evalúan los criterios que tienen que ver con elementos específicos de los escenarios con los que interactúa el jugador. Dentro de este método se encuentran las siguientes técnicas:
    .row.mt-4
      .col-lg-4
        .row.align-items-center
          .col-2
            img(src="@/assets/curso/tema1/i2.svg")
          .col-10
            h3.mb-0 Técnica de evaluación heurística
      p.mt-4 consiste en el análisis de la interfaz con la cual interactúa el usuario para determinar si responde a los siguientes principios de usabilidad, donde cada principio corresponde a una “H” en la heurística:
    TabsC.color-acento-contenido
      .py-3.py-md-4(titulo="H1")
        .row
          .col-md-1
          .col-md-4.mb-4.mb-md-0
            h4 Visibilidad del estado del sistema
            p El usuario debe recibir una retroalimentación del estado del producto en cada instante para saber qué pasa cuando interactúa con él. 
            p Por ejemplo, en un videojuego se debe poder determinar si el programa se está cargando para empezar a jugar o si hay algún tipo de error.
          .col-md-7
            figure
              img(src='@/assets/curso/tema3/3.png', alt='Texto que describa la imagen')
              figcaption Cargando
      .py-3.py-md-4(titulo="H2")
        .row
          .col-md-1
          .col-md-4.mb-4.mb-md-0
            h4 Relación del producto con el mundo real
            p Se debe brindar al usuario toda la información necesaria para que no tenga dudas o cometa errores en la acción que va a realizar. 

            p Por ejemplo, si se va a registrar en el juego debe poder ingresar sus datos a través de un formulario donde se le pregunte lo mínimo necesario como la edad, ya que todos los juegos no son aptos para menores.
          .col-md-7
            figure
              img(src='@/assets/curso/tema3/4.png', alt='Texto que describa la imagen')
              figcaption Registro
      .py-3.py-md-4(titulo="H3")
        .row
          .col-md-1
          .col-md-4.mb-4.mb-md-0
            h4 Libertad al usuario
            p El sistema debe permitir que el usuario cancele un proceso que estaba realizando sin finalizarlo, de tal manera que esta acción no representa compromisos o penalizaciones que puedan llegar a afectar en cualquier aspecto de su estado emocional o material. 


            p Por ejemplo, si el jugador intentó comprar el juego y después se arrepiente.
          .col-md-7
            figure
              img(src='@/assets/curso/tema3/5.png', alt='Texto que describa la imagen')
              figcaption Compra
      .py-3.py-md-4(titulo="H4")
        .row
          .col-md-1
          .col-md-4.mb-4.mb-md-0
            h4 Consistencia
            p Utilizar un patrón de diseño de los elementos del producto no solo le proporciona coherencia sino claridad y facilidad de uso a la hora de ser utilizado por el usuario. 

            p Por ejemplo, cuando se diseñan botones se deben diseñar del mismo color y tamaño.
          .col-md-7
            figure
              img(src='@/assets/curso/tema3/6.png', alt='Texto que describa la imagen')
              figcaption Registro
      .py-3.py-md-4(titulo="H5")
        .row
          .col-md-1
          .col-md-4.mb-4.mb-md-0
            h4 Prevención de errores
            p Se deben dar instrucciones claras a los usuarios sobre cómo manejar el producto y las acciones que deben realizar para evitar su mal uso y, posteriormente, el abandono, debido a los errores que puede arrojar. 

            p Por ejemplo, dibujar unas flechas en el camino para indicarle al jugador por dónde seguir.
          .col-md-7
            figure
              img(src='@/assets/curso/tema3/7.png', alt='Texto que describa la imagen')
              figcaption Indicación
      .py-3.py-md-4(titulo="H6")
        .row
          .col-md-1
          .col-md-4.mb-4.mb-md-0
            h4 Recordación
            p El producto debe proporcionar toda la información posible en aquellos momentos donde el usuario necesita recordar los detalles clave que le permitan confirmar la decisión que está a punto de tomar.


            p Por ejemplo si el jugador quiere adquirir el videojuego se le debe proporcionar el detalle del valor y no esperar a que él recurra a su memoria.
          .col-md-7
            figure
              img(src='@/assets/curso/tema3/8.png', alt='Texto que describa la imagen')
              figcaption Recordación
      .py-3.py-md-4(titulo="H7")
        .row
          .col-md-1
          .col-md-4.mb-4.mb-md-0
            h4 Flexibilidad y eficiencia de uso
            p Se refiere a la capacidad de utilización del producto independientemente del tipo de usuario; es decir, si a este se le facilita el uso de las herramientas tecnológicas o si, por el contrario, no le es sencillo ni familiar hacerlo.

            p Por ejemplo se puede poner un mensaje cuando pase el mouse por cada botón para indicar qué acción puede realizar en el juego.
          .col-md-7
            figure
              img(src='@/assets/curso/tema3/9.png', alt='Texto que describa la imagen')
              figcaption Indicador acciones realizar en el juego
      .py-3.py-md-4(titulo="H8")
        .row
          .col-md-1
          .col-md-4.mb-4.mb-md-0
            h4 Diseño minimalista
            p Es importante no saturar de información al usuario del producto, mostrándole contenido innecesario que lo distraiga y lo desvíe del objetivo de utilización del producto.

            p Por ejemplo las imágenes de las escenas deben contener pocos elementos para que el usuario entienda mejor las mecánicas del juego.
          .col-md-7
            figure
              img(src='@/assets/curso/tema3/10.png', alt='Texto que describa la imagen')
              figcaption Minimalista
      .py-3.py-md-4(titulo="H9")
        .row
          .col-md-1
          .col-md-4.mb-4.mb-md-0
            h4 Reconocer y corregir errores
            p Proporciona información al usuario de lo que está generando errores en la utilización del producto multimedia, y le brinda recomendaciones de las acciones que puede realizar para un buen uso del sistema. 

            p Por ejemplo, si el jugador desea descargar el videojuego y se presenta un problema, el sistema debe indicarle cuál fue el error.
          .col-md-7
            figure
              img(src='@/assets/curso/tema3/11.png', alt='Texto que describa la imagen')
              figcaption Errores
      .py-3.py-md-4(titulo="H10")
        .row
          .col-md-1
          .col-md-4.mb-4.mb-md-0
            h4 Ayuda y documentación
            p Se deben detectar las dudas más comunes de los usuarios cuando está usando el producto e incluir la información necesaria para que él mismo pueda encontrar la manera de resolverlas. De esta forma, el producto se hace auto gestionable.

            p Por ejemplo, incluir una explicación de cómo usar cada icono del juego haciendo clic en él.
          .col-md-7
            figure
              img(src='@/assets/curso/tema3/12.png', alt='Texto que describa la imagen')
              figcaption Ayudas
    p.mt-4 Para aplicar esta técnica se deben definir las heurísticas a evaluar y se llevan a cabo métricas de evaluación a través de una tabla de relevancia que mide la severidad del error o falla del producto y una tabla de frecuencia que determina cuántas veces ha fallado el producto en las heurísticas seleccionadas. En el ejemplo que se expone más adelante se verá con más detalle su aplicación.
    separador
    #t_3_2.titulo-segundo.color-acento-contenido
      h2 3.2 Modelo de indagación       
    p En este método se investiga acerca de lo que el usuario espera resolver con el producto, por eso es recomendable realizarlo en la fase de diseño y también en la fase de terminación, puesto que es en estos dos momentos, donde se verifica lo que el usuario necesita antes y lo que puede satisfacerlo cuando hace uso del producto. 
    .row.mt-4
      .col-lg-4
        .row.align-items-center
          .col-2
            img(src="@/assets/curso/tema1/i2.svg")
          .col-10
            h3.mb-0 Técnica de cuestionario
    p.mt-4 En esta técnica se puede seleccionar un grupo amplio de personas que podrán con testear las preguntas en tiempos diferentes y se puede realizar cuantas veces sea necesario; por ello es la más flexible de utilizar, incorporando varios tipos de preguntas: 
    .col-sm.mb-5.mb-sm-0.mt-5
      ol.lista-ol--cuadro.lista-ol--separador
        li 
          .lista-ol--cuadro__vineta
            span a
          |  Preguntas de tipo general: Son aquellas que ayudan a identificar el perfil del usuario como sexo, edad, nivel de educación, cargo que ocupa en la entidad, lugar de residencia, dirección, email, entre otras.

        li 
          .lista-ol--cuadro__vineta
            span b
          | Preguntas abiertas: Permiten recoger información de apreciación sobre algo en particular, interviene la parte subjetiva por que la respuesta es dada de acuerdo con el juicio del usuario, son útiles para atacar otros puntos de vista del producto.
        li 
          .lista-ol--cuadro__vineta
            span c
          | Preguntas cerradas: Permiten al usuario escoger entre varias opciones que se le presentan, por ello son más precisas y concretas, fáciles de tabular, graficar y analizar después, por ello se pueden obtener rápidamente los resultados. 
        li 
          .lista-ol--cuadro__vineta
            span d
          | Preguntas tipo escala: El usuario debe escoger una opción de una escala numérica. Por ejemplo: ¿la aplicación es comprensible? 
    .row.justify-content-center.mt-4
      .col-lg-8      
        img(src="@/assets/curso/tema3/13.png")      
    .col-sm.mb-5.mb-sm-0.mt-5
      ol.lista-ol--cuadro.lista-ol--separador        
        li 
          .lista-ol--cuadro__vineta
            span e
          |  Preguntas con opción múltiple: Se presentan al usuario varias opciones de respuesta a una pregunta dada, para solamente seleccione una. Por ejemplo: ¿cuál de las siguientes opciones le resultó más fácil de utilizar?                                                                
    .row.justify-content-center.mt-4
      .col-lg-8      
        img(src="@/assets/curso/tema3/14.png")            
    .row.mb-5.mt-5
      .col-md-6.col-lg.mb-5.mb-lg-0
        .tarjeta-avatar
          img(src='@/assets/curso/tema3/15.png' alt='AvatarTop')
          .tarjeta.color-acento-contenido
            .p-4
              h4.text-center Pre-tarea
              p.text-center Antes de que el usuario realice una tarea con el producto con el propósito de medir sus habilidades con el manejo de los sistemas informáticos.
      .col-md-6.col-lg.mb-5.mb-lg-0
        .tarjeta-avatar
          img(src='@/assets/curso/tema3/16.png' alt='AvatarTop')
          .tarjeta.color-acento-contenido
            .p-4
              h4.text-center Post-tarea

              p.text-center Después de que el usuario ha interactuado con alguna función del producto para medir su usabilidad.
      .col-md-6.col-lg.mb-5.mb-lg-0
        .tarjeta-avatar
          img(src='@/assets/curso/tema3/17.png' alt='AvatarTop')
          .tarjeta.color-acento-contenido
            .p-4
              h4.text-center Post-test

              p.text-center Después de que el usuario ha interactuado con todas las tareas que se le han planteado y se pueda medir su percepción global del producto.
    p.mt-4 Se pueden realizar cuestionarios en diferentes momentos:
    separador
    #t_3_3.titulo-segundo.color-acento-contenido
      h2 3.3 Modelo de test        
    .row.justify-content-center 
      .col-lg-10
        .bloque-texto-g.color-acento-contenido.p-3.p-sm-4.p-md-5
          .bloque-texto-g__img(
            :style="{'background-image': `url(${require('@/assets/curso/tema3/18.png')})`}"
          )
          .bloque-texto-g__texto.p-4
            p.mb-0 Este método se utiliza cuando se tiene el prototipo del producto, para lo cual el diseñador selecciona un grupo de usuarios a los que se les asignan diferentes tareas a ser ejecutadas para determinar cómo el sistema entrega los resultados de lo que se le está solicitando. Los resultados de esta prueba son utilizados para determinar si el diseño de las interfaces puede soportar las tareas que los usuarios están realizando con el producto.
    .row.mt-4
      .col-lg-4
        .row.align-items-center
          .col-2
            img(src="@/assets/curso/tema1/i2.svg")
          .col-10
            h3.mb-0 Técnica de test de prestaciones 
    p.mt-4 Esta técnica se utiliza para medir aspectos del uso del producto, por ello se debe llevar a cabo sobre el prototipo o sobre el producto terminado de tal forma que el evaluador pueda visualizar el número de errores que arroja el aplicativo, o las percepciones de los usuarios frente a lo que el producto lo puede beneficiar, por lo que se considera una técnica cuantitativa y cualitativa, en ella se debe: 
    .col-sm.mb-5.mb-sm-0.mt-5
      ol.lista-ol--cuadro.lista-ol--separador
        li 
          .lista-ol--cuadro__vineta
            span a
          |  Seleccionar usuarios reales o potenciales que realmente usarán el producto.

        li 
          .lista-ol--cuadro__vineta
            span b
          | Entregar instrucciones claras acerca de cómo presentar la prueba.
        li 
          .lista-ol--cuadro__vineta
            span c
          | Elaborar una lista de tareas que los usuarios realizarán con el producto y analizar la manera en que lo utilicen y el tiempo que tardan en ejecutar cada tarea asignada.
        li 
          .lista-ol--cuadro__vineta
            span d 
          | Observar el comportamiento del usuario durante la prueba.
        li 
          .lista-ol--cuadro__vineta
            span e
          | No entregar pistas ni orientaciones al usuario de cómo usar o recorrer la aplicación/producto.
        li 
          .lista-ol--cuadro__vineta
            span f 
          | Grabar las expresiones del usuario y la forma de usar la aplicación o el producto.
        li 
          .lista-ol--cuadro__vineta
            span g 
          | Analizar los datos recolectados en la ejecución de las tareas, los problemas detectados para llevar a cabo soluciones que mejoren la usabilidad del producto.
    separador
    #t_3_4.titulo-segundo.color-acento-contenido
      h2 3.4 Ejemplo de aplicación
    p Partiendo del supuesto que el equipo de diseño ha creado un juego llamado “La isla de los tesoros escondidos” en este, el jugador debe encontrar tesoros escondidos en diferentes puntos de la isla, a los que se debe llegar haciendo la búsqueda y superando obstáculos. Si el jugador está muy perdido puede solicitar pistas pagando mucho dinero.
    p El equipo ha decidido hacer pruebas de usabilidad aplicando los siguientes modelos y técnicas:
    .row.justify-content-center 
      .col-lg-6
        img(src="@/assets/curso/tema3/19.svg")            
    p.mt-3 Antes de empezar las pruebas, el equipo debe definir con exactitud:
    SlyderF.mb-5(columnas="col-lg-6 col-xl-4")
      .tarjeta.color-secundario.p-4
        .row.justify-content-center.mb-3
          .col-8
            img(src='@/assets/curso/tema3/x1.png' alt='AvatarTop')
        h4.text-center Objetivo de la prueba
        p.text-center Es el propósito que condujo a la aplicación de la evaluación ya que hay muchos aspectos que se pueden medir en los productos o aplicativos informáticos en general y se debe especificar a cuál de ellos le apuntará las pruebas que se realicen.
      .tarjeta.color-secundario.p-4
        .row.justify-content-center.mb-3
          .col-8
            img(src='@/assets/curso/tema3/x2.png' alt='AvatarTop')
        h4.text-center Participantes
        p.text-center Se deben definir las características o competencias que deben cumplir los usuarios para la realización de las pruebas, ya que estos deben ser seleccionados basados en ellas. Dichas características deben ser similares y se recomienda un número de participantes aproximadamente de ocho (8), ya que como dice Nielsen citado por Vega (s. f.) entre más usuarios participen más repetición de resultados se obtendrán, pero esto lo define el equipo de evaluadores de acuerdo con su conveniencia.
      .tarjeta.color-secundario.p-4
        .row.justify-content-center.mb-3
          .col-8
            img(src='@/assets/curso/tema3/x3.png' alt='AvatarTop')
        h4.text-center Descripción de la técnica utilizada 
        p.text-center La técnica que se llevará a cabo debe quedar clara para los participantes al igual que el instrumento que se utilice para la medición. Por ejemplo, las tareas a ejecutar deben ser completamente comprensibles para los usuarios, se deben definir con exactitud las H (heurísticas) que se van a evaluar y las preguntas que contestarán no pueden tener rastros de ambigüedad.
      .tarjeta.color-secundario.p-4
        .row.justify-content-center.mb-3
          .col-8
            img(src='@/assets/curso/tema3/x4.png' alt='AvatarTop')
        h4.text-center Análisis de resultados
        p.text-center Después de aplicadas las pruebas el equipo debe analizar los resultados obtenidos y determinar cuáles son los aspectos que se deben mejorar en el producto para que la experiencia de usuario sea satisfactoria por cumplir con las condiciones de fácil uso.
    .row.justify-content-center 
      .col-lg-10.mt-4
        .cajon.color-acento-contenido.p-4.mb-4
          p Participantes: se convocaron 4 usuarios que les llama la atención los videojuegos por lo que han jugado alguna vez y poseen entre 18 y 22 años, poseen habilidades tecnológicas por las ocupaciones de estudio y trabajo.
    .row.mt-4
      .col-lg-5
        .row.align-items-center
          .col-1
            img(src="@/assets/curso/tema1/i2.svg")
          .col-11
            h3.mb-0 Primera técnica de usabilidad: heurística
    p.mt-4 Esta técnica se utiliza para medir aspectos del uso del producto, por ello se debe llevar a cabo sobre el prototipo o sobre el producto terminado de tal forma que el evaluador pueda visualizar el número de errores que arroja el aplicativo, o las percepciones de los usuarios frente a lo que el producto lo puede beneficiar, por lo que se considera una técnica cuantitativa y cualitativa, en ella se debe: 
    .col-sm.mb-5.mb-sm-0.mt-5
      ol.lista-ol--cuadro.lista-ol--separador
        li 
          .lista-ol--cuadro__vineta
            span a
          |  Objetivo de la prueba: En el videojuego de “La isla de los tesoros escondidos” el equipo de diseño y desarrollo deberá determinar si la interfaz de usuario presenta saturación de imágenes y si el jugador puede tomar el control del juego con facilidad a través de las diferentes funciones que posee.


        li 
          .lista-ol--cuadro__vineta
            span b
          | Descripción de la técnica: para evaluar los aspectos definidos en el objetivo se utilizará la técnica heurística con la definición de las siguientes H: 
    .tarjeta--container.row.mb-5
      .col-md.tarjeta.color-acento-contenido.p-5
        .row.justify-content-center.mb-4
          .col-6
            figure
              img(src='@/assets/curso/tema3/h1.svg', alt='Texto que describa la imagen')
          
        h2.text-center.text-white Consistencia
        p.text-center.text-white Está limitado por el Fillrate o tasa de relleno que determina, en esencia, la cantidad de píxeles que la tarjeta gráfica es capaz de dibujar o renderizar, procesar y almacenar, por cada unidad de tiempo.

      .col-md.tarjeta.color-primario.p-5
        .row.justify-content-center.mb-4
          .col-6
            figure
              img(src='@/assets/curso/tema3/h2.svg', alt='Texto que describa la imagen')
          
        h2.text-center Diseño minimalista
        p.text-center Está limitado por el número de Batches o lotes de información gráfica que necesita ser renderizada. En términos generales, se remite al cálculo por el procesador de la máquina y el almacenamiento de información en memoria RAM.
    p.mt-3 Según Fernández (2019), la métrica de evaluación del método heurístico es la que utiliza Nielsen: 
    TabsA.color-acento-contenido.mb-5
      .tarjeta.color-secundario.p-4(titulo="Relevancia del problema")
        .row 
          .col-lg-8
            h4 Relevancia del problema
            p En esta tabla se observa el grado de severidad de un problema presentado con el producto, siendo el más alto (4) cuando el problema es bloqueante o le impide al usuario seguir adelante con otra función, es grave (3) cuando el usuario puede utilizar alguna otra función del producto, es menor (2) cuando puede operar el producto aunque presente algunos inconvenientes, es cosmético (1) cuando el producto es utilizable y funcional aunque requiera en algún momento de realizar cualquier tipo de actualización para su óptimo funcionamiento, y no supone problema (0) cuando el producto funciona correctamente.

          .col-lg-4
            img(src='@/assets/curso/tema3/z1.png', alt='Texto que describa la imagen')

      .tarjeta.color-secundario.p-4(titulo="Frecuencia del problema")
        .row 
          .col-lg-8
            h4 Frecuencia del problema
            p Aquí se observa la frecuencia con que la heurística no satisface al usuario y le asigna una calificación, es decir que si se obtuvo un 4 es porque más del 90% de las veces el producto presenta fallas, si es de 3 es porque entre el 50% y el 90% el producto no cumple con lo esperado por algún tipo de problemas, si es de 2 quiere decir el producto presenta problemas entre el 10% y 25% de las veces en que es utilizado, y si es 0 el producto falla máximo el 10% de las veces y se puede considerar que tiene un buen funcionamiento. 
            
          .col-lg-4
            img(src='@/assets/curso/tema3/z2.png', alt='Texto que describa la imagen') 
      .tarjeta.color-secundario.p-4(titulo="Heurísticas")
        .row 
          .col-lg-8
            h4 Heurísticas
            p Las afirmaciones diseñadas para cada heurística también pueden ser preguntas si se desea. De acuerdo con las pruebas, el número de veces que se puede dar la falla en la toma del control del videojuego (H4) es cinco (5), ya que es la cantidad de veces que se prueba la afirmación y el número de veces que consideran los usuarios se falla por el exceso de imágenes es de tres (3). El porcentaje se halló dividiendo el número de veces de la falla entre el máximo número de fallas el cual es ocho (8). Si se trasladan los resultados a las tablas de relevancia y frecuencia se obtiene:
          .col-lg-4
            img(src='@/assets/curso/tema3/z3.png', alt='Texto que describa la imagen') 
      .tarjeta.color-secundario.p-4(titulo="Nivel de gravedad y número de reiteraciones")
        .row 
          .col-lg-8
            h4 Nivel de gravedad y número de reiteraciones
            p En estas dos tablas se observa que, de acuerdo con lo establecido respecto a la relevancia y la frecuencia, el problema con mayor prioridad está en la heurísticas H4 de consistencia con la falla para tomar el control del juego cuando se interacciona con él. La heurística H8 representa un problema menor para el producto, ya que se considera que solo el 38% de la muestra considera que hay exceso de imágenes. Lo anterior quiere decir que el aspecto prioritario a modificar en el producto está en la elaboración de controles más sencillos, siguiendo un patrón de colores o estilos para hacerlo más comprensible y funcional para el jugador.
          .col-lg-4
            img(src='@/assets/curso/tema3/z4.png', alt='Texto que describa la imagen') 
    .row.mt-4
      .col-lg-5
        .row.align-items-center
          .col-1
            img(src="@/assets/curso/tema1/i2.svg")
          .col-11
            h3.mb-0 Segunda técnica de usabilidad: cuestionario
    .col-sm.mb-5.mb-sm-0.mt-5
      ol.lista-ol--cuadro.lista-ol--separador
        li 
          .lista-ol--cuadro__vineta
            span a
          |  Objetivo de la prueba: en el videojuego de “La isla de los tesoros escondidos” el equipo de diseño y desarrollo deberá determinar si la interfaz de usuario presenta una estructura sencilla con una interacción clara, buena calidad de imágenes sin saturación de ellas y sonidos acordes a las situaciones presentadas.


        li 
          .lista-ol--cuadro__vineta
            span b
          | Descripción de la técnica: para evaluar los aspectos definidos en el objetivo se utilizará la técnica de cuestionario con la definición de las siguientes preguntas:

    .row.justify-content-center 
      .col-lg-6
        img(src='@/assets/curso/tema3/20.png', alt='Texto que describa la imagen') 
    p.mt-4 En el cuestionario anterior se observan diferentes tipos de preguntas; cerradas y abiertas para un análisis de tipo cuantitativo y cualitativo. Cuando se tiene las respuestas de los participantes, se hace una tabulación usando la herramienta ofimática de Excel para la obtención de los resultados. Al igual que el método heurístico se obtienen los porcentajes de las respuestas con preguntas cerradas y en las abiertas se tienen en cuenta todas las observaciones realizadas, por ello, el número de participantes debe ser pequeño. De acuerdo con los porcentajes y las observaciones se priorizan los aspectos con mayor porcentaje de negatividad y deficiencia para realizar las modificaciones y se ejecutan los cambios que requiere cada comentario insatisfactorio de los usuarios.
    .row.mt-4
      .col-lg-5
        .row.align-items-center
          .col-1
            img(src="@/assets/curso/tema1/i2.svg")
          .col-11
            h3.mb-0 Tercera técnica de usabilidad: test de prestación 
    .col-sm.mb-5.mb-sm-0.mt-5
      ol.lista-ol--cuadro.lista-ol--separador
        li 
          .lista-ol--cuadro__vineta
            span a
          |  Objetivo de la prueba: en el videojuego “La isla de los tesoros escondidos” el equipo de diseño y desarrollo deberá identificar las fallas en las funciones de búsqueda, entrega de pistas, cancelación de una búsqueda, registrarse para obtener beneficios y conexión con otro jugador.

        li 
          .lista-ol--cuadro__vineta
            span b
          | Descripción de la técnica: para evaluar los aspectos definidos en el objetivo se utilizará la técnica de test de prestación, utilizando un formato en el que los participantes diligenciarán datos personales básicos y estarán frente al producto terminado realizando la lista de tareas que se indica y anotando los eventos de éxito o de error que perciben en las funcionalidades que se le solicita probar: 
    p.mt-4 Los formatos diligenciados por los participantes son analizados y verificados por el equipo desarrollador para proceder a la corrección de las fallas presentados y volver a realizar la prueba que comprueben las mejoras en la funcionalidad del producto. 
    p Si se quiere profundizar en las demás técnicas de cada modelo se recomienda la siguiente lectura complementaria:
    .row.justify-content-center.mt-4
      .col-lg-10
        .tarjeta.color-primario.p-3.mb-5.mt-5
          .row.justify-content-around.align-items-center
            .col-3.col-sm-2.col-lg-1
              img(src="@/assets/curso/tema1/i3.svg")
            .col
              .row.justify-content-between.align-items-center
                .col.mb-3.mb-sm-0
                  h3.mb-1 Lectura de consulta
                  p.text-small Si se quiere profundizar en las demás técnicas de cada modelo se recomienda la siguiente lectura complementaria:
                .col-sm-auto
                  a.boton.color-acento-botones.texto-blanco(:href="obtenerLink('downloads/prueba.pdf')" target="_blank")
                    span Ver video
                    i.fas.fa-file-download

</template>

<script>
export default {
  name: 'Tema3',
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
.bloque-texto-b.color-acento-contenido:before
  background-color: #F1EFFE
</style>
