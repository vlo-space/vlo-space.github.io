---
layout: base
title: "Strona główna"
---

<article>
    <section>
        <strong>W roku szkolnym 2025/26 wracamy do akcji!</strong> <a href="{% link _posts/2025-09-16-vlo-space-wraca-do-akcji.md %}">Przeczytaj naszego bloga</a>

        <h1>Witaj na naszej stronie!</h1>

        <p>
            Jesteśmy grupą pasjonatów szeroko pojętej technologii, biorących udział w konkursie CanSat organizowanym przez Europejską Agencję Kosmiczną. 
        </p>
        
        <p>
            Budujemy latającą sondę z systemem radiowej nawigacji bez użycia GPS. Będzie ona wielkości puszki po napoju. W trakcie finału konkursu nasze urządzenie zostanie wyrzucone z rakiety na wysokości 2,5 km.
        </p>
        
        <p>
            Budowa takiej jednostki jest bardziej skomplikowana niż mogłoby się wydawać - mnóstwo różnych elementów, od mechaniki, przez elektronikę, po oprogramowanie, musi być dobrze wykonanych aby misja się udała. Na szczęście, nasza drużyna posiada szeroką gamę zainteresowań i talentów, które ułatwiają pokonanie tego wyzwania.
        </p>
        
        <p>
            Chcesz wiedzieć więcej?
            
            <div class="link-buttons-container">
                <a href="{% link o-nas.md %}">O nas</a>
                <a href="{% link nasz-projekt.md %}">Nasz projekt</a>
            </div>
        </p>
    </section>
</article>

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
        <a href="/assets/media/post/vlo-space-wraca-do-akcji/druzyna.jpg"><img src="/assets/media/post/vlo-space-wraca-do-akcji/druzyna.jpg" alt="Drużyna VLO Space 2025/26 stojąca przed rollupem zespołu."></a>
    </section>
</aside>
