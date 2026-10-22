+++
author = "Olivia and Eloi"
title = "Olivia Proust and Eloi Perdereau presented their work at the CONFLANG'26 workshop"
date = "2026-10-22"
description = "Olivia and Eloi at CONFLANG'26"
tags = [
    "talk",
]
categories = [
    "talks",
]
series = ["Talks"]
toc = true
+++
<!--more-->

The [CONFLANG'26 workshop](https://conf.researchr.org/home/ase-2026/conflang-2026), co-hosted with the [ASE 2026 conference](https://conf.researchr.org/home/ase-2026), held at Munich the Monday, October 12.
During this occasion, the For-CoaLa team was well represented. Two members assisted the workshop and gave talks presenting their work.

Olivia presented her ongoing PhD work about the analysis of variable scopes in [Ansible](https://www.ansible.com).
She exposed the ambiguities and peculiarities of Ansible's scope precedence, and presented her solution, Scopeannon, a static analysis tool that reports the scopes consulted when evaluating expressions in an Ansible playbook.
Practitioners can use this information to identify unexpected scope selection or unintended variable overrides, hence augmenting the reliability of Ansible code.

This work is published as a short paper in the workshop's proceedings.

* *Olivia Proust*, *Hélène Coullon*, *Jolan Philippe*, *Frédéric Loulergue*, **Scopeannon: A Static Analyzer of Ansible’s Scope Ambiguities**. In Proceedings of the 3rd International Workshop on Configuration Languages (ConfLang '26), ACM, 2026. [doi](https://dl.acm.org/doi/10.1145/3844136.3845868), [PDF](../conflang26-scopeannon.pdf), [slides](../conflang26-scopeannon-slides.pdf).

![Olivia at CONFLANG'26](../conflang26-olivia.jpeg)


Eloi gave two talks, presenting the work done during his past position at IMT Atlantique as part of the [Taranis project](https://taranis-cloud.fr/) of the [Cloud PEPR](https://pepr-cloud.fr/fr/projet-taranis/).
The first presentation was about the CUE language. He exposed the interpretation and execution semantics of a fragment of CUE that retains the core of the language.
Despite the fragment being minimal, it shows some non obvious behaviors regarding the interaction of references and unification.
The second presentation concerned the provisioning engine [Terraform](https://terraform.io) and the problems that might occur during executions, simply due to the ordering of actions updating the state (Create, Update or Delete).
The presented solution, BPlan, builds upon an operational semantics of Terraform executions.
By defining LTL stability properties and verifying them with model-checking, BPlan is able to capture issues before the actual execution.

These works were submitted as extended abstract and hence are not part of the proceedings.

* *Eloi Perdereau*, *Jacques Noyé*, **How to represent CUE terms as graphs**. 2026. [PDF](), [slides]().
* *Eloi Perdereau*, *Daniel Sokolowski*, *Jolan Philippe*, *Hélène Coullon*, *Guido Salvaneschi*, **Verifying the Stability of Terraform Executions**. 2026. [PDF](../conflang26-terraform-stability.pdf), [slides](../conflang26-terraform-stability-slides.pdf).


![Eloi at CONFLANG'26](../conflang26-eloi.jpeg)

