---
layout: home
title: Coala - Activismo Vegano
permalink: /
---

<section id="cover">
  <div class="fill"></div>
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
  <div class="bg-content problematica-principal">         
    <p class="lead">Los animales son usados por los seres humanos para producción de vestimenta y alimentos, testeo de productos médicos y cosméticos, transporte de personas y de cargas pesadas, exposición en zoológicos y acuarios, con fines de entretenimiento en circos, corridas de toros, peleas de perros y doma, deportes como la pesca y las carreras y con fines bélicos, entre otros.</p>
         
    <p>Todos estos usos resultan en sufrimiento y muerte a los animales, y son totalmente innecesarios.</p> 
  </div>
</section>





<section id="realidad">

<h2 class="section-header">Explotación animal</h2>

<div class="row">

<div class="col-lg-3 col-sm-12">
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

<div class="col-lg-9 col-sm-12">
<section id="myTabContent" class="tab-content">
{% for p in site.pages %}
  {% if p.kind == 'explotacion' %}
    <div class="tab-pane fade {% if p.number == 2 %}active in{% endif %}" id="{{ p.url | remove:'/'}}">
      <div class="content bg-content">
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

</div>



<section id="propuesta">
  <div class="container">
    <h2 class="section-header">Propuesta</h2>

    <div class="row">
      <div class="col-lg-12 text-center">

        <div class="col-lg-12">
          <div class="featurette" id="about">
            <img class="featurette-image img-circle img-responsive pull-right" src="assets/queesveganismo.png">
            <h2 class="featurette-heading">El veganismo es una posición ética <span class="text-muted"> que busca exluir en la medida de lo posible y practicable, todas las formas de explotación y crueldad hacia los animales.</span></h2>

            <p class="lead">Los veganos no comemos carne, lácteos ni huevos; no usamos lana, cuero ni otras pieles; no asistimos a espectáculos con animales y rechazamos la experimentación animal.</p>  
            <p class="lead">Ser vegano es reconocer el valor moral de los animales y aplicar en nuestras vidas la idea de que la explotación animal es inaceptable.</p>
            <p class="lead">Podemos vivir vidas felices y saludables sin usar a los animales, y eso es lo más importante que cada uno de nosotros puede hacer ahora mismo por ellos.</p>
          </div>
        </div>

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
    </div>
  </div>
</section>




<section id="quienes-somos2">
  <div class="container">
    <h2 class="section-header">¿Quiénes somos?</h2>

    <div class="row">
      <div class="col-lg-12 text-center">
        <h4 class="">Somos un <span class="greencolor">grupo de activistas</span> formado en la ciudad de La Plata dedicado a la <span class="greencolor">difusión del veganismo</span>. Coala nació en agosto de 2013 y, a partir de entonces, <span class="greencolor">lucha sin descanso</span> por la liberación animal.</h4>
      </div>
        
      <div class="col-lg-12 text-center">
        <img id="logoimg" src="assets/cow.jpg" alt="Smiley face" height="190" width="255">
      </div>

      <div class="col-lg-12 text-center">
        <h2 class="section-heading">Nuestros ejes de trabajo son:</h2>
      </div>
    </div>
    
    <div class="row text-center">
      <div class="col-md-4">
        <span class="fa-stack fa-4x">
          <i class="fa fa-circle fa-stack-2x greencolor"></i>
          <i class="fa fa-info fa-stack-1x fa-inverse"></i>
        </span>
        
        <h4 class="service-heading">Difusión de la problemática del uso animal</h4>
        <p class="text-muted text-morebig">De forma comprometida y no violenta informamos a las personas sobre la grave situación que están viviendo los animales a causa del uso que les dan los seres humanos, alentando al cambio personal y a la abolición del uso animal en el ámbito individual.</p>
      </div>
      
      <div class="col-md-4">
        <span class="fa-stack fa-4x">
          <i class="fa fa-circle fa-stack-2x greencolor"></i>
          <i class="fa fa-comments fa-stack-1x fa-inverse"></i>
        </span>

        <h4 class="service-heading">Asistencia a las personas para impulsarlas a hacer la transición al veganismo.</h4>
        <p class="text-muted text-morebig">Con la amabilidad y continuidad que nos caracteriza, motivamos a las personas con preocupación por los animales a realizar la transición a una forma de vida vegana. Si queremos eliminar la explotación animal, un movimiento vegano es un requisito necesario, y ese movimiento empieza con la decisión de cada individuo.</p>
      </div>

      <div class="col-md-4">
        <span class="fa-stack fa-4x">
          <i class="fa fa-circle fa-stack-2x greencolor"></i>
          <i class="fa fa-users fa-stack-1x fa-inverse"></i>
        </span>
        <h4 class="service-heading">Alentar a las personas veganas o en transición a realizar activismo.</h4>
        <p class="text-muted text-morebig">Creemos que lo siguiente más importante que podemos hacer por los animales es ayudar a difundir los derechos animales y el veganismo. Los animales tienen voz, pero han sido silenciados, y necesitan que nosotros seamos su voz).</p>
      </div>
    </div>
  </div>
</section>




<section id="involucrate">
  <div class="container">
    <h2 class="section-header">Involucrate</h2>

    <div class="row">
      <div class="col-lg-12 text-center">
        <h3>Si ya sos vegano o estás en transición y querés hacer algo más por los animales, lo siguiente más importante que podés hacer es educar a otros.</h3>
        <p class="lead">Si no sabés cómo empezar, estás invitado a participar con nosotros.</p>
      </div>

      <div class="col-md-7">
        <a href="#">
          <img class="img-responsive" src="assets/difusion.jpg" alt="">
        </a>
      </div>

      <div class="col-md-5">
        <h3>Activismos en 7 y 50</h3>
        <h4>Sumate!</h4>
        <p>Todos los viernes a la tarde nos podés encontrar en la esquina de 7 y 50 (La Plata) difundiendo los derechos animales y el veganismo. ¡Si querés informarte o participar acércate a conocernos!</p>
      </div>

      <div class="col-md-7">
        <a href="#">
          <img class="img-responsive" src="assets/pizza.jpg" alt="">
        </a>
      </div>

      <div class="col-md-5">
        <h3>Talleres de cocina</h3>
        <h4>Sumate!</h4>
        <p>Además realizamos talleres de cocina todos los meses para mostrarle a las personas que una forma de vida vegana puede ser saludable, nutricionalmente adecuada, deliciosa y al alcance de todos!</p>
      </div>

      <div class="col-md-7">
        <a href="#">
          <img class="img-responsive" src="assets/charlas.jpg" alt="">
        </a>
      </div>

      <div class="col-md-5">
        <h3>Eventos y charlas</h3>
        <h4>Sumate!</h4>
        <p>Además realizamos otras actividades de difusión, como degustaciones en plazas y charlas en eventos en La Plata y en otras ciudades, y proyecciones.</p>
      </div>
    </div>
  </div>
</section>




<section id="contacto">
  <div class="container">
    <h2 class="section-header">Contacto</h2>

    <div class="row">
      <div class="col-lg-12 text-center">
        <h3>Pueden contactarse a través de nuestro facebook o enviando un correo electrónico a nuestro email.</h3>
      </div>

      <div class="col-lg-6 text-center">
        <span class="fa-stack fa-5x">
          <i class="fa fa-circle fa-stack-2x greencolor"></i>
          <i class="fa fa-facebook fa-stack-1x fa-inverse"></i>
        </span>
        <h4 class="service-heading">fb.com/activismo.coala</h4>
      </div>

      <div class="col-lg-6 text-center">
        <span class="fa-stack fa-5x">
          <i class="fa fa-circle fa-stack-2x greencolor"></i>
          <i class="fa fa-google fa-stack-1x fa-inverse"></i>
        </span>
        <h4 class="service-heading">activismo.coala@gmail.com</h4>
      </div>
    </div>
  </div>
</section>