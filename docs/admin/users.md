---
layout: default
title: User-Liste
nav_exclude: true
parent: System
search_exclude: true
---

# User-Liste
{: .no_toc }

---

{: .intern-title }
> ☠️ Admin-Bereich ☠️
>
> Diese Seite ist für die System-Admins.

Die User-Liste zeigt alle Benutzer\*innen an, die ein Konto bei chuchipirat haben. Die Gesamtanzahl wird oberhalb der Tabelle angezeigt. Über das Suchfeld kannst du nach bestimmten Einträgen suchen.

## Übersicht

Die Tabelle enthält folgende Spalten:

- **Öffnen** — öffnet die Detailansicht
- **Supabase-ID** — eindeutige Kennung
- **Anzeigename**, **Vorname**, **Nachname**
- **E-Mail-Adresse**
- **Member-ID**

## Detailansicht

Klickst du auf das Öffnen-Symbol, siehst du das vollständige Profil mit drei Tabs:

### Profil

- **Anzeigename**, **Vorname**, **Nachname**
- **E-Mail-Adresse**
- **Supabase-ID**, **Firebase-UID**
- **Member-ID**
- **Mit dabei seit** — Registrierungsdatum
- **Rollen** — aktuelle Berechtigungen (z.B. basic, communityLeader, admin)

### Statistik

Zeigt Aktivitätsdaten der Benutzer\*in.

### Anlässe

Zeigt alle Anlässe, bei denen die Person mitgekocht hat. Nützlich, um die Event-UID für den [Support-User]({% link docs/admin/activate_support_user.md %}) herauszufinden.
{::comment}[[activate_support_user]]{:/comment}

## Berechtigungen anpassen

1. Öffne die Detailansicht und klicke auf `Berechtigung bearbeiten`.
2. Aktiviere oder deaktiviere die gewünschten Rollen über die Schalter:
   - **Basic** — Standardrolle (immer aktiv)
   - **Community-Leader\*in** — Zugriff auf Community-Leader-Funktionen
   - **Admin** — voller Systemzugriff
3. Klicke auf `Speichern`.

{: .note }
Darunterliegende Berechtigungen werden automatisch mit vergeben (z.B. Admin erhält automatisch auch Community-Leader).

{: .important }
Die neuen Berechtigungen werden erst aktiv, nachdem die Person sich erneut angemeldet hat.
