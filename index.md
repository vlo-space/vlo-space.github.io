---
layout: base
title: "Strona główna"
---

<main>
    <section>
        <h1>Witaj na naszej stronie!</h1>

        <p>
            Jesteśmy grupą pasjonatów szeroko pojętej technologii, biorących udział w konkursie CanSat. 
        </p>
        
        <p>
            Budujemy urządzenie służące wykrywaniu i badaniu fal sejsmicznych. Będzie ono wielkości puszki po napoju. W trakcie finału konkursu nasza puszka zostanie wyrzucona z rakiety na wysokości 2,5 km.
        </p>
        
        <p>
            Budowa takiej jednostki jest bardziej skomplikowana niż mogłoby się wydawać - wszystkie elementy muszą być dokładnie przemyślane i starannie wykonane. 
        </p>
        
        <p>
            Chcesz wiedzieć więcej?
            
            <div class="link-buttons-container">
                <a href="{% link o-nas.md %}">O nas</a>
                <a href="{% link nasz-projekt.md %}">Nasz projekt</a>
            </div>
        </p>
    </section>
</main>

<aside>
    {% if site.posts.size > 0 %}
    <section>
        <h2>Sprawdź naszego bloga:</h2>
        <ul>
        {% for post in site.posts limit:10 %}
            <li><a href="{{ post.url }}">{{ post.title }}</a></li>
        {% endfor %}
        </ul>
    </section>
    {% endif %}
    
    <section class="image-container">
        <a href="https://picsum.photos/seed/1/600/400"><img src="https://picsum.photos/seed/1/600/400"></a>
    </section>
</aside>
