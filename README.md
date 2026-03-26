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
- test-only und standardmaessig fuer spaeteres Cleanup gedacht

## Zweck

Dieses Repo ist kein kanonisches Beispiel, sondern ein realer temporarer
Beweisfall dafuer, dass aus dem validierten stateless Website-Pfad auf
`coolify-01` wirklich eine laufende Coolify-App entstehen kann.

Es ist **nicht**:

- ein dauerhaftes Live-Projekt
- ein Host-Runbook
- die wiederverwendbare kanonische Vorlage

## Aktueller Runtime-Status

- Repo-/Contract-Ebene: sauber
- Coolify-Runtime-Ebene: aktuell blockiert

Der erste echte Deploy-Versuch gegen `coolify-01` ist nicht an Docker, nicht am
Dockerfile und nicht an stateless Defaults gescheitert, sondern bereits an der
Git-Quelle:

- verwendete Test-Quelle:
  `https://rtx5090.tail278d58.ts.net/public-stateless-website-live-proof.git`
- Befund im Coolify-Build-Helfer:
  `Could not resolve host: rtx5090.tail278d58.ts.net`

Das Repo bleibt damit ein valider test-only Beweisfall fuer den Git-basierten
Pfad, aber noch kein erfolgreich runtime-validiertes Live-Projekt.
