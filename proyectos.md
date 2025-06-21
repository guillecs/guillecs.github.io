---
title: Mis acomplishments
subtitle: Discover my acomplishments as quality engineer
layout: page # Usa el layout de página estándar del tema Forty
permalink: /acomplishments/ # Asegura que la URL sea /proyectos/
---

<div id="main">
    <section id="one" class="tiles">
        {% for acomplishment in site.acomplishments %}
            <article>
                <span class="image">
                    <img src="{{ site.baseurl }}/{{ acomplishment.image }}" alt="{{ acomplishment.alt }}" />
                </span>
                <header class="major">
                    <h3><a href="{{ acomplishment.url | relative_url }}" class="link">{{ acomplishment.title }}</a></h3>
                    <p>{{ project.subtitle }}</p>
                </header>
                <a href="{{ acomplishment.url | relative_url }}" class="link primary"></a>
            </article>
        {% endfor %}
    </section>
</div>