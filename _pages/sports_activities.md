
---
title: "Sports & Activities"
permalink: /sports_activities/
layout: single
author_profile: true
---

<style>
.sports-page {
  --sports-bg: #101820;
  --sports-panel: #18242e;
  --sports-accent: #8bd450;
  --sports-text: #edf2f5;
  --sports-muted: #b5c0c8;
  color: var(--sports-text);
  margin-top: 1.5rem;
}
.sports-hero {
  background: linear-gradient(135deg, #182b34, #101820 70%);
  border: 1px solid #31424c;
  border-radius: 16px;
  padding: 2.2rem;
  margin-bottom: 2rem;
}
.sports-kicker {
  color: var(--sports-accent);
  text-transform: uppercase;
  letter-spacing: 3px;
  font-size: .8rem;
  font-weight: 700;
}
.sports-hero h2 {
  color: #fff;
  font-size: clamp(2rem, 5vw, 3.3rem);
  line-height: 1.1;
  margin: .7rem 0 1rem;
}
.sports-hero p, .sports-page p {
  color: var(--sports-muted);
  line-height: 1.8;
}
.sports-position {
  display: inline-block;
  background: #263b30;
  border: 1px solid #46664a;
  color: #d7ffb9;
  border-radius: 30px;
  padding: .45rem .85rem;
  margin-top: .4rem;
  font-size: .9rem;
}
.sports-section {
  margin: 2.8rem 0;
}
.sports-section h2 {
  color: var(--sports-text);
  border-bottom: 1px solid #34444e;
  padding-bottom: .7rem;
  margin-bottom: .7rem;
}
.sports-section h3 {
  color: #fff;
}
.sports-timeline {
  border-left: 2px solid #526c50;
  margin: 1.5rem 0 1rem .5rem;
  padding-left: 1.4rem;
}
.sports-event {
  position: relative;
  background: var(--sports-panel);
  border: 1px solid #2d3c46;
  border-radius: 10px;
  padding: 1rem 1.2rem;
  margin: 0 0 1rem;
}
.sports-event:before {
  content: "";
  position: absolute;
  left: -1.85rem;
  top: 1.35rem;
  width: 10px;
  height: 10px;
  background: var(--sports-accent);
  border-radius: 50%;
}
.sports-date {
  color: var(--sports-accent);
  font-size: .85rem;
  font-weight: 700;
  letter-spacing: .5px;
}
.sports-gallery {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 12px;
  margin-top: 1.3rem;
}
.sports-photo {
  margin: 0;
  background: var(--sports-panel);
  border: 1px solid #2d3c46;
  border-radius: 10px;
  overflow: hidden;
}
.sports-photo img {
  display: block;
  width: 100%;
  height: 220px;
  object-fit: cover;
  background: #202b33;
  transition: transform .25s ease;
}
.sports-photo:hover img {
  transform: scale(1.035);
}
.sports-photo figcaption {
  padding: .65rem .8rem;
  color: var(--sports-muted);
  font-size: .82rem;
}
.sports-note {
  background: var(--sports-panel);
  border-left: 3px solid var(--sports-accent);
  padding: 1rem 1.2rem;
  border-radius: 0 8px 8px 0;
}
@media (max-width: 700px) {
  .sports-hero { padding: 1.4rem; }
  .sports-gallery { grid-template-columns: repeat(2, minmax(0, 1fr)); gap: 8px; }
  .sports-photo img { height: 160px; }
}
@media (max-width: 420px) {
  .sports-gallery { grid-template-columns: 1fr 1fr; }
  .sports-photo img { height: 135px; }
}
</style>

<div class="sports-page">

  <section class="sports-hero">
    <div class="sports-kicker">Beyond the everyday</div>
    <h2>Sports &amp; Activities</h2>
    <p>
      Sports have been an important part of my life, from playing football
      on local fields to exploring cycling and other activities. This page
      brings together some of my sporting experiences, interests and memories.
    </p>
    <span class="sports-position">Football · Central Defender (CB)</span>
  </section>

  <section class="sports-section">
    <h2>Football</h2>
    <p>
      Football has been one of my strongest interests since childhood.
      Growing up, I spent a lot of time playing on a large local field.
      Over the years, I played with local clubs and represented my school
      in an inter-school tournament.
    </p>

    <h3>Playing Experience</h3>
    <div class="sports-timeline">

      <div class="sports-event">
        <div class="sports-date">2019</div>
        <h3>Kushtia First Division Football League</h3>
        <p>
          Represented Kushtia Football Club in the First Division Football
          League in Kushtia.
        </p>
      </div>

      <div class="sports-event">
        <div class="sports-date">2018–2020</div>
        <h3>Kushtia Jubo Sporting Club</h3>
        <p>
          Played for Kushtia Jubo Sporting Club during this period.
        </p>
      </div>

      <div class="sports-event">
        <div class="sports-date">2018</div>
        <h3>Inter-School Football Tournament</h3>
        <p>
          Represented Kamalapur Secondary School in the Inter-School
          Football Tournament in Kushtia Sadar Upazila while studying
          in Class Eight.
        </p>
      </div>

      <div class="sports-event">
        <div class="sports-date">Local Club Experience</div>
        <h3>United Football Club</h3>
        <p>
          Played for the local United Football Club for an extended period.
        </p>
      </div>

    </div>

    <div class="sports-note">
      <strong>Playing position:</strong> Central Defender
      (Centre-Back / CB). My role is focused on defensive positioning,
      reading the game and supporting the team's defensive line.
    </div>

    <h3 style="margin-top: 2rem;">Football Gallery</h3>
    <div class="sports-gallery">
      {% assign football_images = "football-1.jpeg,football-2.jpeg,football-3.jpeg,football-4.jpg,football-5.jpeg,football-6.jpeg,football-7.jpg,football-8.jpeg,football-9.jpeg,football-10.jpeg,football-11.jpeg,football-12.jpeg,football-13.jpeg" | split: "," %}
      {% for image in football_images %}
      <figure class="sports-photo">
        <img src="{{ site.baseurl }}/images/sports/{{ image }}" alt="Football photo {{ forloop.index }}" loading="lazy">
        <figcaption>Football · Photo {{ forloop.index }}</figcaption>
      </figure>
      {% endfor %}
    </div>
  </section>

  <section class="sports-section">
    <h2>Cycling</h2>
    <p>
      Cycling is another activity featured in my collection. The gallery
      below brings together cycling photographs. Individual locations,
      dates and stories can be added to each image later.
    </p>
    <div class="sports-gallery">
      {% assign cycling_images = "cycling-1.jpg,cycling-2.jpg,cycling-3.jpg,cycling-4.jpg,cycling-5.jpg,cycling-6.jpg,cycling-7.jpg,cycling-8.jpg,cycling-9.jpg,cycling-10.jpg,cycling-11.jpg,cycling-12.jpg,cycling-14.jpg" | split: "," %}
      {% for image in cycling_images %}
      <figure class="sports-photo">
        <img src="{{ site.baseurl }}/images/sports/{{ image }}" alt="Cycling photo {{ forloop.index }}" loading="lazy">
        <figcaption>Cycling · Photo {{ forloop.index }}</figcaption>
      </figure>
      {% endfor %}
    </div>
  </section>

  <section class="sports-section">
    <h2>Chess</h2>
    <p>
      Chess is included among my other sporting interests.
      More details about the photograph can be added later.
    </p>
    <div class="sports-gallery">
      <figure class="sports-photo">
        <img src="{{ site.baseurl }}/images/sports/chess-1.jpg" alt="Chess photograph" loading="lazy">
        <figcaption>Chess · Photo 1</figcaption>
      </figure>
    </div>
  </section>

  <section class="sports-section">
    <h2>Badminton</h2>
    <p>
      A glimpse of another sporting activity from my collection.
    </p>
    <div class="sports-gallery">
      <figure class="sports-photo">
        <img src="{{ site.baseurl }}/images/sports/badminton-1.jpeg" alt="Badminton photograph" loading="lazy">
        <figcaption>Badminton · Photo 1</figcaption>
      </figure>
    </div>
  </section>

  <section class="sports-section">
    <h2>Other Sports &amp; Activities</h2>
    <p>
      This section is reserved for other athletic moments and activities.
      More details can be added as the collection grows.
    </p>
    <div class="sports-gallery">
      <figure class="sports-photo">
        <img src="{{ site.baseurl }}/images/sports/athlete-1.jpg" alt="Athletic activity photograph" loading="lazy">
        <figcaption>Sports &amp; Activities · Photo 1</figcaption>
      </figure>
    </div>
  </section>

</div>
