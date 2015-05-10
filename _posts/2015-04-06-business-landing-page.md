---
layout: post
title:  "Issue 2 // Business Landing Page"
date:   2015-04-06
---

### Full Screen Landing Pages

Los sitios modernos tienen secciones <em>full-screen</em> en sus páginas de inicio — home —. Y si no son <em>full-screen</em>, al menos toman el 80 o 90% del total de la pantalla, y en ciertas ocasiones utilizan pequeños <em>hacks</em> con JavaScript — horrible — para hacer que ese efecto tenga la funcionalidad deseada.

Para dar un ejemplo de lo que estoy hablando aquí hay unos casos que estuve investigando de sitios web que usan esta técnica.

<figure>
	<img src="{{ site.url }}/assets/img/everybodyscroll.gif" alt="Everybody scroll!"> 
	<figcaption>Fig1. - Tendencia actual de Landing Pages</figcaption>
</figure>

### spotify.com
Ellos usan <em>data-attributes</em> para guardar las proporciones del <em>layout</em>, yo no lo haría así pero el objetivo no es criticar el trabajo, sino ver la técnica en acción.

<figure>
	<img src="{{ site.url }}/assets/img/spotify.png" alt="spotify.com"> 
	<figcaption>Fig2. - Página principal de spotify.com</figcaption>
</figure>

### exposure.co
Exposure mantiene una altura del 90% en la sección principal y enseguida cambia el tamaño con un poco de JavaScript.

<figure>
	<img src="{{ site.url }}/assets/img/exposure.png" alt="exposure.co"> 
	<figcaption>Fig3. - Página principal de exposure.co</figcaption>
</figure>

### nimber.com
Nimber usa una técnica similar a <a href="https://www.spotify.com">spotify.com</a>. La altura de la primera sección es establecida por default al 90% pero las demás secciones mantienen un <em>min-height</em> para asegurarse que son más grandes que el <em>viewport</em>, esto trae como consecuencia que en la versión <em>desktop</em> sean secciones más grandes pero, para la versión mobile se muestren correctamente. ¡Un gran truco!

<figure>
	<img src="{{ site.url }}/assets/img/nimber.png" alt="nimber.com"> 
	<figcaption>Fig4. - Página principal de nimber.com</figcaption>
</figure>


### flickr.com
Yahoo salió temprano al mercado en este año, modernizó su sitio con una de las tendencias actuales del diseño web, y vaya que lo hicieron muy bien. Ellos se evitaron el problema de establecer una altura de 90% abarcando todo el <em>viewport</em>, es decir, el 100%. Ofrece una gran usabilidad (UX) al usuario y está enfocado directamente en el producto, incluso tienen la teoría del <em>call-to-action</em> que indica al usuario acceder a más detalles del producto como acción a desarrollar, interpretan muy bien esta teoría, una <strong>Landing Page</strong> tiene que vender, es la principal cara del producto — o empresa —.

<figure>
	<img src="{{ site.url }}/assets/img/flickr.png" alt="flickr.com"> 
	<figcaption>Fig5. - Página principal de flickr.com</figcaption>
</figure>

<hr>
Todos esos ejemplos mostrados están usando JavaScript para realizar esa técnica, y está bien, sólo es una Landing Page que muestra el <em>call-to-action</em> al producto, no hay de que preocuparse sobre el <em>performance</em> de la aplicación, pero ¿y si podemos evitar eso usando solo <strong>CSS</strong>? Sé que en velocidad serán unos cuantos milisegundos la diferencia, pero en un mercado como este cada milisegundo cuenta, además no es verificar cuánta velocidad estamos obteniendo, sino mejorar la Experiencia de Usuario (UX) y Usabilidad que tiene el cliente al navegar por el sitio.

Me pondré un poco técnico, para realizar este técnica con CSS bastaría una simple línea — estoy exagerando —...

{% highlight css %}
.section { height: 100vh; }
{% endhighlight %}

Sí, <strong>viewport height, 1vh = 1%</strong> de la altura del navegador. Sin ningún esfuerzo, la imagen se adaptará a la altura del navegador, y estaría cubriendo el RWD — responsive web design —. He estado trabajando con ejemplos el fin de semana y he logrado adaptarme a la técnica usando solo CSS, una gran mejora en <em>performance</em>.

### ¿Por qué mejora en performance?
Haciendo esta técnica con CSS evitamos el llamado JavaScript, y solo trabajaría con <em>snippets CSS</em>, manteniendo en control todo el código de un solo lado — el mío —, obteniendo como resultado una mejor guía de estilo para cualquier que desee modificar el proyecto.

Ahora, digamos que se necesita que la primera sección abarque solo el 90% de altura, y todas las demás el 100%, para hacer esto no necesitaría JavaScript, con CSS podría realizar esto y cuidando el <em>performance</em>, siempre enfocado en eso. Bastaría con...

{% highlight css %}
.section { height: 100vh; }
.section--first { height: 90vh; }
{% endhighlight %}

## Muy bien, ¿y la compatibilidad de navegadores?
Investigando en las especificaciones de cada unidad de medida con sus referentes navegadores, en promedio existe un 78.38% de compatibilidad entre todos, incluso con soporte para IE9+, aquí una muestra del estudio:

<figure>
	<img src="{{ site.url }}/assets/img/crossbrowser.png" alt="Compatibilidad"> 
	<figcaption>Fig6. - Compatibilidad entre navegadores</figcaption>
</figure>

Suena muy lindo para ser real, pero esa es la verdad. No se tendrían problemas para implementar esta técnica.

### 6wunderkinder.com
Los chicos detrás de <a href="https://www.wunderlist.com/es/">wunderlist</a> usan un <em>background fixed</em> para posicionar el header, eso te da la posibilidad de posicionar las demás secciones al 100% del <em>viewport</em>. Es un enfoque diferente pero lo hacen sin ningún código JavaScript. ¡Bien por ellos!

<figure>
	<img src="{{ site.url }}/assets/img/6wunderkinder.png" alt="6wunderkinder.com"> 
	<figcaption>Fig7. - Página principal de 6wunderkinder.com</figcaption>
</figure>

## ¿Por qué me interesa saber esto?
He expuesto un poco de teoría combinada con resultados actuales con el fin de mostrar que la <em>business page</em> de Travelnet no está <em>up-to-date</em>, estamos perdiendo por ese lado y obviamente no se permite eso en el nuevo diseño, así que hemos investigado qué técnica sería eficiente para la nueva página de Travelnet y nos hemos decidido por aplicarla, aquí el resultado:

<figure>
	<img src="{{ site.url }}/assets/img/businesslanding.jpg" alt="Business Landing Page"> 
	<figcaption>Fig8. - Business Landing Page de Travelnet.com, en construcción...</figcaption>
</figure>

<figure>
	<img src="{{ site.url }}/assets/img/old_business.png" alt="Página actual"> 
	<figcaption>Fig9. - Página actual de Travelnet, no cuenta una historia.</figcaption>
</figure>

Aún está bajo desarrollo, pero poco a poco vamos adaptando las nuevas técnicas no sin antes haber realizado la investigación correcta.
Incluso hay un <a href="http://www.hugeinc.com/ideas/perspective/everybody-scrolls">estudio</a> donde indica que todos están realizando el scroll — <em>everybody scroll</em> —.

## ¿Que queremos lograr?
Un cliente no necesita saber con exactitud cómo funciona el motor de Travelnet — lo comento porque el diseño actual muestra detalles que son importantes, pero no necesarios para el cliente —, ni como realiza las reservaciones, pero sí necesita saber que Travelnet es una de las mejores opciones en el mercado, y con esta técnica le estamos contando una historia al cliente para atraparlo, es decir, con cada <em>scroll</em> — desplazamiento — que realiza va conociendo un poco más sobre el motor sin ponernos tan técnicos en el tema, solo en la Experiencia — UX — que le estamos brindando. Por que al final del día de eso se trata, de contar una historia que envuelva al cliente, que lo haga sentir confiado y que está utilizando unos de los sistemás más actualizados en estos días — comparando con la competencia —, la competencia ni siquiera ha pensado en esto, es una parte importante en el diseño porque la <em>landing page</em> será la cara del nuevo diseño, aquella que logre atrapar a los usuarios y los anime a unirse y ser parte de este gran equipo.

<figure>
	<img src="{{ site.url }}/assets/img/despegar.png" alt="despegar.com"> 
	<figcaption>Fig10. - despegar.com no tiene Landing Page</figcaption>
</figure>

<figure>
	<img src="{{ site.url }}/assets/img/trivago.png" alt="trivago.com.mx"> 
	<figcaption>Fig11. - trivago.com.mx</figcaption>
</figure>

La simplicidad es muy difícil, todos los sabemos. Pero algunas veces lo que parece una simple solución resulta ser la peor, algunas veces un diseño simple no es necesariamente un diseño fácil de usar.

El objetivo de estas publicaciones es dar a conocer a todo el equipo de Travelnet y MIG las situaciones diarias a las que nos enfrentamos, los análisis rigurosos que realizamos a la competencia, los casos de estudios que investigamos, los <em>sketches, bosquejos, prototipos, e ideas</em> que desarrollamos, cómo es nuestro proceso de diseño, e informar las soluciones que presentamos porque que estamos trabajando en un producto que pretende ser competencia directa de unas cuantas soluciones ya en línea. Y también mostrar que todo en el diseño tiene su porqué, tiene la investigación suficiente.