# LaTeX-Vorlagen für das Corporate Design der DPSG

Die enthaltenen Logos sind ggf. urheberrechtlich geschützt und dürfen nur für verbandliche Zwecke der DPSG genutzt werden (vgl. https://dpsg.de/de/fuer-mitglieder/logos-design/logos-rund-um-die-dpsg.html).

# Benutzung
## Installation
Die Paketdateien müssen in einem Pfad liegen, in dem sie von TeX mittels Kpathsea gefunden werden.
Das kann das systemweite texmf-Verzeichnis (z. B. `/usr/share/texmf`) sein oder das benutzereigene (z. B. `~/texmf`).
Dort kann man die ganzen Dateien in ein neues Verzeichnis ablegen (z. B. `texmf/tex/latex/latex-dpsg/`).
Anschließend muss noch `texhash` aufgerufen werden, um den Index zu aktualisieren.

Anstelle der Installation können die Pakete auch einfach in das Verzeichnis mit der zu kompilierenden Quelldatei kopiert werden.

## Schriftarten
Die CD-Schriftarten müssen auf dem System installiert sein.
Es dürfte auch ausreichen, wenn sie in einem Pfad liegen, wo sie von TeX mittels Kpathsea gefunden werden.
Verwendet werden:
* Rockwell (z. B. in MS Office enthalten, sonst ist mir keine Quelle bekannt)
* Calibri (dürfte in modernen Windows-Versionen enthalten sein)

## LuaTeX
Die Vorlagen greifen auf die im System installierten TrueType-/OpenType-Schriftarten zu.
Deswegen können sie nur mit LuaLaTeX kompiliert werden (XeLaTeX könnte auch funktionieren ist aber nicht getestet).
Das heißt es muss `lualatex` anstelle von `pdflatex` aufgerufen werden.
LuaTeX sollte in jeder halbwegs aktuellen TeX-Distribution enthalten sein.
Eine kurze Einführung in LuaLaTeX gibt es hier: http://mirror.ctan.org/info/luatex/lualatex-doc/lualatex-doc.pdf

# Enthaltene Vorlagen
* beamer: Präsentationsvorlage für das LaTeX-Beamer-Paket, die die PowerPoint-Vorlage von der Bundeshomepage nachbaut.

# Verwendete Farben
Alle Farben sind im RGB-Format spezifiziert.
Die Farbwerte wurden aus dem CD-Leitfaden (Stand: Juli 2014) übernommen.
Die Farben können auch im eigenen Dokument verwendet werden (z. B. mit
`\color{dpsgrot}`).

Layoutfarben:
* `dpsgrot`: RGB(129, 10, 26), verwendet für den Strich der Wort-Bild-Marke und
  die Wegzeichen
* `dpsgblau`: RGB(0, 48, 86), verwendet für den Text der Wort-Bild-Marke
* `dpsgbeige`: RGB(236, 223, 203), beispielsweise für die Fußzeile in
  Präsentationen
* `dpsgmittelbeige`: RGB(199,189,173)

Stufenfarben:
* `dpsgwoes`: RGB(255,100,0)
* `dpsgjupfis`: RGB(47,83,167)
* `dpsgpfadis`: RGB(0,130,60)
* `dpsgrover`: RGB(204,31,47)
* `dpsgleiter`: RGB(177,185,173)
