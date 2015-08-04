---
layout: post
title:  "Issue 5 // Re-diseño [Concepto]"
date:   2015-08-04
---

Éste nuevo re-diseño es una herramienta de conciencia. El objetivo es proveer a la sociedad <strong>informacion objetiva</strong> acerca de un evento o acción, <em>[call-to-action]</em>(https://boagworld.com/design/10-techniques-for-an-effective-call-to-action/).

En realidad, la nueva búsqueda está sujeta a prioridades, actitudes y comportamiento. Permite organizar los eventos y evitar las inconsistencias en la cobertura de los mismos eventos (promociones) con múltiples <em>brokers</em>.

Al día de hoy, hay demasiada información, y mucha de ella depende de sí misma. El "punto de vista" de cada una es muy significante, algo que en el actual Travel no se esfatiza, y mucho menos se enfoca en los resultados.

Se ha vuelto muy difícil entender el flujo de la información. Para la opinión personal, es un tremendo reto buscar un hotel.

> Este problema nos ha permitido idear una idea que permite agilizar la lectura y búsqueda de resultados, enfocando la energía en el contenido de los eventos (promociones).

<figure>
	<img src="{{ site.url }}/assets/img/google-news.jpg" alt="Resultados de Google News"> 
	<figcaption>Fig1. - Resultados de Google News</figcaption>
</figure>

## Investigación

Como la mayoria de los servicios que ofrece Travel, la búsqueda múltiple que realiza es una gran hazaña, pero no sirve de nada generar buenos resultados y las mejores promociones si el producto no ofrece una usabilidad.

### Análisis del sitio actual

El sitio actual se enfoca en solo mostrar resultados, identificar las debilidades fue fácil. Para la época en que salió Travel y la época en que estamos, los usuarios demandan más usabilidad y tener un <em>[story telling]</em>(https://medium.com/about/storytelling-for-good-cac0f81cd79a) muy fuerte.

<figure>
	<img src="{{ site.url }}/assets/img/travel-debilidades.png" alt="Debilidades del Travel actual"> 
	<figcaption>Fig2. - Debilidades del Travel actual</figcaption>
</figure>

### Casos de uso

Comprendiendo la audiencia que tenemos, hemos tomado 4 casos de uso y se ha analizado las necesidades que tendría cada uno al conocer el sitio, nos ha permitido generar <strong>qué funciones serían más útiles</strong>.

<table>
	<thead>
		<tr>
			<th>
				Oliver, 23 años.<br/>
				<em>Estudiante</em>
			</th>
			<th>
				Alberto, 28 años.<br/>
				<em>Ingeniero</em>
			</th>
			<th>
				Olga, 36 años.<br/>
				<em>Abogada</em>
			</th>
			<th>
				Liliana, 56 años.<br/>
				<em>de la vieja escuela</em>
			</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>
				Oliver no está interesado en la búsqueda, en reservar un hotel, algunas veces él le solicita a la secretaria de su papá que realice ese trámite por él. O algunas veces a los profesores. Analicemos qué acciones podría realizar dentro de Travel:<br/><br/>
				
				― Ordenar los resultados <br/>
				― Buscar por ciudad <br/>
				― Leer las promociones (<em>Oh! No sabe donde están.</em>) <br/>
				― Abrir algún resultado sin reservar hotel <br/>
				― No reservó <br/>
				</ul>
			</td>
			<td>
				Alberto siempre ha ocupado grandes motores de búsqueda de hoteles, y por obviedad siempre ha reservado. Él es un usuario que podría ayudarnos mucho en ejemplificar la usabilidad. ¿Que podría hacer un ingeniero como él en Travel? <br/><br/>
				
				― Ordenar por categoria <br/>
				― Guardar los resultados que más le agraden<br/>
				― Crear una lista de Hoteles<br/>
				― Buscar por Hotel<br/>
				― Comentar, preguntar dudas.<br/>
				― Seguir buscando y probando suerte.<br/>
				― Ordenar por fecha<br/>
				― Ajustar su página principal, para mostrar solo las promociones que le interesan.<br/>
				― Mostrar llos hoteles disponibles en el día actual sin tener que seleccionar la fecha.<br/>
			</td>
			<td>
				Olga está interesada solo en las leyes, cambios y pensamientos de políticos poderosos. También está interesada en asistir a una conferencia a USA. Pero no tiene mucha idea de como buscar un hotel y algún vuelo, si es que se anima a reservar con Travel.<br/><br/>
				
				― Selecciona fecha actual para buscar hoteles<br/>
				― Busca por hoteles, por destino.<br/>
				― Le gustaría buscar por mapa.<br/>
				― No habla español<br/>
				― Ajustar la búsqueda, ordenar por precio<br/>
				― Está encantada por la sección de filtros<br/>
			</td>
			<td>
				Liliana le tiene miedo a las computadoras pero no tiene otra salida, necesita visitar a sus hijos en Europa y ella tiene que reservar el vuelo y el hotel. Ya ha reservado hoteles, pero ésta es la primera vez que lo hace sola.<br/><br/>
				
				― Buscar hotel<br/>
				― Seleccionar fecha<br/>
				― No le gusta el color actual<br/>
				― Al ver los resultados se espanta, le gustaría enfocarse en la oferta del día<br/>
				― Ordenar por precio<br/>
				― No tiene mucha idea de donde está el hotel<br/>
				― Seguir buscando hotel<br/>
				― Está a punto de reservar un vuelo<br/>
				― Al final, ha optado por decirle a sus hijos que le reserven el vuelo y el hotel, ha quedado frustrada porque dice que las computadoras no son para ella y se siente "dejada" por la tecnología<br/>
			</td>
		</tr>
	</tbody>
</table>

<figure>
	<img src="{{ site.url }}/assets/img/user-cases.png" alt="Casos de Uso Google News"> 
	<figcaption>Fig3. - Casos de Uso Google News</figcaption>
</figure>

### Features

Basado en el análisis de los casos presentados anteriores, se ha tenido una pequeña sesión de las características que les gustaría a los usuarios poder manejar, las innovaciones han sido separadas en dos categorias: funcional y visual.

<figure>
	<img src="{{ site.url }}/assets/img/research-features.png" alt="Features del nuevo diseño"> 
	<figcaption>Fig4. - Features del nuevo diseño</figcaption>
</figure>

### Distintos escenarios
<figure>
	<img src="{{ site.url }}/assets/img/research-user-scenarios.png" alt=""> 
	<figcaption>Fig5. - Escenarios evaluados por UX People de Google</figcaption>
</figure>

## Principios UX

> Desde que los re-diseños se han enfocado en el usuario, en proveer lo que realmente necesita; la principal meta es simplificar la búsqueda, y minimizar el número de pasos que el usuario necesita para completar una tarea.

### Sketches, Wireframes
Una vez definidas las metas y los instrumentos para re-diseñar, es necesario empezar con sketches, papel y lapiz. Esto sirve para determinar el contenido de la página y el orden de los elementos.

<figure>
	<img src="{{ site.url }}/assets/img/plan.jpg" alt=""> 
	<figcaption>Fig6. - Papel, lápiz e ideas plasmadas</figcaption>
</figure>

<figure>
	<img src="{{ site.url }}/assets/img/ux-sketches-1.png" alt="Sketches, Wireframes">
</figure>

<figure>
	<img src="{{ site.url }}/assets/img/ux-sketches-2.png" alt="Sketches, Wireframes">
</figure>

<figure>
	<img src="{{ site.url }}/assets/img/ux-sketches-3.png" alt="Sketches, Wireframes">
</figure>

<figure>
	<img src="{{ site.url }}/assets/img/ux-sketches-4.png" alt="Sketches, Wireframes">
</figure>

### Panel

Al crear <em>wireframes</em> hemos coleccionado una serie de ventajas comparando las grandes marcas y tratando de copiar lo mejor de ellos, hemos diseñado un <em>board</em> enfocado en resultados de hoteles y promociones.
Esto ayuda a crear una mejor experiencia de usuario y también una idea de cómo se irá diseñando.

<figure>
	<img src="{{ site.url }}/assets/img/mood.png" alt="Páneles de distintas colores, sabores y diseños"> 
	<figcaption>Fig7. - Páneles de distintas colores, sabores y diseños</figcaption>
</figure>

### Tipografía, Grid

Para la tipografía normal, elegimos [Myriad Pro](https://en.wikipedia.org/wiki/Myriad_(typeface)) la cual representa la perfecta simplicidad para Travel. Para resultados elegimos [Trebuchet MS](https://en.wikipedia.org/wiki/Trebuchet_MS), está enfocada mucho más en párrafos.

El <em>grid</em> que utilizamos está elaborado con 12 columnas, y 8 pixeles de base. Uno de los <em>grid</em> más típicos pero no mejor empleados, con el enfoque en resultados el <em>grid</em> de 12 columnas es perfecto para nuestra idea.


<figure>
	<img src="{{ site.url }}/assets/img/typography-1.png" alt="tipografía"> 
	<figcaption>Fig8. - Evaluación de la tipografía seleccionada</figcaption>
</figure>

<figure>
	<img src="{{ site.url }}/assets/img/typography-2.png" alt="grid"> 
	<figcaption>Fig9. - El grid</figcaption>
</figure>

## Diseño, Funcionalidad, Usabilidad

> Después de una intensa investigación, muchas horas de nuestro tiempo libre y gran cantidad de tazas de café, nos tomó solo 2 semanas conjuntar todo y crear un diseño, el diseño será <em>fully-responsive</em> y no hay mejor idea para representar el futuro de una compañía que se dedica a obtener los mejores resultados en reservaciones.

<figure>
	<img src="{{ site.url }}/assets/img/design.jpg" alt="Nuevo diseño"> 
	<figcaption>Fig10 - Nuevo diseño</figcaption>
</figure>


## Responsive sin limitaciones

<figure>
	<img src="{{ site.url }}/assets/img/macbook.jpg" alt="Versión Desktop"> 
	<figcaption>Fig13. - Versión Desktop</figcaption>
</figure>

<figure>
	<img src="{{ site.url }}/assets/img/mversion.jpg" alt="Versión iPad y  Móvil"> 
	<figcaption>Fig14 - Versión iPad y  Móvil</figcaption>
</figure>


### Nota

Este re-diseño es idea nuestra, y fue hecho solo para propósitos de estudio y no se supone que sea desarrollado o implementado en Travel, tal vez para alguna idea que lleguemos a tener más adelante. El re-diseño contiene ideas propias.