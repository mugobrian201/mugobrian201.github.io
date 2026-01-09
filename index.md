---
layout: splash  # Or try 'home' or 'default' if splash doesn't work; Minima uses 'home' often
title: Brian Mugo
permalink: /
header:
  overlay_color: "#5e616c"
  overlay_image: /assets/images/home-bg.jpg
  caption: "Building predictive models that solve real-world problems in Africa and beyond"
  actions:
    - label: "View My Projects"
      url: "/projects/"
excerpt: "Actuarial Science graduate specializing in machine learning solutions for disaster response, urban planning, and environmental health. Currently expanding my skills through WorldQuant University's Applied Data Science Lab."
---

<p style="font-size:1.2em; text-align: center;">
Actuarial Science graduate specializing in machine learning solutions for disaster response, urban planning, and environmental health. Currently expanding my skills through WorldQuant University's Applied Data Science Lab.
</p>

## Featured Projects

<div style="display: flex; flex-wrap: wrap; justify-content: center; gap: 20px; margin: 40px 0;">
  <div style="flex: 1; min-width: 300px; max-width: 400px; text-align: center;">
    <img src="/assets/images/mexico-project-thumb.jpg" alt="Mexico Real Estate Analysis" style="width: 100%; border-radius: 8px;">
    <h3>Mexico Real Estate Analysis</h3>
    <p>Identified key factors influencing Mexican real estate prices using spatial analysis.</p>
    <a href="/projects/#mexico-real-estate-analysis" class="btn btn--primary">Explore Project</a>
  </div>

  <div style="flex: 1; min-width: 300px; max-width: 400px; text-align: center;">
    <img src="/assets/images/nepal-project-thumb.jpg" alt="Nepal Earthquake Prediction" style="width: 100%; border-radius: 8px;">
    <h3>Nepal Earthquake Prediction</h3>
    <p>Predicted building damage severity to optimize emergency resource allocation.</p>
    <a href="/projects/#nepal-earthquake-damage-prediction" class="btn btn--primary">Explore Project</a>
  </div>
</div>

## Featured Technical Skills

<!-- If you have a _data/skills.yml file, this loop will work; otherwise add manually -->
{% for skill in site.data.skills %}
### {{ skill.name }}
{{ skill.description }}
{% endfor %}


