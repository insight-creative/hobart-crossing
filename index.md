---
layout: default
---
<div class="header-image">
<img src="{{ site.baseurl }}/img/hobart-elevation-1.jpg">
</div>

<div class="container">
  <div class="row">
    <div class="col-md-10 center-block">
      <div class="card header-card">
        <h1>Welcome Home to Hobart Crossing!</h1>

        <h2>Luxury leased residences</h2>

        <p class="text-center">There’s an exciting new place to call home in the greater Green Bay area.</p>

        <div class="row">
          <div class="col-md-6">
            <h3>Common Area Amenities include:</h3>
            <ul>
              <li>A large outdoor pool area with grills and lounging space</li>
              <li>Fitness center outfitted with professional equipment</li>
              <li>Spacious clubroom</li>
              <li>Elevator</li>
              <li>Underground Parking</li>
            </ul>
          </div>
          <div class="col-md-6">
            <h3>Apartment Features include:</h3>
            <ul>
              <li>Granite countertops</li>
              <li>In-unit washer/dryer</li>
              <li>Upgraded appliances</li>
            </ul>
          </div>
        </div>

        <p>Take a few minutes to browse our site and see all the advantages of life at Hobart Crossing! Then <a href="{{ site.baseurl }}/contact">contact us</a> with your questions.</p>

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
          <img src="{{ site.baseurl }}/img/community-header.jpg">
        </div>
        <h1>Community</h1>
        <p>Hobart Crossing is located in <em><a href="http://buildinhobart.com">Centennial Centre at Hobart</a></em>, a planned community bringing a luxury presence to the gorgeous countryside just minutes west of Green Bay.</p>
        <div class="card-button-group">
          <a class="card-button" href="{{ site.baseurl }}/community">Learn more &raquo;</a>
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
          <h2><a class="post-title" href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>
          {{ post.excerpt }}</p><!-- weird Jekyll glitch, closing p tag required -->
          <div class="card-button-group">
            <a class="card-button" href="{{ site.baseurl }}{{ post.url }}">Continue reading &raquo;</a>
            <a class="card-button" href="{{ site.baseurl }}/news">See all news &raquo;</a>
          </div>
          {% endfor %}
        </div>
      </div>
    </div>
    <div class="col-md-6">
      <div class="card">
        <h1>Contact Us</h1>
        <div class="card-button-group">
          <div class="card-button"><span class="glyphicon glyphicon-earphone"></span>&nbsp;&nbsp;(920) 461-1900</div>
          <a class="card-button" href="mailto:info@hobartcrossing.com"><span class="glyphicon glyphicon-envelope"></span>&nbsp;&nbsp;leasing@HobartCrossing.com</a>
        </div>
      </div>
    </div>
  </div>
</div>
