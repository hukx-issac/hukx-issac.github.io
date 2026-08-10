---
layout: archive
title: "Team"
permalink: /team/
redirect_from:
  - /talks/
author_profile: true
teachers:
  - name: "Kaixi Hu (胡开喜)"
    role: "Lecturer"
    photo: "/images/Kaixi.png"
    url: "/"
current_students: []
collaborators: []
alumni: []
---

<div class="team-page">
  <p class="team-page__intro">Meet our faculty, current students, collaborators, and alumni.</p>

  <section class="team-section" aria-labelledby="team-faculty">
    <h2 id="team-faculty">Faculty</h2>
    <div class="team-member-grid">
      {% for member in page.teachers %}
        <article class="team-member-card">
          {% if member.url and member.url != empty %}<a class="team-member-card__link" href="{{ member.url | relative_url }}">{% endif %}
            <img class="team-member-card__photo" src="{{ member.photo | relative_url }}" alt="Photo of {{ member.name }}" loading="lazy">
            <div class="team-member-card__details">
              <h3>{{ member.name }}</h3>
              {% if member.role and member.role != empty %}<p>{{ member.role }}</p>{% endif %}
            </div>
          {% if member.url and member.url != empty %}</a>{% endif %}
        </article>
      {% endfor %}
    </div>
  </section>

  <section class="team-section" aria-labelledby="team-students">
    <h2 id="team-students">Current Students</h2>
    {% if page.current_students and page.current_students != empty %}
      <div class="team-member-grid">
        {% for member in page.current_students %}
          <article class="team-member-card">
            {% if member.url and member.url != empty %}<a class="team-member-card__link" href="{{ member.url }}">{% endif %}
              <img class="team-member-card__photo" src="{{ member.photo | relative_url }}" alt="Photo of {{ member.name }}" loading="lazy">
              <div class="team-member-card__details">
                <h3>{{ member.name }}</h3>
              </div>
            {% if member.url and member.url != empty %}</a>{% endif %}
          </article>
        {% endfor %}
      </div>
    {% else %}
      <p class="team-section__empty">To be updated.</p>
    {% endif %}
  </section>

  <section class="team-section" aria-labelledby="team-collaborators">
    <h2 id="team-collaborators">Collaborators</h2>
    {% if page.collaborators and page.collaborators != empty %}
      <div class="team-member-grid">
        {% for member in page.collaborators %}
          <article class="team-member-card">
            {% if member.url and member.url != empty %}<a class="team-member-card__link" href="{{ member.url }}">{% endif %}
              <img class="team-member-card__photo" src="{{ member.photo | relative_url }}" alt="Photo of {{ member.name }}" loading="lazy">
              <div class="team-member-card__details">
                <h3>{{ member.name }}</h3>
                {% if member.affiliation and member.affiliation != empty %}<p>{{ member.affiliation }}</p>{% endif %}
              </div>
            {% if member.url and member.url != empty %}</a>{% endif %}
          </article>
        {% endfor %}
      </div>
    {% else %}
      <p class="team-section__empty">To be updated.</p>
    {% endif %}
  </section>

  <section class="team-section" aria-labelledby="team-alumni">
    <h2 id="team-alumni">Alumni</h2>
    {% if page.alumni and page.alumni != empty %}
      <div class="team-alumni-list">
        {% for member in page.alumni %}
          <article class="team-alumni-card">
            <h3>{{ member.name }}</h3>
            {% if member.destination and member.destination != empty %}<p>{{ member.destination }}</p>{% endif %}
          </article>
        {% endfor %}
      </div>
    {% else %}
      <p class="team-section__empty">To be updated.</p>
    {% endif %}
  </section>
</div>
