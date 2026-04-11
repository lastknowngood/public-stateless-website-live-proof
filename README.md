# public-stateless-website-live-proof

Temporarer test-only Live-Proof fuer den bisher validierten einfachsten
Projektpfad auf `coolify-01`.

## Charakter

- `lifecycle.mode: live`
- oeffentlich
- stateless
- Coolify `dockerfile`
- keine Datenbank
- keine Runtime-Secrets
- test-only Proof, Cleanup abgeschlossen

## Zweck

Dieses Repo ist kein kanonisches Beispiel, sondern der ausgefuehrte reale
Beweisfall dafuer, dass aus dem validierten stateless Website-Pfad auf
`coolify-01` wirklich eine laufende Coolify-App entstehen kann.

Es ist **nicht**:

- ein dauerhaftes Live-Projekt
- ein Host-Runbook
- die wiederverwendbare kanonische Vorlage

## Aktueller Zustand

- historischer Proof: erfolgreich
- Cleanup: abgeschlossen
- retained Runtime: nein
- retained DNS: nein
- verwendete historische Testdomain:
  - `agent-drill.dental-school.education`

Der fruehere blockierte Tailnet-Git-Quellenpfad wurde spaeter durch die
GitHub-Quelle ersetzt und der oeffentliche HTTPS-Proof erfolgreich
abgeschlossen. Die detaillierte Chronologie und Cleanup-Evidence bleibt im
Host-Repo unter `docs/provisioning-log/`.

## Lokale Entwicklung

- statische Dateien und `Dockerfile` bleiben klein
- vor einem erneuten Proof den Contract und Host-Runbook-Stand im Host-Repo
  pruefen
- wenn Docker lokal verfuegbar ist, vor Deploy einen kleinen Image-Smoke fahren

## Laufzeitverhalten

- statische Nginx-Seite
- sichtbarer Proof-Marker
- `robots.txt`
- HTML-`noindex`
- `X-Robots-Tag`
- keine Datenbank
- keine Runtime-Secrets

## Proof-Status

- privater Readiness-Pfad: erfolgreich
- oeffentlicher HTTPS-Proof: erfolgreich
- Cleanup: erfolgreich

## Reale Evidence

- Host-Chronologie:
  - `docs/provisioning-log/2026-03.md`
- historischer FQDN:
  - `agent-drill.dental-school.education`
- dieses Repo bleibt historische Remote-Wahrheit fuer den ausgefuehrten
  stateless Public-Proof, nicht der Steady State eines laufenden Dienstes
