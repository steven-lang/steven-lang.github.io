---
title: Specifying and Checking File System Crash-Consistency Models
summary: Talk for the Operating Systems seminar at JGU Mainz
tags:
- Operating Systems
date: "2016-09-04T00:00:00Z"

image:
  caption: 
  focal_point: Smart

url_pdf: "pdf/bs-seminar/paper.pdf"
url_slides: "pdf/bs-seminar/presentation.pdf"
---

### Abstract (German)

Die heutigen POSIX Dateisystem Schnittstellen besitzen keine klare Definition der resultierenden Zustände eines Systemabsturzes. Dies ist problematisch für Anwendungen, welche auf persistenten Speicher zurückgreifen um den ursprünglichen Zustand nach einem solchen Systemabsturz wiederherzustellen. Die Schwierigkeit für Entwickler besteht nun darin, die Reihenfolge und Abhängigkeit zwischen Dateisystem Operationen zu verstehen. Dies kann zu unvorhersehbarem Fehlverhalten, korrupten Anwendungszuständen und im schlimmsten Fall sogar zum Verlust der Daten führen.

Diese Ausarbeitung beschreibt Absturz-Konsistenz Modelle, analog zu Speicher-Konsistenz Modellen. Sie bestehen aus den folgenden zwei Bestandteilen: Litmus Tests, welche erlaubte und verbotene Verhalten von Dateisystemen zeigen und axiomatische Spezifikationen, welche zulässige Absturzverhalten deklarativ mit einer Menge an Axiomen beschreiben, sowie operationale Spezifikationen, bestehend aus abstrakten Automaten, die relevante Aspekte eines Dateisystem simulieren können.

Des weiteren wird das Framework *FERRITE* beschrieben, mit dem man Absturz-Konsistenz Modelle ausarbeiten und gegen echte Dateisysteme validieren kann.
