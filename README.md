# Schrittplaner

Mehrschritt-Zeitplaner im Browser: beliebig viele Schritte mit Dauer und Typ (aktiv/passiv),
Vorwärtsrechnung („Start um …, wann bin ich fertig?") und Rückwärtsrechnung („Fertig um …,
wann muss ich anfangen?"). Zeigt jeden Zwischenschritt im Zeitplan an.

Basis-Vorlagen oben: Waschmaschine (Startzeitvorwahl in ganzen Stunden), Roggen-Sauerteig,
Pfannkuchen, weitere — Zeiten, Spielräume und Notizen anpassbar. Zeitplan als `.ics`-Datei
exportierbar (z. B. Import in Google Kalender).

Reines HTML/CSS/JS, keine Abhängigkeiten, läuft komplett im Browser. Einstellungen und
Vorlagen liegen in `localStorage`.

## Nutzen

Als Webseite öffnen unter der GitHub-Pages-URL dieses Repos (Settings → Pages), oder lokal
`index.html` im Browser öffnen.

## Kalender-Export (.ics)

1. Zeitplan berechnen lassen
2. **Kalenderdatei (.ics) herunterladen** klicken
3. Google Kalender: Einstellungen → Importieren und Exportieren → Importieren → Datei wählen

Jeder Schritt wird ein eigener Termin. Bei Spielräumen (z. B. 2–5 Std) gilt das volle Zeitfenster.

## Als App aufs Handy installieren

Über die GitHub-Pages-URL (nicht als lokale Datei) öffnen, dann:

- **iPhone (Safari):** Teilen-Symbol → „Zum Home-Bildschirm"
- **Android (Chrome):** Menü (⋮) → „App installieren" / „Zum Startbildschirm hinzufügen"

Dank `manifest.json` öffnet sich die App danach im eigenen Fenster, ohne Browser-Leiste.
