---
title: Workshop "Reproduzierbare Forschung in der Praxis mit R"
description: |
  Herzlich willkommen zum Workshop Reproduzierbare Forschung in der Praxis mit R ...
image: https://raw.githubusercontent.com/crsh/reproducible-research-practices-workshop/main/src/slides/img/Rlogo.png
---

:::info
<div style="text-align: center"> 🚧 
    <br>
    <p>
        <b>Dies ist ein "lebendiges" Dokument.</b><br>
        Es ist möglich, dass einige Aktuallisierungen und Ergänzungen nach dem ersten Seminar-Block vorgenommen werden.
    </p>
    </div>

:::

# Workshop "Reproduzierbare Forschung in der Praxis mit R"

[José C. García Alanis](https://methoden.amd.psychologie.uni-mainz.de/jose-c-garcia-alanis/)
[Abteilung für Analyse und Modellierung komplexer Daten](https://methoden.amd.psychologie.uni-mainz.de/)\
Psychologisches Institut
Johannes Gutenberg-Universität Mainz
Wallstraße 3, Raum 06-255\
D-55122 Mainz\
[jose.alanis at uni-mainz.de](jose.alanis@uni-mainz.de)


## Inhalt des Workshops

Seit mehreren Jahren sieht sich die psychologische Wissenschaft einer Vertrauenskrise gegenüber, die durch Bedenken bezüglich niedriger Erfolgsraten bei der Replikation empirischer Ergebnisse befeuert wird. Verschiedene Lösungen wurden vorgeschlagen, um dieses Problem anzugehen. Ein Schlüsselfaktor bei diesen Bemühungen ist die Steigerung der Transparenz und der computergestützten Reproduzierbarkeit psychologischer Forschung. Obwohl transparente und computergestützt reproduzierbare Forschung nicht zwangsläufig besser replizierbar ist, erleichtert sie Replikationsversuche und trägt dazu bei, Vertrauen in empirische Ergebnisse zu schaffen. Das sich entwickelnde Open-Science-Ökosystem bietet eine Vielzahl von Werkzeugen und Diensten, die zur Implementierung reproduzierbarer Forschungspraktiken genutzt werden können. Die Navigation im wachsenden Raum der Werkzeuge und Praktiken kann jedoch eine entmutigende Aufgabe sein.

Daher ist das Ziel dieses zweitägigen Workshops, Forscherinnen und Forschern die wesentlichen Komponenten maßgeschneiderter, reproduzierbarer Forschungsabläufe sowie die Werkzeuge für deren Umsetzung vorzustellen. Durch die Kombination von Vorträgen mit praktischen Hands-On-Sitzungen wird der Workshop den Schwerpunkt auf Datenanalyse, Ergebnisberichterstattung und Datenaustausch legen. Im Hinblick auf den Werkzeugstapel wird der Workshop die Versionskontrolle mit Git und das Erstellen von Berichten mit R Markdown als Schlüsselkomponenten eines reproduzierbaren Forschungsablaufs abdecken.


## Lernziele

Nach Abschluss des Kurses sollten die Teilnehmerinnen und Teilnehmer

1. mit den Schlüsselkonzepten der reproduzierbaren Forschung vertraut sein
2. in der Lage sein, die geeigneten Werkzeuge für die Implementierung eines für sie maßgeschneiderten Arbeitsablaufs auszuwählen
3. grundlegende Kenntnisse in `R Markdown`, `papaja` und `Git`  erworben haben
4. **Bonus**: In der Lage sein, Projekte zu verwalten und `Git` (und GitHub), um die Zusammenzuarbeit mit anderen zu erleichtern


## Vorbereitungen

Teilnehmerinnen und Teilnehmer sollten grundlegende Kenntnisse in R und etwas Erfahrung mit RStudio haben.

### Sofware und R-Pakete

Für die Hands-On-Teile des Workshops müssen Sie [`R`](https://www.r-project.org/) (Version 4.0.0 oder höher), [`Git`](https://git-scm.com/), [*RStudio*](https://www.rstudio.com/products/rstudio/download/) sowie die R-Pakete [`tinytex`](https://yihui.org/tinytex/) und [`papaja`](https://github.com/crsh/papaja).  installieren.

### Zusätzliche Funktionalität

:::warning
<div style="text-align: center"> 🚧 
    <br>
    <p>
        <b>Achtung.</b><br>
        Das Einrichten eines GitHub-Kontos ist für diesen Workshop <b>nicht zwingend notwendig</b>. Bei Bedarf kann GitHub während des Workshops eingerichtet werden.
    </p>
    </div>

:::

Sie sollten außerdem ein [*GitHub*](https://github.com/) einrichten oder ein Konto für die von Ihrer Einrichtung gehostete GitLab-Instanz (falls vorhanden und Sie es nutzen möchten). Zur Einrichtung von `Git` und *GitHub* für die Nutzung mit *RStudio* beziehen Sie sich auf [*Happy Git and GitHub for the useR*](https://happygitwithr.com/).


## Module

| Tag | Thema | Dauer | Slides | Übungen | Lösungen |
| ---: | :---- | ------: | :----: |:-------:|:--------:|
| 1 | System-Einrichtung & trouble shooting | ~ 1 hrs | [HTML](https://hackmd.io/@JoseAlanis/BJ-lr0pJp) |    -    |    -     |
| 1 | Einführung | ~ 2 hrs | [HTML](https://josealanis.github.io/WoMepS-2023-reproduceR/slides/1_introduction.html#1)|   ⌛\*   |    -     |
| 1 | R Markdown | ~ 2 hrs | ⌛ |    ⌛    |
| 2 | papaja | ~ 1.5 hrs | ⌛ |    ⌛    |
| 2 | Git & GitHub | ~ 1 hr | ⌛ |    ⌛    |
| 2 | Git & RStudio | ~ 1 hr | ⌛ |    ⌛    |
| (2) | Weitere Themen reproduzierbarer Wissenschaft | ~ 1.5 hrs | ⌛ |    ⌛    |    -     |


\*⌛: Wird später freigeschaltet.

## Citation

Dieser Workshop basiert zum großen Teil auf dem Workshop *"Workshop on reproducible research practices for psychologists" von Aust, F., & Breuer, J. (2022)*. Bitte benutzen Sie die folgende Referenz, wenn Sie diese Materialien weiterverwenden und teilen.

> Aust, F., & Breuer, J. (2022). Workshop on reproducible research practices for psychologists. https://github.com/crsh/reproducible-research-practices-workshop

## Acknowledgements

Die Workflow-Empfehlungen in diesem Workshop basieren auf Klein, O., Hardwicke, T. E., Aust, F., Breuer, J., Danielsson, H., Hofelich Mohr, A., … Frank, M. C. (2018). Ein praktischer Leitfaden für Transparenz in der Psychologischen Wissenschaft. Collabra: Psychology, 4(1). doi: [10.1525/collabra.158](https://doi.org/10.1525/collabra.158) ([Supplementary material](
http://psych-transparency-guide.uni-koeln.de/))

