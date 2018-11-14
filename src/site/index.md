---
title: Longshot
subtitle: This is a blog about long takes in films, a topic that has been of interest for the past many years.
layout: layouts/base.njk
---


## This site is a starting point

From this point we should already have:

- [Long Take (Wikipedia)](https://en.wikipedia.org/wiki/Long_take) with a skeleton site
- A date format filter for Nunjucks
- Sass pipeline
- JS pipeline
- JS [search index](/search.json) generator
- Serverless (FaaS) development pipeline with Netlify Functions for Lambda


## Post pages

The pages found in in the posts

<ul class="listing">
{%- for page in collections.post -%}
  <li>
    <a href="{{ page.url }}">{{ page.data.title }}</a> -
    <time datetime="{{ page.date }}">{{ page.date | dateDisplay }}</time>
  </li>
{%- endfor -%}
</ul>



