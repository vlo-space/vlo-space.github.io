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
                        <h2>{{ post.title }}</h2>
                        <span class="meta">{{ post.date | date: "%-d.%m.%Y" }}</span>
                        {{post.excerpt}}
                    </div>
                </a>
            {% endfor %}
        </div>
    </section>
</main>

