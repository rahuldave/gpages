---
title: The Case of the Italian Olives
---

This is the home page

## Lets have fun

>here is a quote

Here is *emph* and **bold**.

Here is some inline math $\alpha = \frac{\beta}{\gamma}$ and, of-course, E rules:

$$G_{\mu\nu} + \Lambda g_{\mu\nu}  = 8 \pi T_{\mu\nu} .$$

## Blog Posts

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
