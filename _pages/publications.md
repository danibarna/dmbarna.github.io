---
permalink: /publications/
---

## Under Review

**Regional index flood estimation at multiple durations with generalized additive models**  
**Danielle M. Barna**, Kolbjørn Engeland, Thomas Kneib, Thordis Thorarinsdottir, Chong-Yu Xu
*Environmetrics*  
[PDF](link-to-preprint) <!-- optional -->

## Selected Publications

### 2026

{% if site.data.publications %}
{% assign pubs_2024 = site.data.publications | where: "year", 2024 %}
{% for pub in pubs_2024 %}
**{{ pub.title }}**  
{{ pub.authors }}  
*{{ pub.venue }}*, {{ pub.year }}  
{% if pub.pdf %}[[PDF]({{ pub.pdf }})]{% endif %}
{% if pub.doi %}[[DOI](https://doi.org/{{ pub.doi }})]{% endif %}
{% if pub.code %}[[Code]({{ pub.code }})]{% endif %}
{% if pub.slides %}[[Slides]({{ pub.slides }})]{% endif %}
{% endfor %}
{% else %}

**The ability of LSTM to model snowmelt versus rainfall generated floods**  
Sigrid J. Bakke, **Danielle M. Barna**, Kolbjørn Engeland, Sjur Anders Kolberg, Sunniva Nordeide
*Hydrology and Earth System Sciences*, 2026  
[[NVE](https://hess.copernicus.org/articles/30/6207/2026/)] [[Code](#)]

{% endif %}

### 2023

**[Paper Title]**  
[Author1], **Your Name**, [Author3]  
*[Conference/Journal Name]*, 2023  
[[PDF](#)] [[DOI](#)]

**[Paper Title]**  
**Your Name**, [Coauthor]  
*[Workshop/Conference Name]*, 2023  
[[PDF](#)]

### 2022

**[Paper Title]**  
**Your Name**, [Coauthor1], [Coauthor2]  
*[Journal Name]*, 2022  
[[PDF](#)] [[DOI](#)]

## Thesis

**[Dissertation Title]**  
Ph.D. Thesis, [University Name], [Year]  
Advisor: [Advisor Name]  
[[PDF](#)]

## Preprints

**[Preprint Title]**  
[Authors]  
*arXiv preprint arXiv:XXXX.XXXXX*, [Year]  
[[arXiv](https://arxiv.org/abs/XXXX.XXXXX)]

---

<small>* indicates equal contribution</small>
