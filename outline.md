---
title: Workshop "Reproduzierbare Forschung in der Praxis mit R (preparations)"
subtitle: "Workshop outline"
author  : "José C. García Alanis"

date    : "25.-26.09.2023"
location: "Goethe-Universität Frankfurt"

abstract: |
  Seit mehreren Jahren sieht sich die psychologische Wissenschaft einer Vertrauenskrise gegenüber, die durch Bedenken bezüglich niedriger Erfolgsraten bei der Replikation empirischer Ergebnisse befeuert wird. Verschiedene Lösungen wurden vorgeschlagen, um dieses Problem anzugehen. Ein Schlüsselfaktor bei diesen Bemühungen ist die Steigerung der Transparenz und der computergestützten Reproduzierbarkeit psychologischer Forschung. Obwohl transparente und computergestützt reproduzierbare Forschung nicht zwangsläufig besser replizierbar ist, erleichtert sie Replikationsversuche und trägt dazu bei, Vertrauen in empirische Ergebnisse zu schaffen. Das sich entwickelnde Open-Science-Ökosystem bietet eine Vielzahl von Werkzeugen und Diensten, die zur Implementierung reproduzierbarer Forschungspraktiken genutzt werden können. Die Navigation im wachsenden Raum der Werkzeuge und Praktiken kann jedoch eine entmutigende Aufgabe sein.

  Daher ist das Ziel dieses zweitägigen Workshops, Forscherinnen und Forschern die wesentlichen Komponenten maßgeschneiderter, reproduzierbarer Forschungsabläufe sowie die Werkzeuge für deren Umsetzung vorzustellen. Durch die Kombination von Vorträgen mit praktischen Hands-On-Sitzungen wird der Workshop den Schwerpunkt auf Datenanalyse, Ergebnisberichterstattung und Datenaustausch legen. Im Hinblick auf den Werkzeugstapel wird der Workshop die Versionskontrolle mit Git und das Erstellen von Berichten mit R Markdown als Schlüsselkomponenten eines reproduzierbaren Forschungsablaufs abdecken.

output:
html_document:
keep_md       : true
theme         : "spacelab"
df_print      : "kable"
toc           : true
toc_float     : true
---

# Workshop "Reproduzierbare Forschung in der Praxis mit R"

[José C. García Alanis](https://methoden.amd.psychologie.uni-mainz.de/jose-c-garcia-alanis/)
[Abteilung für Analyse und Modellierung komplexer Daten](https://methoden.amd.psychologie.uni-mainz.de/)\
Psychologisches Institut
Johannes Gutenberg-Universität Mainz
Wallstraße 3, Raum 06-255\
D-55122 Mainz\
[jose.alanis at uni-mainz.de](jose.alanis@uni-mainz.de)

## Voraussetzungen

Teilnehmerinnen und Teilnehmer sollten grundlegende Kenntnisse in R und etwas Erfahrung mit RStudio haben.


# Vorbereitungen

### R and RStudio

Bitte stellen Sie sicher, dass Sie eine aktuelle Version von R (≥ 4.0.0) und RStudio verwenden.

### LaTeX

Um das vollständige Funktionsset von `papaja` nutzen zu können, benötigen Sie eine [TeX](http://de.wikipedia.org/wiki/TeX)-Distribution.
Wir empfehlen, dass Sie [TinyTex](https://yihui.name/tinytex/) verwenden, eine LaTeX-Distribution, die für die Verwendung mit R Markdown konzipiert ist.
TinyTex kann wie folgt innerhalb von R installiert werden.


```r
# If necessary, install tinytex R package
if(!requireNamespace("tinytex", quietly = TRUE)) install.packages("tinytex")

# Install TinyTex distribution
tinytex::install_tinytex()
```

Falls Sie möchten, können Sie auch [MikTeX](http://miktex.org/) für Windows, [MacTeX](https://tug.org/mactex/) für Mac oder [TeX Live](http://www.tug.org/texlive/) für Linux verwenden.
Beziehen Sie sich ebenfalls auf das [`papaja` manual](https://crsh.github.io/papaja_man/introduction.html#getting-started) für Anweisungen.


#### `papaja`

`papaja` kann folgendermaßen installiert werden:


```r
# Install latest CRAN release
install.packages("papaja")
```

### Git and GitHub

:::warning
<div style="text-align: center"> 🚧 
    <br>
    <p>
        <b>Achtung.</b><br>
    Das Einrichten eines GitHub-Kontos ist für diesen Workshop **nicht zwingend notwendig**. Bei Bedarf kann GitHub während des Workshops eingerichtet werden.
    </p>
    </div>

:::


Wir werden Git für die Versionskontrolle (Änderungsnachverfolgung) und als Werkzeug für die Zusammenarbeit verwenden. Die folgenden Schritte können zunächst entmutigend sein, aber die verlinkten Anleitungen sind ausgezeichnet und sollten Ihnen helfen, sich schnell einzurichten. Sie schaffen das! :)

Gehen Sie folgendermaßen vor:

1. Erstellen Sie ein [GitHub](https://github.com)-Konto
2. Installieren Sie Git (see [instructions](https://happygitwithr.com/install-git.html))
   - Während der Installation von Git, fügen Sie `git bash` zum Windows-Kontextmenü hinzu, indem Sie die entsprechende Option auswählen (dies sollte die Standardeinstellung sein)
3. Konfigurieren Sie Git (see [ instructions](https://happygitwithr.com/hello-git.html))
4. Erstellen Sie einen persönlichen Zugriffstoken für HTTPS (see [instructions](https://happygitwithr.com/https-pat.html))
5. bestätigen Sie, dass Sie eine Verbindung zu GitHub herstellen können (see [instructions](https://happygitwithr.com/push-pull-github.html))
