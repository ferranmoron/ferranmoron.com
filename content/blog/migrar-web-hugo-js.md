---
title: "Migrar la web a Hugo js i AWS"
date: 2020-03-10T07:54:00+01:00
draft: false

# meta description
description: "Projecte de migració d'una web estàtica a Hugo js i Amazon Web Services S3"

# post thumb
image: "/images/hugojs.jpg"

# taxonomies
categories: 
  - "webdev"
tags:
  - "cms"
  - "aws"

# post type
type: "top3"

---

Fa unes setmanes vaig decidir migrar aquesta web personal a un nou hosting i fer servir un dels nous Flat File CMS o *static site generators* que hi ha al mercat i que són open-source.

## Hosting

Pel tema del hosting, vaig decidir experimentar amb [AWS](https://aws.amazon.com/) (Amazon Web Services). La primera vegada que hi arribes tot sembla molt complicat. Per començar, has de crear un compte AWS per accedir a totes les funcionalitats.

En el meu cas he fet servir:

* S3 per allotjar les pàgines estàtiques
* Cloudfront per publicar el site
* Certificate Manager pel tema del https
* Route 53 pel domini

No és difícil però has d'anar seguint molt bé tots els tutorials propis d'AWS i algun vídeo de Youtube amb instruccions com aquest [Hosting a static website with HTTPS on an S3 bucket](https://youtu.be/uwgB_sIhIko).

## Publicació

En aquest punt vaig estar fent recerca i finalment, gràcies al consell del meu company [Joan Ribas](https://www.linkedin.com/in/joan-ribas/), vaig decidir-me per fer servir [Hugo](https://gohugo.io/). Vaig estar mirant també [GatsbyJS](https://www.gatsbyjs.org/) i potser ho faré servir en algun altre projecte.

La veritat és que va ser molt senzill. Permet diferents idiomes sense cap complicació i es poden fer *partials* i modificar mòduls i templates. Ho desenvolupes tot en local i després fas el desplegament a Producció. En el meu cas, ho vaig connectar amb AWS i va ser molt senzill veure-ho tot funcionant com estava previst.

Molt recomanable. Encara he d'anar aprenent com funciona. Ja aniré explicant l'evolució del tema més endavant. 