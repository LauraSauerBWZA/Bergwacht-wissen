# Bergwacht Zollernalb – Wissensplattform

Interne Eigenentwicklung einer geschützten Wissensplattform für die Bergwacht Zollernalb.

## Das Projekt

Eine browserbasierte Plattform, auf der berechtigte Mitglieder Einsatzwissen, Dokumente und Videos abrufen können. Nicht öffentlich. Vollständiges Zugriffskontrollsystem auf eigenem Server.

**Stack:** Node.js + Express · SQLite · Eigener VPS

## Projektübersicht

Öffne [`bergwacht-projekt.html`](bergwacht-projekt.html) im Browser für eine **interaktive, klickbare Übersicht** der Architektur, Rollen, des Datenmodells und der Sicherheitskonzepte.

(Einfach herunterladen und lokal im Browser öffnen.)

---

## Schnelle Fakten

| Aspekt | Details |
|--------|---------|
| **Zugang** | Nur für aktive Bergwacht-Mitglieder |
| **Rollen** | Admin (verwaltet), Mitglied (liest) |
| **Inhalte** | Themen, Artikel, Dokumente, Videos |
| **Hosting** | Eigener VPS (keine Abhängigkeit von Firebase/GitHub Pages) |
| **Sicherheit** | HTTPS, Passwort-Hashing, Rechteprüfung auf jeder Route |
| **Wartbarkeit** | Einfach genug für ehrenamtliche Weiterentwicklung |

---

## Architektur (vereinfacht)

```
Browser (Client)
    ↓ (Login, Anfragen)
Node.js + Express (Server)
    ↓ (Prüfung, API)
SQLite Datenbank
    ↓ (Speicherung)
/uploads (Dateien & Videos)
```

---

## Entwicklung

Dieses Projekt wird mit Unterstützung von Claude Code entwickelt.

**Stand:** Mai 2026  
**Lizenz:** UNLICENSED – Internes Projekt der Bergwacht Zollernalb
