---
layout: page
title: Story
image: /assets/stbarth-girl.jpg
permalink: /story/
pagination:
    enabled: true
date: 2024-10-30
navorder: 3
---

<div class="container">
    <div class="row">
        <div class="col col-12 col-d-10 col-m-12 push-m-0 push-d-1">
            <div class="contaniner__inner">
                <div class="row grid">
                    {% if site.posts.size > 0 %}
                    {% for post in paginator.posts %}
                    {% include article-content.html %}
                    {% endfor %}
                    {% endif %}
                </div>
            </div>
        </div>
    </div>
</div>
{% include pagination.html %}