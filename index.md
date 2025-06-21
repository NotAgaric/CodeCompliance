---
layout: default
title: Привет, я [Имя]!
subtitle: Веб-разработчик / UI дизайнер
---

![Аватар](/assets/images/avatar.jpg){:.avatar}

## Обо мне
Я специалист по... с опытом работы в... Мои основные навыки:

- Разработка на JavaScript/React
- UI/UX дизайн
- Оптимизация производительности

## Последние проекты
<div class="projects">
{% for project in site.portfolio limit:3 %}
  <div class="project-card">
    <a href="{{ project.url }}">
      <img src="/assets/images/{{ project.thumbnail }}" alt="{{ project.title }}">
      <h3>{{ project.title }}</h3>
    </a>
    <p>{{ project.short_description }}</p>
  </div>
{% endfor %}
</div>

[Смотреть все работы →](/portfolio)
