# MeteoCasarano Lab

Repository pubblico di distribuzione di **MeteoCasarano Lab** per Windows.

MeteoCasarano Lab è un'applicazione desktop dedicata all'analisi di temporali,
fenomeni intensi e instabilità atmosferica nel Basso Salento.

## Download

Le versioni ufficiali vengono pubblicate esclusivamente nella sezione
**Releases** di questo repository.

Sono previsti:

- installer Windows NSIS (`.exe`);
- installer Windows MSI (`.msi`);
- file `SHA256SUMS.txt` per verificare l'integrità dei download.

## Verifica SHA-256

Dopo avere scaricato un installer, in PowerShell è possibile calcolarne
l'impronta con:

```powershell
Get-FileHash "MeteoCasarano Lab_0.1.0_x64-setup.exe" -Algorithm SHA256
```

Il valore deve coincidere esattamente con quello pubblicato insieme alla
release.

## Firma digitale Windows

Gli installer di MeteoCasarano Lab sono attualmente distribuiti senza un
certificato commerciale di Code Signing.

Windows SmartScreen può quindi mostrare un avviso con indicazione
**Autore sconosciuto**, soprattutto per versioni nuove o poco diffuse.

Questo avviso, da solo, non significa che il programma sia stato identificato
come malware.

Per ridurre il rischio di scaricare copie alterate:

1. scaricare MeteoCasarano Lab esclusivamente da questo repository;
2. verificare sempre il valore SHA-256 pubblicato nella release.

## Componenti di terze parti

Gli installer includono gli avvisi e i materiali relativi alle dipendenze
software di terze parti utilizzate dalla build distribuita, compresi i
materiali richiesti per i componenti soggetti a Mozilla Public License 2.0.

## Codice sorgente

Questo repository è destinato esclusivamente alla distribuzione delle build.

La pubblicazione degli installer in questo repository non implica la
pubblicazione del codice sorgente di MeteoCasarano Lab e non concede,
di per sé, diritti sul software oltre a quelli eventualmente indicati
separatamente.

## Stato del progetto

MeteoCasarano Lab è un progetto amatoriale e sperimentale.

Le informazioni meteorologiche prodotte dall'applicazione non costituiscono
un servizio ufficiale di allerta o protezione civile.
