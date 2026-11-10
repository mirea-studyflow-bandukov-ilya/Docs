---
layout: default
title: Документация
---
# Документация StudyFlow

Рабочие материалы учебного проекта: описание команды и календарь предстоящих событий.

## С чего начать

Откройте [Our team]({{ '/our-team/' | relative_url }}), чтобы узнать об участниках, ответственности и порядке внесения изменений.

## Предстоящие события

{% assign events = site.pages | where: "section", "events" | sort: "source_name" %}
{% for event in events %}
- [{{ event.title }}]({{ event.url | relative_url }})
{% endfor %}

Даты событий — учебные примеры, а не официальный график занятий.

## О проекте

StudyFlow помогает организовать учебные задачи по предметам, срокам и статусам. [Описание проекта и Wiki](https://github.com/mirea-studyflow-bandukov-ilya/studyflow/wiki).
