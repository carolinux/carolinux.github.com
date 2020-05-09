---
layout: index
title: Karolina Alexiou - Zurich Data Engineer, DevOps, Technical Interviewing
---
{% include JB/setup %}

<div class="wrapper">
  <div id="contact" >
    <div class="container">
      <div class="row col-sm-8 col-sm-offset-2 speak">

       <p> Hi! </p>

 <p>I am Karolina Alexiou and I am a software engineer based in Zurich, Switzerland. I support businesses to deploy their infrastructure into the cloud and also undertake data engineering projects to integrate, combine and visualize data sources.</p> <p>I can also support your company design and carry out an effective hiring process for software engineers.</p>
<p> Check out my <a href="services.html">services page</a> or get in touch below to learn more. </p>
        <div class='social-media'>
          <a href="https://github.com/carolinux" rel="me"><i class="fa fa-github"></i></a>
          <a href="https://www.linkedin.com/in/ariadni-karolina-alexiou-9a365734/" rel="me"><img src="assets/li.png" width="40" height="40"/></a>
        </div>
<p><a href="mailto://hello@lucidcode.ch">hello@lucidcode.ch</a></p>

      </div>
    </div>
  </div>

<div class="container">
    <div class="row col-md-12 projects">

          <div class="col-xs-10 col-xs-offset-2 col-sm-4 col-sm-offset-2 col-md-3">
           <h4>Write to me</h4>
          <div class='img-container'>
            <div>
                <img class="img-responsive" src="assets/img/project/tech-articles-before-small.png"  alt="" onmouseover="this.src='assets/img/project/tech-articles-after-small.png'"
    onmouseout="this.src='assets/img/project/tech-articles-before-small.png'">
            </div>
           
           
           </div>
        </div>

          <div class="col-xs-10 col-xs-offset-1 col-sm-4 col-sm-offset-1 col-md-3">
<h4>Your details:</h4>
<form
  action="https://formspree.io/xknqgnqg"
  method="POST"
>
<p>
  <label>
    Name:
    <input type="text" name="name">
  </label>
  <label>
    Email:
    <input type="text" name="_replyto">
  </label>
  <label>
    Message:
    <textarea name="message"></textarea>
  </label>

  <!-- your other form fields go here -->
  <button type="submit">Send</button>
</p>
</form>
</div>
</div>
</div>
<!---
  <div class="container">
    <div class="row col-md-12 projects">
      {% assign projects = site.projects | sort: 'ranking' %}
      {% for project in projects %}
        {% assign loopindex = forloop.index | modulo: 3 %}
          <div class="col-xs-10 col-xs-offset-1 col-sm-4 col-sm-offset-0 col-md-3">
          <div class='img-container'>
            <div>
                <a href="{{project.url}}">
                <img class="img-responsive" src="assets/img/project/{{ project.picture-before-small }}" alt="" onmouseover="this.src='assets/img/project/{{ project.picture-after-small }}'"
    onmouseout="this.src='assets/img/project/{{ project.picture-before-small }}'"></a>
            </div>
           
               <a class="project-title" href="{{project.url}}">
              <h4>
                {{project.title}}
              </h4>
              <p>
              <span class="status">{{ project.status }}</span></p>
            </a>
           
           </div>
        </div>
        {% if forloop.index == 3 %}
          <div class="clearfix visible-sm-block"></div>
        {% elsif forloop.index == 4 %}
          <div class="clearfix visible-md-block visible-lg-block"></div>
        {% elsif forloop.index == 12 %}
          <div class="clearfix visible-md-block visible-lg-block"></div>
                {% elsif forloop.index == 20 %}
          <div class="clearfix visible-md-block visible-lg-block"></div>
                {% elsif forloop.index == 24 %}
          <div class="clearfix visible-md-block visible-lg-block"></div>
                {% elsif forloop.index == 28 %}
          <div class="clearfix visible-md-block visible-lg-block"></div>

                {% elsif forloop.index == 40 %}
          <div class="clearfix visible-md-block visible-lg-block"></div>
        {% endif %}

      {% endfor %}
    </div>
  </div>
</div>
-->
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
  </div>
</div>

-->
{% include footer.html %}
