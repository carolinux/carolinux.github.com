---
layout: index
title: Karolina Alexiou
tagline: My personal website, where I showcase all my main projects.
---
{% include JB/setup %}

<div class="wrapper">
  <div id="contact" >
    <div class="container">
      <div class="row col-sm-8 col-sm-offset-2 speak">

       <p> Under construction! </p>

        <div class='social-media'>
          <a href="https://github.com/carolinux" rel="me"><i class="fa fa-github"></i></a>
          <a href="https://twitter.com/#!/_sandtweets" rel="me"><i class="fa fa-twitter"></i></a>
          <a href="https://medium.com/@_sandtweets"><i class="fa fa-medium"></i></a>
          <a href="https://instagram.com/idledaze/"><i class="fa fa-instagram"></i></a>
        </div>

        <p><a href="mailto:carolinegr@gmail.com">carolinegr@gmail.com</a></p>

      </div>
    </div>
  </div>
  <div class="container">
    <div class="row col-md-12 projects">
      {% assign projects = site.projects | sort: 'ranking' %}
      {% for project in projects %}
        {% assign loopindex = forloop.index | modulo: 3 %}
          <div class="col-xs-10 col-xs-offset-1 col-sm-4 col-sm-offset-0 col-md-3">
            <div class="hovereffect">
                <img class="img-responsive" src="assets/img/project/{{ project.picture-small }}" alt="">
                    <div class="overlay">
                       <h2>{{project-title}}</h2>
                      <p>{{ project.stub}}<br />
                        <a href="{{project.url}}">info</a>
                      {{ project.role }} <span class="status">{{ project.status }}</span></p>

                    </div>
            </div>
        </div>

      {% endfor %}
    </div>
  </div>
</div>
<!---
<div class="container">
  <div class="row press">
    <h1 class="section-header">Press</h1>
    {% for press in site.data.press %}
      {% if press.hide != true %}
        <div class="col-xs-6 col-sm-3 col-md-2">
          <div class="img-container">
            <a href="{{ press.url }}" title="{{ press.title }}">
              <img src="assets/img/press/{{ press.image }}" class="card-image">
            </a>
          </div>
        </div>
      {% endif %}
    {% endfor %}
  </div>-->
</div>

{% include footer.html %}
