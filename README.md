# SHIZU — OSINT Intelligence Platform

Kostenlose, statische Browser-App für öffentliche und autorisierte OSINT-Prüfungen.

## Funktionen
- Domain/DNS: A, AAAA, MX, TXT, NS, CAA und DS über Cloudflare DNS-over-HTTPS
- IP-Intelligence: ungefähre öffentliche Netzwerk-/Geo-Metadaten über ipwho.is
- Discord Snowflake: lokale Berechnung des Account-Erstellungszeitpunkts
- E-Mail-Sicherheit: MX, SPF und DMARC der Domain (keine Konto- oder Passwortsuche)
- Public Address: öffentliche Geschäfte/Behörden über OpenStreetMap Nominatim
- Cyber Intelligence: CISA KEV und NVD CVE-Feed
- Username: Links zu öffentlichen Suchergebnissen
- Suchhistorie: lokal im Browser (localStorage)

## Lokal starten
Einfach `index.html` im Browser öffnen. Für Nominatim/Browser-API-Zugriffe kann ein lokaler HTTP-Server nötig sein.

## GitHub Pages
1. Repository Settings → Pages öffnen.
2. Unter Build and deployment als Source **GitHub Actions** wählen.
3. Den Workflow `.github/workflows/pages.yml` ausführen lassen.
4. Die veröffentlichte URL wird unter Settings → Pages angezeigt.

## Datenschutz und Grenzen
SHIZU ist eine statische Browser-App. Suchverläufe bleiben lokal im Browser. Es gibt kein Backend, keine Nutzerkonten und keine serverseitige Speicherung. Öffentliche API-Quellen können CORS, Rate-Limits oder Verfügbarkeitsgrenzen haben; dann zeigt SHIZU einen Fehler statt Daten zu erfinden.
Discord-IDs liefern keine privaten E-Mail-Adressen, Telefonnummern, IP-Adressen oder Passwörter. Es werden keine fremden Zugangsdaten gesammelt und kein heimlicher Gerätezugriff ermöglicht.

## Quellen
- Cloudflare DNS: https://developers.cloudflare.com/1.1.1.1/encryption/dns-over-https/
- ipwho.is: https://ipwho.is/
- OpenStreetMap Nominatim: https://operations.osmfoundation.org/policies/nominatim/
- CISA KEV: https://www.cisa.gov/known-exploited-vulnerabilities-catalog
- NVD: https://nvd.nist.gov/developers/vulnerabilities

## Lizenz
MIT
