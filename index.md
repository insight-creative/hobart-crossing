---
layout: default
---
<div class="header-image">
<img src="{{ site.baseurl }}/img/hobart-elevation-1.jpg">
</div>

<!--
<div class="container">
  <div class="row">
    <div class="col-md-8 center-block">
      <div class="card">
        <h1>Landing Page</h1>
        <ul>
          <li>Header image</li>
          <li>Link to apartments page</li>
          <li>Link to community page</li>
          <li>Most recent news posts</li>
          <li>Call to action to contact with link to contact page</li>
      </div>
    </div>
  </div>
</div>-->

<div class="container">
  <div class="row">
    <div class="col-md-12">
      <div class="card">
        <h1>Hobart Crossing—Luxury Leased Residences</h1>

        <p>Enjoy life at Hobart Crossing in Centennial Centre! Hobart Crossing features upscale amenities and a refined urban feel.</p>
      </div>
    </div>
  </div>
  
  <div class="row">
    <div class="col-md-6">
      <div class="card">
        <h1>Apartments</h1>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus mattis justo eget magna vehicula molestie. Sed porta feugiat lacus ut ultrices.</p>
        <div class="card-button-group">
          <a class="card-button" href="{{ post.url }}">Learn more &raquo;</a>
        </div>
      </div>
    </div>
    
    <div class="col-md-6">
      <div class="card">
        <h1>Community</h1>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus mattis justo eget magna vehicula molestie. Sed porta feugiat lacus ut ultrices.</p>
        <div class="card-button-group">
          <a class="card-button" href="{{ post.url }}">Learn more &raquo;</a>
        </div>
      </div>
    </div>
  </div>
  
  <div class="row">
    <div class="col-md-6">
      <div class="card">
        <h1>Latest News</h1>
        {% for post in site.posts | limit: 1 %}
        <div class="post">
          <h2><a class="post-title" href="{{ post.url }}">{{ post.title }}</a></h2>
          {{ post.content | truncatewords: 15 }}</p><!-- weird Jekyll glitch, closing p tag required -->
          <div class="card-button-group">
            <a class="card-button" href="{{ post.url }}">Continue reading &raquo;</a>
            <a class="card-button" href="{{ site.baseurl }}/news">See all news &raquo;</a>
          </div>
          {% endfor %}
        </div>
      </div>
    </div>
    <div class="col-md-6">
      <div class="card">
        <h1>Contact Us</h1>
        <p>Pre-leasing begins April 2015 for occupancy August 2015.</p>

        <p><em>Don’t delay—units will fill fast!</em></p>

        <div class="card-button-group">
          <div class="card-button"><span class="glyphicon glyphicon-earphone"></span>&nbsp;&nbsp;(920) 461-1900</div>
          <a class="card-button" href="mailto:info@hobartcrossing.com"><span class="glyphicon glyphicon-envelope"></span>&nbsp;&nbsp;info@HobartCrossing.com</a>
        </div>
      </div>
    </div>
  </div>
</div>

