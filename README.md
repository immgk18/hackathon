# Employee AccessGuard 360

A defensive, evidence-led investigation dashboard for CRIMEATHON'26 Case CR-26-047.

## Project focus
Investigate possible misuse of a BlueVault third-party storage key, using:
- **E05** — BlueVault access log (primary access evidence)
- **E02** — HelpDeskr audit log (supporting integration activity)
- **E09** — Risk register (known control risk)

The prototype distinguishes recorded activity from conclusions that still require verification. It does not claim that suspicious access proves data theft.

## Run locally
This is a static browser application. Open `index.html` in a modern browser, or serve the folder with any static web server.

## Import evidence
- E02: CSV
- E05: CSV
- E09: XLSX/XLS or CSV

Files are parsed in the browser and are not uploaded to an application server. The XLSX reader is loaded from the SheetJS CDN.

## Important limitations
- The initial dashboard figures are labelled demonstration case values.
- Timestamp and identity correlation is not yet implemented as a full forensic pipeline.
- BlueVault clock drift and missing IP values require careful interpretation.
- The dashboard is an investigation aid, not an automated incident verdict.
- Validate IP ownership, key ownership, approved permissions and vendor activity before containment.

## Track
DEFENSE — detect, investigate and recommend human-approved response.
