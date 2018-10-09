---
layout: post
title:  "gtf to bed"
date:   2018-10-8 22:14:54
categories: genome
tags: gtf linux genome
---

* content
{:toc}

```
awk 'OFS="\t" {if ($3=="gene") {print $1,$4-1,$5,$10,$16,$7}}'
Crassostrea_gigas.oyster_v9.37.gtf | tr -d '";'>Crassostrea_gigas.oyster_v9.37.bed```