---
permalink: /teaching/socialhours
title: "Social office hours"

layout: single

toc: true
toc_label: "Content"
toc_icon: "user-friends"

---

Social office hours are a way for you to get to know me, your classmates and peers at UCLA, and professional mathematicians!

Once or twice a quarter, I will invite guest mathematicians to attend special office hours, where they can share details about their journey through mathematics, why they chose to pursue math, and to answer any questions that you have for them.

## Previous Guests:

<ul>
{% for guest in site.data.socialofficehours %}
<li><a href="{{ guest.website }}"> {{ guest.fancyname }}</a> visited in {{ guest.visit }}{% if guest.virtual == true %}
  (virtually, via Zoom){% endif %}.
</li>
{% endfor %}
</ul>
