---
layout: pagina
---

<section id="publicaciones">
  <div class="container">
    <div class="row text-center">
      <h1 class="titulo">Archivo</h1>
    </div>

    {% for post in site.posts %}
      <div class="row publicacion">
        <div class="col-xs-4 col-md-offset-2 col-md-2 data" align="right">
          <h5>{{ post.date | date_to_string }}</h5>
          <a href="{{ post.url }}">{{ post.category }}</a>
        </div>
      <div class="col-xs-8 col-md-6 text" align="left">
        <a href="{{ post.url }}"><h3>{{ post.title }}</h3></a>
        <p>{{ post.excerpt }}</p>
        <a href="{{ post.url }}">Ver más</a>
      </div>
    </div>
    {% endfor %}

  </div>
</section>
