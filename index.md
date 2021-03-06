---
layout: default
---
<div class="header-image">
<img src="{{ site.baseurl }}/img/hobart-elevation-1.jpg">
</div>

<div class="container">
  <div class="row">
    <div class="col-md-12 center-block">
      <div class="card header-card">
        <h1>Welcome Home to Hobart Crossing Luxury Leased Residences!</h1>

        <p class="text-center">There’s an exciting new place to call home in the greater Green Bay area.</p>

      </div>
    </div>
  </div>

  <div class="row">
    <div class="col-md-6">
      <div class="card">
        <div class="card-header">
          <img src="{{ site.baseurl }}/img/apartments-header.jpg">
        </div>
        <h1>Apartments</h1>
        <p>Experience life with luxury amenities, serene surroundings and more convenience than ever before. Each Hobart Crossing apartment home brings a refined, contemporary feel and is directly connected to the development’s amenities.</p>
        <div class="card-button-group">
          <a class="card-button" href="{{ site.baseurl }}/apartments">Learn more &raquo;</a>
        </div>
      </div>
    </div>
    <div class="col-md-6">
      <div class="card">
        <div class="card-header">
          <img src="{{ site.baseurl }}/img/amenities-header.jpg">
        </div>
        <h1>Amenities</h1>
        <p>Our commmunity amenities are second to none. Commercial grade fitness equipment, a stunning club room and an amazing pool/sundeck are yours to enjoy 7 days a week.</p>
        <p class="padding-card-hack"> </p>
        <div class="card-button-group">
          <a class="card-button" href="{{ site.baseurl }}/amenities">Learn more &raquo;</a>
        </div>
      </div>
    </div>
  </div>

  <div class="row">
    <div class="col-md-6">
      <div class="card">
        <div class="card-header">
          <img src="{{ site.baseurl }}/img/community-header.jpg">
        </div>
        <h1>Community</h1>
        <p>Hobart Crossing is located in <em><a href="http://buildinhobart.com">Centennial Centre at Hobart</a></em>, a planned community bringing a luxury presence to the gorgeous countryside just minutes west of Green Bay.</p>
        <div class="card-button-group">
          <a class="card-button" href="{{ site.baseurl }}/community">Learn more &raquo; </a>
        </div>
      </div>
    </div>

    <div class="col-md-6">
      <div class="card">
        <h1>Latest News</h1>
        {% for post in site.posts limit: 1 %}
        <div class="post">
          <h2><a class="post-title" href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>
          {{ post.excerpt }}<!-- weird Jekyll glitch, closing p tag required -->
          <p class="padding-card-hack2"> </p>
          <div class="card-button-group">
            <a class="card-button" href="{{ site.baseurl }}{{ post.url }}">Continue reading &raquo;</a>
          </div>
          {% endfor %}
        </div>
      </div>
    </div>
  </div>

  <div class="row">
    <div class="col-md-6 col-md-offset-3">
      <div class="card">
        <h1>Contact Us</h1>
        <div class="card-button-group">
          <div class="card-button"><span class="glyphicon glyphicon-earphone"></span>&nbsp;&nbsp;(920) 461-1900</div>
        </div>
      </div>
    </div>
  </div>
</div>
