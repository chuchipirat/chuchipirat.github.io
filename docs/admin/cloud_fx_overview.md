---
layout: home
title: Cloud Functions Monitor
permalink: docs/admin/cloudfx_overview
nav_exclude: 
parent: System
search_exclude: true
---
# Cloud Functions Monitor
{: .no_toc }

<details markdown="block">
  <summary>
    Inhalt
  </summary>
  {: .text-delta }
- TOC
{:toc}
</details>

---

{: .intern-title }

> ☠️ Admin-Bereich ☠️
>
>Diese Seite ist für System-Admins.

Diverse Funktionen werden über Cloud Functions ausgeführt. Diese sind Codes, die in der Cloud laufen. Zum Beispiel wird dies genutzt, um Benutzer\*innen keinen direkten Zugriff auf sensible Daten zu gewähren. Der Cloud-Functions Monitor zeigt an, welche Cloud Function von wem ausgelöst wurde und welche Daten oder Parameter dabei verwendet wurden.

![Cloud-FX Monitor](https://github.com/chuchipirat/chuchipirat.github.io/blob/main/docs/admin/_images/cloud_functions_monitor.png?raw=true)


## Ansicht

Die angezeigte Tabelle zeigt an, wann welche Funktion von wem ausgeführt wurde. Bei Bedarf können weitere Spalten eingeblendet werden.

### Detailansicht

Wenn du auf das Icon am Anfang einer Zeile klickst, werden die alle Daten des Triggerdokumentes angezeigt.


## Löschen von Trigger-Dokumenten  

Um eine Cloud Function auszulösen, wird oft ein Dokument in einem Verzeichnis erstellt, das die erforderlichen Daten für die Cloud Function enthält. Diese Dokumente können nach ihrer Ausführung wieder gelöscht werden.

Du kannst über den Tab `Löschen` Cloud Function Trigger-Dokumente aus der Datenbank entfernen. Gib einfach die Anzahl der Tage ein, für die du die Protokolle behalten möchtest. Alles, was älter als die angegebene Anzahl von Tagen ist, wird gelöscht.

Klicke auf `Cloud-FX Trigger-Dokumente löschen`, um den Löschvorgang zu starten.