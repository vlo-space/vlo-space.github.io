---
layout: base
title: "Strona główna"
---

<main>
    <section>
        <h2>Najnowsze posty na naszym blogu:</h2>
        <div class="card-container">
            {% for post in site.posts limit:10 %}
                <a href="{{ post.url }}">
                    <div class="card">
                        <h2>{{ post.title }}</h2>
                        <p>{{ post.date | date: "%-d.%m.%Y" }} - {{post.excerpt}}</p>
                    </div>
                </a>
            {% endfor %}
        </div>
    </section>
</main>

