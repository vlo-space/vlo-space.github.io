---
layout: base
title: "Blog"
---

<main>
    <section>
        <h2>Najnowsze posty na naszym blogu:</h2>
        <div class="card-container">
            {% for post in site.posts limit:10 %}
                <a href="{{ post.url }}">
                    <div class="card card-post">
                        <div class="post-info">
                            <h2>{{ post.title }}</h2>
                            <span class="meta">{{ post.date | date: "%-d.%m.%Y" }}</span>
                            {{post.excerpt}}
                        </div>

                        {% for media in post.media %}
                            {% capture media_url %}/assets/media/post/{{ post.slug }}/{% endcapture %}
                            {% if media.url %}
                                {% capture media_url %}{{ media_url }}{{ media.url }}{% endcapture %}
                            {% else %}
                                {% capture media_url %}{{ media_url }}{{ media }}{% endcapture %}
                            {% endif %}

                            <img src="{{ media_url }}" {% if media.title %}title="{{ media.title }}"{% endif %} {% if media.alt %}alt="{{ media.alt }}"{% endif %} >

                            {% break %}
                        {% endfor %}
                    </div>
                </a>
            {% endfor %}
        </div>
    </section>
</main>

