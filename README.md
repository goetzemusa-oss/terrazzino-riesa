# Shelby's Burger & Vino — CMS Setup

## Struktur
```
public/
  index.html          ← Die eigentliche Website
  admin/
    index.html        ← Decap CMS Admin-UI
    config.yml        ← Definiert was der Besitzer bearbeiten kann
  images/             ← Hochgeladene Fotos landen hier
netlify.toml          ← Netlify-Konfiguration
ANLEITUNG.html        ← Anleitung für den Besitzer (ausdrucken/schicken)
```

## Setup in 5 Schritten

### 1. GitHub Repository erstellen
- Neues (privates) Repository auf github.com anlegen
- Alle Dateien hochladen

### 2. Netlify mit GitHub verbinden
- netlify.com → "Add new site" → "Import from Git"
- GitHub-Repo auswählen
- Build-Einstellungen: Publish directory = `public`
- Deploy starten

### 3. Netlify Identity aktivieren
- Site settings → Identity → Enable Identity
- Registration: "Invite only" auswählen
- Git Gateway aktivieren (unter Identity → Services)

### 4. Besitzer einladen
- Identity → Invite users → E-Mail des Besitzers eingeben
- Er bekommt eine Einladungs-E-Mail und setzt sein Passwort

### 5. Anleitung übergeben
- ANLEITUNG.html im Browser öffnen und als PDF drucken
- Oder per E-Mail als HTML-Datei schicken

## Backend-URL für den Besitzer
https://[deine-netlify-domain]/admin

## Was der Besitzer bearbeiten kann
- ✅ Öffnungszeiten (alle Wochentage)
- ✅ Speisekarte (Burger, Weine, Cocktails, Snacks)
- ✅ Galerie (bis zu 6 Fotos)
- ✅ Kontaktdaten (Telefon, E-Mail)
- ❌ Design, Farben, Layout (geschützt)
