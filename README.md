# MacMetadataCleaner

**Windows x64 · Version 1.3.2 · DP-Soft**

[English](#english) | [Italiano](#italiano)

## English

MacMetadataCleaner removes unwanted macOS metadata files from folders and drives on Windows. This repository distributes the compiled application and documentation only; application source code is not included.

### Download and run

1. Open this repository's **Releases** page.
2. Download **MacMetadataCleaner.exe** from the latest release's **Assets** section.
3. Run the executable. No installation or separate .NET runtime is required.

**Platform:** Windows desktop x64. The Store package declares Windows 10 build 19041 or later; certification-kit validation was performed on Windows 11. Other Windows versions have not been independently verified.

### Features

- Detects `.DS_Store` and valid AppleDouble metadata files beginning with `._`.
- Cleans `.Spotlight-V100` and `.fseventsd` service folders.
- Includes hidden and system entries without changing File Explorer settings.
- Displays file counts, total sizes and a detailed report before deletion.
- Supports selected folders, subfolders and entire drive roots.
- Offers optional `.Trash` / `.Trashes` cleanup, disabled by default.
- Follows the Windows light or dark app theme.
- Processes files locally; no account or internet connection is required.

### How to use

1. Click **Choose folder** and select a folder or drive.
2. Leave the Trash option unchecked unless you intend to delete its contents.
3. Click **Analyze folder** and review the results and notices.
4. Click **Confirm cleanup…**, then **Delete files** to authorize deletion.

> **Permanent deletion:** cleanup does not use the Recycle Bin. Optional Trash cleanup can delete discarded user documents, not just metadata. Changing the Trash option requires a new analysis.

The app does not follow symbolic links or junctions. Files changed or added after analysis are protected by cleanup checks. Empty service directories are removed individually. Access-denied entries are reported. Cleanup does not remove metadata embedded in photos or documents.

### Integrity and feedback

The release includes **SHA256.txt**. Verify the download in PowerShell with:

```powershell
Get-FileHash .\MacMetadataCleaner.exe -Algorithm SHA256
```

Compare the value with `SHA256.txt`. Report problems through this repository's **Issues**, if enabled. Include the app version and the error message, avoiding personal file paths or private data.

**Developer:** DP-Soft · **Copyright:** © 2026 DP-Soft.

No open-source license is granted by this repository. Third-party notices accompanying the binary describe the bundled .NET components. MacMetadataCleaner is an independent utility and is not affiliated with Apple or Microsoft.

## Italiano

MacMetadataCleaner rimuove i file di metadati macOS indesiderati da cartelle e unità su Windows. Questo repository distribuisce soltanto l'applicazione compilata e la documentazione; il codice sorgente dell'app non è incluso.

### Scaricare e avviare

1. Apri la pagina **Releases** di questo repository.
2. Scarica **MacMetadataCleaner.exe** dalla sezione **Assets** dell'ultima release.
3. Avvia l'eseguibile. Non occorrono installazione o un runtime .NET separato.

**Piattaforma:** Windows desktop x64. Il pacchetto Store dichiara Windows 10 build 19041 o successiva; la verifica con il kit di certificazione è stata eseguita su Windows 11. Le altre versioni di Windows non sono state verificate indipendentemente. L'interfaccia dell'app è in inglese.

### Funzionalità

- Riconosce `.DS_Store` e i file di metadati AppleDouble validi che iniziano con `._`.
- Pulisce le cartelle di servizio `.Spotlight-V100` e `.fseventsd`.
- Include elementi nascosti e di sistema senza cambiare le impostazioni di Esplora file.
- Mostra numero dei file, dimensioni totali e report dettagliato prima dell'eliminazione.
- Supporta cartelle selezionate, sottocartelle e radici di intere unità.
- Offre la pulizia facoltativa di `.Trash` / `.Trashes`, disattivata per impostazione predefinita.
- Segue il tema chiaro o scuro delle app di Windows.
- Elabora i file localmente; non richiede account o connessione Internet.

### Come usarla

1. Premi **Choose folder** e seleziona una cartella o un'unità.
2. Lascia disattivata l'opzione Trash se non vuoi eliminarne il contenuto.
3. Premi **Analyze folder** e controlla risultati e avvisi.
4. Premi **Confirm cleanup…**, poi **Delete files** per autorizzare l'eliminazione.

> **Eliminazione definitiva:** la pulizia non utilizza il Cestino. La pulizia facoltativa delle cartelle Trash può eliminare documenti cestinati, oltre ai metadati. Cambiare questa opzione richiede una nuova analisi.

L'app non segue collegamenti simbolici o junction. I controlli di pulizia proteggono i file modificati o aggiunti dopo l'analisi. Le directory di servizio vuote vengono rimosse singolarmente. Gli elementi non accessibili vengono segnalati. La pulizia non rimuove i metadati incorporati in foto o documenti.

### Integrità e segnalazioni

La release include **SHA256.txt**. Verifica il download in PowerShell:

```powershell
Get-FileHash .\MacMetadataCleaner.exe -Algorithm SHA256
```

Confronta il valore con `SHA256.txt`. Segnala eventuali problemi tramite **Issues** di questo repository, se abilitato, indicando versione ed errore senza includere percorsi personali o dati privati.

**Sviluppatore:** DP-Soft · **Copyright:** © 2026 DP-Soft.

Il repository non concede una licenza open source. Le informative di terze parti che accompagnano il binario descrivono i componenti .NET inclusi. MacMetadataCleaner è un'utilità indipendente, non affiliata ad Apple o Microsoft.
