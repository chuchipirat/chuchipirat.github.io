---
layout: default
title: Kosten & Transparenz
parent: FAQ
nav_exclude: false
nav_order: 10
has_children: false
---
# Kosten & Transparenz
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

chuchipirat ist kostenlos nutzbar – und das soll so bleiben. Damit das möglich ist, entstehen im Hintergrund laufende Kosten, die durch Spenden gedeckt werden. Diese Seite erklärt offen und ehrlich, wofür das Geld verwendet wird.

---

## Wer steckt hinter chuchipirat?

chuchipirat wird vom gleichnamigen Verein betrieben und ausschliesslich durch Freiwillige entwickelt und betreut. Es gibt keine bezahlten Mitarbeitenden. Alle, die an der App arbeiten, tun dies in ihrer Freizeit – neben Beruf, Studium und anderen Verpflichtungen.

---

## Wofür entstehen Kosten?

Auch eine kostenlose App ist nicht gratis. Im Folgenden sind alle wiederkehrenden Kostenpositionen aufgeführt, mit einem ungefähren Jahresbetrag.

### 🖥️ Server-Hosting

Die App läuft auf einem gemieteten Server bei [Hetzner](https://www.hetzner.com/), einem deutschen Anbieter mit Rechenzentren in Deutschland und Finnland. Auf diesem Server laufen die Webapplikation, die Datenbank sowie alle weiteren Dienste.

| Posten | Kosten |
|---|---|
| Hetzner CX33 (Produktivumgebung) | ~ CHF 240 / Jahr |

Ein eigener Server ist notwendig, damit die Daten in Europa gespeichert werden und wir die volle Kontrolle über die Infrastruktur behalten.

---

### 🌐 Domain

Damit chuchipirat unter `chuchipirat.ch` erreichbar ist, muss die Domain jährlich erneuert werden.

| Posten | Kosten |
|---|---|
| Domain `chuchipirat.ch` | ~ CHF 30 / Jahr |

---

### 📬 E-Mail-Hosting

Für offizielle Vereins-E-Mails (z.B. `hallo@chuchipirat.ch`) wird ein Postfach bei einem E-Mail-Anbieter gemietet.

| Posten | Kosten |
|---|---|
| E-Mail-Postfach (Vereinsadresse) | ~ CHF 40 / Jahr |

---

### 📨 E-Mail-Versand (transaktional)

Die App verschickt automatisch E-Mails – etwa wenn du dein Passwort zurücksetzt, eine Einladung erhältst oder eine Bestätigung bekommst. Für diesen Massenversand wird ein spezialisierter Dienst ([Brevo](https://www.brevo.com/)) verwendet, da normales E-Mail-Hosting dafür nicht ausgelegt ist.

| Posten | Kosten |
|---|---|
| Brevo (Free Tier, bis 300 Mails/Tag) | CHF 0 / Jahr |

Aktuell sind wir im kostenlosen Kontingent. Sollte chuchipirat stark wachsen, kann hier künftig ein kostenpflichtiger Plan notwendig werden.

---

### 🔒 SSL-Zertifikat

Damit alle Verbindungen zur App verschlüsselt sind (erkennbar am `https://` in der Adresszeile), wird ein SSL-Zertifikat benötigt. Wir nutzen [Let's Encrypt](https://letsencrypt.org/), einen gemeinnützigen Anbieter, der Zertifikate kostenlos ausstellt.

| Posten | Kosten |
|---|---|
| SSL-Zertifikat (Let's Encrypt) | CHF 0 / Jahr |

---

### 💾 Backup-Speicher

Regelmässige Datensicherungen sind essenziell. Die Backups werden auf einem separaten, externen Speicher abgelegt – losgelöst vom Hauptserver. So sind die Daten auch dann sicher, wenn der Server selbst ein Problem hat.

| Posten | Kosten |
|---|---|
| Offsite-Backup-Speicher | ~ CHF 50 / Jahr |

---

### 🐛 Fehlerüberwachung (Error Monitoring)

Um Fehler in der App schnell zu erkennen und zu beheben, wird [Sentry](https://sentry.io/) eingesetzt. Der Dienst meldet uns automatisch, wenn etwas in der App nicht wie erwartet funktioniert.

| Posten | Kosten |
|---|---|
| Sentry (Free Tier) | CHF 0 / Jahr |

Auch hier gilt: Wir bewegen uns aktuell im kostenlosen Kontingent.

---

### 📊 Nutzungsstatistiken (Analytics)

Um zu verstehen, wie chuchipirat genutzt wird, setzen wir [Umami](https://umami.is/) ein – eine datenschutzfreundliche Alternative zu Google Analytics. Umami läuft direkt auf unserem eigenen Server, es werden keine Daten an Dritte weitergegeben und es ist kein Cookie-Banner nötig.

| Posten | Kosten |
|---|---|
| Umami (self-hosted, auf eigenem Server) | CHF 0 / Jahr |

---

### 🤝 Vereinskosten

Der Verein chuchipirat hat auch organisatorische Kosten. Dazu gehören gelegentliche Sitzungen (z.B. Jahresversammlung) sowie kleine Formen der Wertschätzung für die Freiwilligen, die das Projekt am Laufen halten.

| Posten | Kosten |
|---|---|
| Vereinssitzungen, Spesen, Wertschätzung | ~ CHF 100–200 / Jahr |

---

## Zusammenfassung

| Kostenkategorie | Geschätzte Jahreskosten |
|---|---|
| Server-Hosting | ~ CHF 240 |
| Domain | ~ CHF 30 |
| E-Mail-Hosting | ~ CHF 40 |
| E-Mail-Versand (Brevo) | CHF 0 |
| SSL-Zertifikat | CHF 0 |
| Backup-Speicher | ~ CHF 50 |
| Fehlerüberwachung (Sentry) | CHF 0 |
| Analytics (Umami) | CHF 0 |
| Vereinskosten | ~ CHF 150 |
| **Total** | **~ CHF 510 / Jahr** |

Das Spendenbudget orientiert sich an diesen realen Kosten. Überschüsse werden nicht ausgeschüttet, sondern für künftige Betriebskosten zurückgelegt.

---

## Was passiert, wenn nicht genug gespendet wird?

chuchipirat wird nicht von heute auf morgen abgeschaltet – aber ohne ausreichende Deckung der laufenden Kosten müssten wir früher oder später Dienste reduzieren oder die App auf einen günstigeren, möglicherweise weniger zuverlässigen Betrieb umstellen. Im schlimmsten Fall wäre ein Weiterbetrieb langfristig nicht möglich.

---

## Wie kann ich helfen?

Auf der [Spendenseite](../spenden) findest du alle Möglichkeiten, das Projekt zu unterstützen. Jeder Betrag hilft – auch eine kleine Spende trägt dazu bei, dass chuchipirat für alle Jungwacht-, Blauring, Pfadi- und Jungscharen kostenlos nutzbar bleibt.

{: .note }
Hast du Fragen zur Verwendung der Spendengelder? Schreib uns unter [info@chuchipirat.ch](mailto:info@chuchipirat.ch).