+++
author = "Hélène"
title = "Keynote of Frédéric Loulergue at GDR GPL 2025, Pau, France"
date = "2025-06-24"
description = "Keynote of Frédéric Loulergue at GDR GPL 2025"
tags = [
    "keynote",
]
categories = [
    "talks",
]
series = ["Keynotes"]
toc = true
+++
<!--more-->

Frédéric (partner of the project) has given the 18th of June a keynote at [GDR GPL 2025](https://gdrgpl2025.sciencesconf.org/resource/page/id/4) (in French)

Slide are available [here](../../gdr.pdf)!

## Titre

Approches formelles pour les composants et outils système

## Résumé

Cet exposé présentera des approches formelles d’une part pour la vérification de composants système et d’autre part pour la formalisation d’outils système. Dans la première partie, on considérera des programmes C, tandis que dans la seconde, on considérera des langages de configuration.

Frama-C est un framework pour l’analyse et la vérification de programmes C. Il propose une collection d’analyses sous forme de greffons qui peuvent collaborer, parmi lesquels EVA pour l’analyse statique par interprétation abstraite, WP pour la vérification déductive, E-ACSL pour la vérification dynamique, RTE pour la génération d’annotation pour assurer l’absence de Runtime Error ou encore MetACSL pour la vérification de propriétés de haut-niveau. Nous aborderons les fonctionnalités de Frama-C via des cas d’études de composants systèmes avec un focus sur la vérification déductive, mais aussi ses limites et quelques recherches en cours pour les repousser, notamment dans le cadre du projet ANR CoMeMoV.

Les grands systèmes logiciels distribués sont désormais omniprésents. Les systèmes à base de composants offrent un moyen pratique de structurer de grands systèmes, en particulier les systèmes déployés dans le Cloud, au cœur ou à la périphérie du réseau. Les opérations DevOps, fournies par divers outils, qui incluent la configuration et la reconfiguration de système, sont nécessaires pour gérer divers types de scénarios tels que la tolérance aux pannes, l'évolutivité, les mises à jour logicielles ou diverses optimisations. De tels changements peuvent entraîner des incidents. Le principal avantage des outils DevOps est leur intégration et leur adoption dans la communauté DevOps. Leur inconvénient est qu'ils manquent de spécifications formelles et mêmes textuelles. L’exposé présentera nos premiers efforts, dans le contexte du projet **ANR For-CoaLa**, pour améliorer la compréhension de ces langages en se basant sur des sémantiques formelles mécanisées.

