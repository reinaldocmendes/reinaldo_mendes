---
layout: page
permalink: /about/index.html
title: Reinaldo Carlos Mendes
tags: [Mendes, Reinaldo, reinaldocmendes]
imagefeature: fourseasons.jpg
chart: true
---
<figure>
  <img src="{{ site.url }}/images/rm_400x400.png" alt="Reinaldo Carlos Mendes">
  <figcaption>Reinaldo Carlos Mendes</figcaption>
</figure>

{% assign total_words = 0 %}
{% assign total_readtime = 0 %}
{% assign featuredcount = 0 %}
{% assign statuscount = 0 %}

{% for post in site.posts %}
    {% assign post_words = post.content | strip_html | number_of_words %}
    {% assign readtime = post_words | append: '.0' | divided_by:200 %}
    {% assign total_words = total_words | plus: post_words %}
    {% assign total_readtime = total_readtime | plus: readtime %}
    {% if post.featured %}
    {% assign featuredcount = featuredcount | plus: 1 %}
    {% endif %}
{% endfor %}


Meu nome é **Reinaldo Carlos Mendes** e esse é um site para falar sobre computação. Aqui nesse site você vai encontrar temas como **_Inteligência Artificial, Mineração de Dados, Linguagens de Programação, Sistemas embarcados, Bancos de Dados e muito mais!_**

Sou engenheiro da computação com especialização em banco de dados. Com 10 anos de atuação no mercado privado administrando redes, desenvolvendo softwares, ministrando aulas, atualmente sou pesquisador e aluno no curso de mestrado em modelagem matemática e computacional, no qual, foco minha pesquisa em aprendizado de máquina (Deep Learning).

Hoje minhas atenções estão voltadas para o campo da inteligência artificial e Análise de Dados, tema qual será bastante recorrente aqui no site.

***_Reinaldo C. Mendes_
_Engenheiro da Computação_***
