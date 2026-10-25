# Whiteboard + Document – Teams-app

Links staat je Microsoft Whiteboard, rechts een documentviewer die je kunt sluiten.
Is de viewer dicht, dan gebruikt het whiteboard de volle breedte. Rechts verschijnt
dan een lipje "Document" om de viewer weer te openen.

## Inhoud
- `app/index.html`: de app zelf. Dit bestand moet online staan op een https-adres.
- `teams-package/`: het Teams-pakket (manifest en iconen).

## Installeren in 4 stappen

1. **Zet `app/index.html` online** op een https-adres. Gratis opties zijn GitHub Pages
   of Azure Static Web Apps. Je IT-afdeling kan het ook op een eigen server zetten.
2. **Pas `teams-package/manifest.json` aan.** Vervang elke `JOUW-DOMEIN.example` door
   je echte domein, bijvoorbeeld `sandino.github.io`. Zet in `contentUrl` het volledige
   adres van de pagina. Vervang `*.sharepoint.com` eventueel door het SharePoint-domein
   van je organisatie, bijvoorbeeld `bedrijf.sharepoint.com`.
3. **Maak een zip** van de drie bestanden in `teams-package` (manifest.json, color.png,
   outline.png). Zet ze direct in de zip, niet in een map.
4. **Upload in Teams:** Apps, dan Apps beheren, dan Een app uploaden. Als uploaden
   geblokkeerd is, vraag je IT-beheerder de zip via het Teams-beheercentrum toe te staan.

## Gebruik
- Plak de link van je whiteboard (in Whiteboard: Delen, dan Link kopiëren).
- Klik op **Document tonen**, plak de link van een bestand en kies **Bekijken** of **Bewerken**.
- Sluiten kan met ✕, met de knop **Document verbergen** of met Esc.
- Sleep de scheidingslijn om de viewer breder of smaller te maken.
- De app onthoudt je whiteboard, document en paneelbreedte.

## Bekende beperkingen
- **Whiteboard laden:** Microsoft bepaalt of Whiteboard binnen een andere app mag laden.
  Werkt dat niet, dan toont de app een melding met een knop om het whiteboard apart te openen.
- **Bewerken:** bekijken werkt doorgaans goed. Bewerken binnen het paneel kan door je
  organisatie of door Microsoft geblokkeerd zijn. Gebruik dan de knop ↗ om het document
  in een nieuw venster te bewerken.
- **Deellinks** (korte links met `/:w:/` of `/:x:/`) laden soms alleen als bekijkweergave.
  Lukt bewerken niet, open het bestand in de browser en plak het adres uit de adresbalk.
