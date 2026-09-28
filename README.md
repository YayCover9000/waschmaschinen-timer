# Schrittplaner

Mehrschritt-Zeitplaner im Browser: beliebig viele Schritte mit Dauer und Typ (aktiv/passiv),
Vorwärtsrechnung („Start um …, wann bin ich fertig?") und Rückwärtsrechnung („Fertig um …,
wann muss ich anfangen?"). Zeigt jeden Zwischenschritt im Zeitplan an.

Basis-Vorlagen oben: Waschmaschine (Startzeitvorwahl in ganzen Stunden), Roggen-Sauerteig,
Pfannkuchen, weitere — Zeiten, Spielräume und Notizen anpassbar. Zeitplan exportierbar
nach Google Kalender (OAuth) oder als `.ics`-Datei.

Reines HTML/CSS/JS, keine Abhängigkeiten, läuft komplett im Browser. Einstellungen und
Vorlagen liegen in `localStorage`.

## Google Kalender (einmalige Einrichtung)

1. [Google Cloud Console](https://console.cloud.google.com/) → Projekt anlegen oder wählen
2. **Google Calendar API** aktivieren
3. **OAuth-Zustimmungsbildschirm** konfigurieren (Extern, Testnutzer: deine Google-Adresse)
4. **Anmeldedaten** → OAuth-Client-ID → **Webanwendung**
5. **Autorisierte JavaScript-Ursprünge:** `https://yaycover9000.github.io` (plus `http://localhost:PORT` für lokale Tests)
6. Client-ID in der App unter **Einstellungen** eintragen
7. **In Google Kalender übernehmen** klicken, einmalig anmelden — jeder Schritt wird ein Termin

Alternativ ohne OAuth: **Als .ics-Datei** → Google Kalender → Einstellungen → Importieren und Exportieren → Importieren.

## Nutzen

Als Webseite öffnen unter der GitHub-Pages-URL dieses Repos (Settings → Pages), oder lokal
`index.html` im Browser öffnen.

## Als App aufs Handy installieren

Über die GitHub-Pages-URL (nicht als lokale Datei) öffnen, dann:

- **iPhone (Safari):** Teilen-Symbol → „Zum Home-Bildschirm"
- **Android (Chrome):** Menü (⋮) → „App installieren" / „Zum Startbildschirm hinzufügen"

Dank `manifest.json` öffnet sich die App danach im eigenen Fenster, ohne Browser-Leiste.
