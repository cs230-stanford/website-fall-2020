---
layout: default
keywords:
comments: false

title: Office Hours
description: Times and locations may occasionally change each week; please check this page often.
buttons: [project_appt_calendly, nooks]
micro_nav: false
---

## Office Hours Table <a name="table"></a>

| TA | Project Office Hour Signup | Zoom URL |
|----|:--------------------------:|----------|
{% assign people = site.course.ta | concat: site.course.staff -%}
{% for ta in people -%}
{% unless ta.zoom_id == null -%}
| {{ ta.name }} | [Click to book]({{ ta.calendly }}) | [{{ ta.zoom_id }}]({{ ta.zoom_link }}) |
{% endunless -%}
{% endfor %}

Nooks link for Homework OH: [{{ site.course.nooks }}]({{ site.course.nooks }})

~~QueueStatus link for Homework OH: [{{ site.course.queuestatus.url }}]({{ site.course.queuestatus.url }})~~

## Google Calendar

**All Office Hours are held remotely over Zoom. Use the Zoom link above for the respective TA.**

<div>
<iframe src="https://calendar.google.com/calendar/embed?src=4g7an8rtkd4tssnkampke8g2tc%40group.calendar.google.com&ctz=America%2FLos_Angeles" style="border: 0" width="800" height="600" frameborder="0" scrolling="no"></iframe>
</div>
