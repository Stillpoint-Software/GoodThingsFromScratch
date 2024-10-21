---
layout: default
---

{% include hero.html %}
{% include home-content.html %}
{% include review-content.html %}
<div class="container">
    <div class="row">
        <div class="col col-12 col-d-10 col-m-12 push-m-0 push-d-1">
            <div class="contaniner__inner">
                <h1>Recent Stories</h1>
                <div class="row grid">
                    {% if site.posts.size > 0 %}
                    {% for post in site.posts limit: 3 %}
                    {% include article-content.html %}
                    {% endfor %}
                    {% endif %}
                </div>
            </div>
        </div>
    </div>
</div>

<div class="container">
    <div class="row">
        <div class="col col-12 col-d-10 col-m-12 push-m-0 push-d-1">
            <div class="contaniner__inner">
                <p><a class="button" href="{{site.baseurl}}/about">More Stories</a></p>
            </div>
        </div>
    </div>
</div>
