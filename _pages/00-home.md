---
layout: home
title: Coala - Activismo Vegano
permalink: /
---

<section id="cover">
  <img src="assets/cover-1024.jpg"
    srcset="assets/cover-1024.jpg 1024w, assets/cover-1920-800.jpg 1920w"
class="img-fluid" alt="Responsive image">
</section>

<div class="container">

<section id="quienes-somos">
  
  <h2 class="section-header">¿Quiénes somos?</h2>

  <p>Somos una organización de voluntarios sin ánimo de lucro fundada en la Ciudad de La Plata.
  <abbr title="Colectivo Abolicionista por la Liberación Animal">Coala</abbr>
  nació en Agosto de 2013 y a partir de entonces busca, a través de un activismo constante y comprometido,
  ponerle fin a la explotación animal.</p>

  <article class="vision">
    <strong>Nuestra visión:</strong>
    <p class="important">Un mundo sin explotación animal.</p>
  </article>

  <p class="mision"><strong>Nuestra misión:</strong> Concientizar a las personas sobre la grave problemática de la explotación animal, alentarlas a hacerse veganas, acompañarlas en su transición e inspirarlas a involucrarse a través de activismo vegano efectivo y no violento.</p>

</section>

<section id="problematica">

  <h2 class="section-header">Problemática</h2>

  <div class="row">
    <div class="col-lg-6 col-sm-12">
      <section class="bg-content bg-green-alpha problematica-principal text-center">

        <p>La mayoría de las personas estamos de acuerdo en que está mal causar <strong> sufrimiento innecesario y muerte </strong> a los animales. O por lo menos que no deberíamos hacerlo meramente porque obtengamos placer o diversión, porque sea conveniente, o porque sea una simple costumbre.</p>

        <i class="fa fa-paw "></i>

        <p>Pero casi todo el uso que se les da a los animales no puede justificarse por otra razón que no sea placer, entretenimiento, conveniencia o hábito.</p>
      </section>
    </div>
  </div>
</section>



<section id="problematica2">
  <div class="problematica-principal">
    <p>Los animales son usados por los seres humanos para producción de vestimenta y alimentos, para testeo de productos médicos y cosméticos, para transporte de personas y de cargas pesadas, y para exposición en zoológicos y acuarios.</p>
  
    <p>También con fines de entretenimiento en circos, corridas de toros, peleas de perros y doma, deportes tales como la pesca y las carreras, y con fines bélicos, entre otros.</p>
         
    <p>Todos estos usos resultan en sufrimiento y muerte a los animales, y son totalmente innecesarios.</p> 
  </div>
</section>





<section id="realidad">

<h2 class="section-header">Explotación animal</h2>

<div class="row">

<div class="col-md-3 col-sm-12 hidden-sm-down">
<ul id="menu-realidad" class="nav nav-tabs nav-stacked">
{% for p in site.pages %}
  {% if p.kind == 'explotacion' %}  
    <li class="nav-item{% if p.number == 2 %} active{% endif %}">
      <a class="nav-link" data-toggle="tab" href="#{{ p.url | remove:'/'}}">
        {{ p.title }}
      </a>
    </li>
  {% endif %}
{% endfor %}
</ul>
</div>

<div class="col-md-9 col-sm-12">
<section id="myTabContent" class="tab-content">
{% for p in site.pages %}
  {% if p.kind == 'explotacion' %}

  {% assign post_index0 = forloop.index0 %}
  {% assign post_index1 = forloop.index %}

    <div class="tab-pane fade {% if p.number == 2 %}active in{% endif %}" id="{{ p.url | remove:'/'}}">
      <div class="content bg-content">

        {% for post in site.pages %}
          {% if post_index0 == forloop.index  %}
            {% assign prev_post_id = post.url | remove:'/' %}
            {% assign prev_post_title = post.title %}
          {% endif %}
          {% if post_index1 == forloop.index0 %}
            {% assign next_post_id = post.url | remove:'/' %}
            {% assign next_post_title = post.title %}
          {% endif %}
        {% endfor %}

        <nav id="paginador-realidad" class="hidden-md-up">
          <ul class="pager">
            {% if prev_post_id and forloop.index > 3 %}
              <li class="pager-prev">
                <a data-toggle="tab" href="#{{ prev_post_id }}">
                ← <span class="pager-page-title">{{ prev_post_title }}</span>
                </a>
              </li>
            {% endif %}
          
            {% if next_post_id and forloop.index < 9 %}
              <li class="pager-next">
                <a data-toggle="tab" href="#{{ next_post_id }}">
                  <span class="pager-page-title">{{ next_post_title }}</span> →
                </a>
              </li>
            {% endif %}
          </ul>
        </nav>

        <h3>{{ p.title}}</h3>
        <p class="page-description">{{ p.description}}</p>
        <a class="btn btn-primary" href="{{ site.baseurl }}{{ p.url}}">Más información</a>
      </div>
    </div>
  {% endif %}
{% endfor %}
</section>
</div>
      
</div>

</section>




<section id="propuesta">
    <h2 class="section-header">Propuesta</h2>

    <p>Los animales valoran sus vidas incluso si nadie más lo hace. Son capaces de ser felices y de sufrir, y en este momento la están pasando muy mal.</p>

    <h3>¿Es dejar la carne la solución?</h3>

    <p>Dejar la carne es una decisión muy importante, aunque se debe tener en cuenta que en la industria de los huevos y la leche hay tanto o más sufrimiento, y una vez que el animal deja de ser económicamente eficiente en su producción, se lo mata.</p>

    <h3>¿Y si mejoramos las condiciones en las cuales los animales son utilizados?</h3>

    <p>La mayoría de las prácticas más cureles ocurren también en granjas no industriales. Debido a que los naimales son vistos como propiedad, se permite que las personas los usen para cualquier propósito que quieran y que les provoquen un terrible sufrimiento en el proceso.</p>

    <h3>¿Y cuál es la solución?</h3>

    <p>En la medida en que no cambiemos nuestra mirada hacia los animales, jamás habrá un cambio significativo para ellos. Es por esto que debemos abolir todo uso animal.</p>

    <p class="lead">Esto en la práctica significa ser vegamos.</p>

    <div class="featurette" id="about">
      <h2 class="featurette-heading">El veganismo es una posición ética <span class="text-muted"> que busca exluir en la medida de lo posible y practicable, todas las formas de explotación y crueldad hacia los animales.</span></h2>

      <p class="lead">Los veganos no comemos carne, lácteos ni huevos; no usamos lana, cuero ni otras pieles; no asistimos a espectáculos con animales y rechazamos la experimentación animal.</p>  
      <p class="lead">Ser vegano es reconocer el valor moral de los animales y aplicar en nuestras vidas la idea de que la explotación animal es inaceptable.</p>
      <p class="lead">Podemos vivir vidas felices y saludables sin usar a los animales, y eso es lo más importante que cada uno de nosotros puede hacer ahora mismo por ellos.</p>
    </div>

    <div class="row">

      <div class="col-lg-6 text-center">
        <div class="thumbnail">
          <img src="" alt="">
          <div class="caption">
            <h3>Documental Terrícolas</h3>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
            <p><a href="https://youtube.googleapis.com/v/PRrH6Ml5IDU" class="btn btn-default">Ver</a></p>
          </div>
        </div>
      </div>

      <div class="col-lg-6 text-center">
        <div class="thumbnail">
          <img src="" alt="">
          <div class="caption">
            <h3>El mejor discurso que jamás escucharás !!!</h3>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
            <p><a href="https://youtube.googleapis.com/v/PRrH6Ml5IDU" class="btn btn-default">Ver</a></p>
          </div>
        </div>
      </div>
    </div>
</section>

<section id="involucrate">
  <h2 class="section-header">Involucrate</h2>

  <h3>Si ya sos vegano o estás en transición y querés hacer algo más por los animales, lo siguiente más importante que podés hacer es educar a otros.</h3>
  
  <p class="lead">Si no sabés cómo empezar, estás invitado a participar con nosotros.</p>

  <h3>Activismos en 7 y 50</h3>
  <h4>Sumate!</h4>
  
  <p>Todos los viernes a la tarde nos podés encontrar en la esquina de 7 y 50 (La Plata) difundiendo los derechos animales y el veganismo. ¡Si querés informarte o participar acércate a conocernos!</p>

  <h3>Talleres de cocina</h3>
  <h4>Sumate!</h4>
  
  <p>Además realizamos talleres de cocina todos los meses para mostrarle a las personas que una forma de vida vegana puede ser saludable, nutricionalmente adecuada, deliciosa y al alcance de todos!</p>

  <h3>Eventos y charlas</h3>
  <h4>Sumate!</h4>
  
  <p>Además realizamos otras actividades de difusión, como degustaciones en plazas y charlas en eventos en La Plata y en otras ciudades, y proyecciones.</p>

</section>


</div>



<section id="contacto">
  <div class="container">
    <h2 class="section-header">Contacto</h2>

    <div class="row">
      <div class="col-lg-12 text-center">
        <h3>Pueden contactarse a través de nuestro facebook o enviando un correo electrónico a nuestro email.</h3>
      </div>

      <div class="col-lg-6 text-center">
        <span class="fa-stack fa-3x">
          <i class="fa fa-circle fa-stack-2x greencolor"></i>
          <i class="fa fa-facebook fa-stack-1x fa-inverse"></i>
        </span>
        <h4 class="service-heading">fb.com/activismo.coala</h4>
      </div>

      <div class="col-lg-6 text-center">
        <span class="fa-stack fa-3x">
          <i class="fa fa-circle fa-stack-2x greencolor"></i>
          <i class="fa fa-google fa-stack-1x fa-inverse"></i>
        </span>
        <h4 class="service-heading">activismo.coala@gmail.com</h4>
      </div>
    </div>
  </div>
</section>