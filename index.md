---
layout: default
title: Документация
---
# Документация StudyFlow

Рабочие материалы учебного проекта: описание команды и календарь предстоящих событий.

## С чего начать

Откройте [Наша команда]({{ '/our-team/' | relative_url }}), чтобы узнать об участниках, ответственности и порядке внесения изменений.

## Предстоящие события

{% assign events = site.pages | where: "section", "events" | sort: "source_name" %}
<ul data-event-list>
{% for event in events %}<li data-page="{{ event.source_name | escape }}"><a href="{{ event.url | relative_url }}">{{ event.title | escape }}</a></li>{% endfor %}
</ul>

Даты событий — учебные примеры, а не официальный график занятий.

## О проекте

StudyFlow помогает организовать учебные задачи по предметам, срокам и статусам. [Описание проекта и Wiki](https://github.com/mirea-studyflow-bandukov-ilya/studyflow/wiki).
