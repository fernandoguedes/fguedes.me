---
categories:
- Hugo
- Deploy
- Automação
date: 2019-02-04
published: true
status: publish
tags:
- cd
- travis-ci
- tutorial
title: 'Deploy automatizado no GitHub Pages do "Hugo" utilizando Travis CI'
type: post
author: Luís Fernando Guedes
url: /2019/02/16/automatizando-hugo-travis-ci/
---

![Pipelines](/microservices/trainyard.jpg)

> Meu objetivo com esse post é te ajudar com a automação do seu projeto
desenvolvido utilizando Hugo como __framework__ de geração estática de conteúdo.

# Introdução

Já existem diversos tutoriais ensinando a configurar o [Hugo](https://gohugo.io/getting-started/) e também como transformar o seu projeto em [GitHub Pages](https://pages.github.com/), por isso vou partir do principío que você já tem um projeto Hugo configurado e o repositório criado.

Uso o [CNAME](https://help.github.com/articles/using-a-custom-domain-with-github-pages/) para poder "relacionar" meu domínio próprio com o GitHub Pages, resolvi seguir pela linha de ter dois repositórios, em um eu mantenho os [arquivos originais do Hugo](https://github.com/fernandoguedes/fguedes.me) e em outro eu mantenho os arquivos já [__buildados__](https://github.com/fernandoguedes/fernandoguedes.github.io) e expostos na pasta `public/`.

# Etapas

