---
layout: default
title: Past Speakers & Fellows
nav_title: Past Speakers & Fellows
permalink: /past-speakers-and-fellows/
order: 1
---

# Past Speakers
<div class="card-container">
{% for speaker in site.data.speakers %}
  <div class="person-card">
    <div class="person-card-image-container">
      <img src="/images/{{ speaker.image }}" />
    </div>
    <div class="person-card-text-container">
      <h3>{{ speaker.name }}</h3>
      <p>{{ speaker.bio }}</p>
    </div>
  </div>
{% endfor %}
</div>

# Past Fellows
<div class="card-container">
{% for speaker in site.data.speakers %}
  <div class="person-card">
    <h3>{{ speaker.name }}</h3>
    <p>{{ speaker.bio }}</p>
  </div>
{% endfor %}
</div>
