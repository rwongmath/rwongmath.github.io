---
permalink: /teaching/socialhours
title: "Social office hours"

layout: single

toc: true
toc_label: "Content"
toc_icon: "user-friends"

---

They are a way for you to get to know me, your classmates and peers at UCLA, and professional mathematicians!

As a faculty associate at [McMurtry College](https://mcmurtry.rice.edu/), I will typically have lunch at West Servery on Thursdays from 12-1pm. If you see me there, feel free to sit down and chat!

Once or twice a semester, I will invite guest mathematicians to attend special office hours, where they can share details about their journey through mathematics, why they chose to pursue math, and to answer any questions that you have for them.

## Previous Guests:

<ul>
{% for guest in site.data.socialofficehours %}
<li><a href="{{ guest.website }}"> {{ guest.fancyname }}</a> visited in {{ guest.visit }}{% if guest.virtual == true %}
  (virtually, via Zoom){% endif %}.
</li>
{% endfor %}
</ul>
