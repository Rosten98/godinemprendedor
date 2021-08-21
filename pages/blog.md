---
layout: blog
title: Blog
# header_image: 
---
<section id="portfolio" class="bg-light-gray">
    <div class="container">
        <div class="row">
            <div class="col-lg-12 text-center">
                <h2 class="section-heading">Blog</h2>
            </div>
        </div>
        <div class="row">
        {% for post in site.posts %}
            <div class="col-md-4 col-sm-6 portfolio-item">
                <a href="{{post.url}}" class="portfolio-link">
                    <div class="portfolio-hover">
                        <div class="portfolio-hover-content">
                            <i class="fa fa-plus fa-3x"></i>
                        </div>
                    </div>
                    <img src="/assets/uploads/{{ post.thumbnail }}" class="img-responsive img-centered" alt="">
                </a>
                <div class="portfolio-caption">
                    <h4>{{ post.title }}</h4>
                    <p class="text-muted">{{ post.excerpt }}</p>
                </div>
            </div>
        {% endfor %}
        </div>
    </div>
</section>
