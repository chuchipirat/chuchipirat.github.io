---
layout: default
title: Mail-Konsole
permalink: docs/admin/mailconsole
nav_exclude: true
parent: System
search_exclude: true
---
# Mail-Konsole
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
> Diese Seite ist für die System-Admins.

Über die Mail-Konsole kannst du E-Mails im Newsletter-Stil an Benutzer\*innen versenden. Rechts neben dem Editor wird eine Live-Vorschau der Nachricht angezeigt.

![Mailkonsole](/docs/admin/images/mailconsole.png)
## Empfänger

Wähle aus, an wen die Nachricht gesendet werden soll. Es gibt drei Optionen:

- **E-Mail-Adresse:** direkte Eingabe einer oder mehrerer E-Mail-Adressen
- **User-UID:** Eingabe einer oder mehrerer User-UIDs
- **Rolle:** Auswahl einer Rolle aus dem Dropdown (z.B. alle Community-Leader)

{: .note }
Mehrere Werte trennst du mit einem Semikolon `;`.

## Editor

Wähle zuerst ein **Mail Template** aus dem Dropdown (oder «Leere Vorlage» für eine freie Nachricht). Fülle dann die folgenden Felder aus:

- **Betreff:** Betreffzeile der E-Mail
- **Titel:** grosse Überschrift im Newsletter (optional). Lässt du das Feld leer, beginnt die Mail direkt mit dem Text.
- **Untertitel:** kurzer Untertitel (optional)
- **E-Mail Nachricht:** der Haupttext mit Rich-Text-Editor (fett, kursiv, Listen, Links etc.)
- **Button-Beschriftung:** Text des Buttons (optional)
- **Link für Button (Ziel):** URL, auf die der Button verlinkt (optional)
- **Abmelde-Footer anhängen:** Abmeldelink am Ende der Mail, siehe unten. Standardmässig aktiv.

## Abmelde-Footer

Newsletter enthalten am Ende einen Link, über den sich Nutzer\*innen abmelden können. Wer sich abgemeldet hat, bekommt keine Mails mehr aus der Mail-Konsole.

Für eine persönliche Nachricht an eine einzelne Person passt dieser Hinweis nicht. Deshalb kannst du den Footer mit der Checkbox **Abmelde-Footer anhängen** ausschalten. Die Vorschau rechts zeigt dir sofort, ob der Hinweis in der Mail steht.

- **Empfänger E-Mail-Adresse oder User-UID:** Du kannst den Footer ausschalten.
- **Empfänger Rolle:** Der Footer ist immer aktiv, die Checkbox ist gesperrt. So geht ein Newsletter nie ohne Abmeldelink an viele Personen.

{: .important }
Ohne Footer wird die Mail auch an Personen gesendet, die sich vom Newsletter abgemeldet haben. Das ist für Direktnachrichten gewollt (z.B. eine Antwort auf eine Anfrage), aber schalte den Footer nur aus, wenn die Mail wirklich eine persönliche Nachricht ist.

{: .highlight }
Wechselst du die Einstellung, musst du danach erneut eine Test Mail senden. Erst dann wird der Button zum Versenden wieder aktiv.

## Versenden

1. **Vorschau prüfen:** kontrolliere die Nachricht in der Live-Vorschau rechts.
2. **Test Mail senden:** klicke auf `Test Mail senden`, um eine Testmail an deine eigene E-Mail-Adresse zu erhalten.
3. **Mail versenden:** wenn alles passt, klicke auf `Mail an X Empfänger senden`. Der Button zeigt die Anzahl der Empfänger\*innen an.

Über `Entwurf löschen` kannst du alle Eingaben zurücksetzen und von vorne beginnen.
