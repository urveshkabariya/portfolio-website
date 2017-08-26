---
layout: page
title : Portfolio
header : Project Archive
group: navigation
---
<div id="portfolio">

  {% include JB/setup %}

  <div class="row">
  {% for portfolio in site.data.portfolios %}
      <div class="col-md-4 col-sm-6 portfolio-item">
          <a href="#portfolioModal{{ portfolio.id }}" class="portfolio-link" data-toggle="modal">
              <div class="portfolio-hover">
                  <div class="portfolio-hover-content">
                      <i class="fa fa-puzzle-piece fa-3x"></i>
                  </div>
              </div>
              {% if portfolio.thumbnail %}
                <img src="{{ ASSET_PATH }}/img/portfolio/{{ portfolio.thumbnail }}" class="img-responsive" alt="">
              {% endif %}
              <div class="portfolio-caption">
                  <h4>{{ portfolio.title }}</h4>
                  <p class="text-muted">{{ portfolio.subtitle }}</p>
              </div>
          </a>
      </div>
  {% endfor %}
  </div>

</div>
