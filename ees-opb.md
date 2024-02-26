Et si Parcoursup était compté
================
Pauline Boyer, <pauline.boyer@cnrs.fr>Julien Gossa,
<gossa@unistra.fr>Université de Strasbourg

Projet d’article pour « Orientation post-bac : Parcoursup et
l’introduction de la sélection à l’université – Varia (72/juin 2024) ».

Axes : transversal.

## Introduction

Les données proviennent pour l’essentiel de la plateforme de données
ouvertes du ministère [^1] [^2] [^3] [^4] [^5] [^6], également utilisée
pour alimenter Parcoursup, ses tableaux de bord, et les notes
d’information du ministère.

Les traitements sont effectués en R (Xie, Allaire, and Grolemund 2019)
et les représentations en ggplot (Wickham 2009 ; Wilke 2019). Ils sont
mis en ligne et librement accessibles sur la plateforme GitHub[^7],
ainsi que les brouillons exploratoires [^8]. Les irrégularités ou
incohérences apparentes sont systématiquement discutées publiquement sur
le réseau social Twitter.

## Mesurer Parcoursup

### Qualité de l’affectation : de la `satisfaction de l'affectation` à la `satisfaction d'utilisation de la plateforme`

<img src="figs/ipsos.png" title="Enquête IPSOS Opinion des néo-bacheliers sur Parcoursup, septembre 2022" alt="Enquête IPSOS Opinion des néo-bacheliers sur Parcoursup, septembre 2022" width="100%" style="display: block; margin: auto;" />

### Qualité de l’affectation : de la `satisfaction` au `débit`

<img src="ees-opb_files/figure-gfm/aff-1.png" title="Tableaux de bord Parcoursup et vitesse de l'affectation" alt="Tableaux de bord Parcoursup et vitesse de l'affectation" width="100%" style="display: block; margin: auto;" />

### Offre de formation : `taille` et `nombre de formations`

<img src="ees-opb_files/figure-gfm/odf-1.png" title="Formations et admissions par taille de formation" alt="Formations et admissions par taille de formation" width="100%" style="display: block; margin: auto;" />

## Offre de formation : de la `pression` au `taux d'accès`

<img src="ees-opb_files/figure-gfm/sel-1.png" title="Sélectivité des formations de Parcoursup" alt="Sélectivité des formations de Parcoursup" width="100%" style="display: block; margin: auto;" />

<img src="ees-opb_files/figure-gfm/sel.taux-1.png" title="Sélectivité des formations de Parcoursup" alt="Sélectivité des formations de Parcoursup" width="100%" style="display: block; margin: auto;" />

### `Places non pourvues`, `Places vacantes` et `Taux de remplissage`

<img src="ees-opb_files/figure-gfm/pnp-1.png" title="Taux de remplissage des formations post-bac" alt="Taux de remplissage des formations post-bac" width="100%" style="display: block; margin: auto;" />

<img src="ees-opb_files/figure-gfm/tdr.disp-1.png" title="Taux de remplissage des formations post-bac" alt="Taux de remplissage des formations post-bac" width="100%" style="display: block; margin: auto;" />

## `Taux de poursuite d'étude` et `Nombre de non poursuites d'étude`

<img src="ees-opb_files/figure-gfm/pe-1.png" title="Taux de poursuite et nombre de non-poursuites d'étude des néo-bacheliers" alt="Taux de poursuite et nombre de non-poursuites d'étude des néo-bacheliers" width="100%" style="display: block; margin: auto;" />

## Informations additionnelles

### sur déclaration de capacités

<details>
<summary>
Surdéclarants
</summary>

| Session | capacité_plus_1000 | nb_formations |
|--------:|:-------------------|--------------:|
|    2016 | FALSE              |           446 |
|    2016 | TRUE               |            68 |
|    2017 | FALSE              |           358 |
|    2017 | TRUE               |            40 |
|    2018 | FALSE              |           207 |
|    2018 | TRUE               |             2 |
|    2019 | FALSE              |            96 |
|    2019 | TRUE               |             7 |
|    2020 | FALSE              |            51 |
|    2020 | TRUE               |             9 |
|    2021 | FALSE              |            74 |
|    2021 | TRUE               |            12 |
|    2022 | FALSE              |            84 |
|    2022 | TRUE               |            12 |

</details>

### Taux remplissage

<img src="ees-opb_files/figure-gfm/unnamed-chunk-2-1.png" width="100%" style="display: block; margin: auto;" />
<img src="ees-opb_files/figure-gfm/unnamed-chunk-3-1.png" width="100%" style="display: block; margin: auto;" />

<img src="ees-opb_files/figure-gfm/unnamed-chunk-4-1.png" width="100%" style="display: block; margin: auto;" />

<div id="refs" class="references csl-bib-body hanging-indent">

<div id="ref-wickham_ggplot2_2009" class="csl-entry">

Wickham, Hadley. 2009. *Ggplot2: Elegant Graphics for Data Analysis*.
Use R! New York: Springer.

</div>

<div id="ref-wilke_fundamentals_2019" class="csl-entry">

Wilke, Claus. 2019. *Fundamentals of Data Visualization: A Primer on
Making Informative and Compelling Figures*. First edition. Beijing
Boston Farnham Sebastopol Tokyo: O’Reilly.

</div>

<div id="ref-xie_r_2019" class="csl-entry">

Xie, Yihui, Joseph J. Allaire, and Garrett Grolemund. 2019. *R Markdown:
The Definitive Guide*. Chapman & Hall/CRC, the R Series. Boca Raton
London New York: CRC Press, Taylor & Francis Group.

</div>

</div>

[^1]: <https://data.enseignementsup-recherche.gouv.fr/explore/dataset/fr-esr-parcoursup/>

[^2]: <https://data.enseignementsup-recherche.gouv.fr/explore/dataset/fr-esr-parcoursup_2020/>

[^3]: <https://data.enseignementsup-recherche.gouv.fr/explore/dataset/fr-esr-parcoursup-2019/>

[^4]: <https://data.enseignementsup-recherche.gouv.fr/explore/dataset/fr-esr-parcoursup-2018/>

[^5]: <https://data.enseignementsup-recherche.gouv.fr/explore/dataset/fr-esr-apb_voeux-et-admissions/>

[^6]: <https://data.enseignementsup-recherche.gouv.fr/explore/dataset/fr-esr-taux-poursuite-enseignement-superieur-par-academie/>

[^7]: <https://github.com/juliengossa/parcoursup/>

[^8]: <https://github.com/cpesr/RFC/>
