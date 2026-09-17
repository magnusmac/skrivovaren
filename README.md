# Skrivövaren

Ett skrivträningsverktyg för svensk skola. Läraren skriver en bokstav för hand
på skärmen, och verktyget spelar upp exakt hur den skrevs — i vilken ordning
och åt vilket håll dragen gick. Eleverna får se själva rörelsen, inte bara den
färdiga bokstaven.

**Öppna verktyget:** https://magnusmac.github.io/skrivovaren/

## Vad det gör

- **Spela upp** ritar om bokstaven precis som den skrevs, med en pennmarkör som
  visar var pennan är. Paus mitt i draget för att peka på något.
- **Bokstavsbibliotek** sparar din handstil under ett namn. Spela upp den igen
  nästa lektion, eller exportera biblioteket och dela det med en kollega.
- **Spårläge** gör din egen handstil till en blek förlaga som eleven skriver
  ovanpå — inte ett typsnitt, utan din bokstav.
- **Svensk linjatur**: linjerat, punktlinjer, rutat 5 och 10 mm, skrivlinjer,
  fyrlinjesystem, Montessori, sneda hjälplinjer och kollegieblock.
- **Tavelläge** förstorar alla kontroller för smartboard, tillsammans med
  helskärm och ett fokusläge som döljer panelerna.
- Spara som bild, skriv ut eller spara som PDF.

## Så använder du det

Skriv en bokstav för hand med mus, pekskärm eller penna. Tryck **Spela upp**.
Ge bokstaven ett namn och tryck **Spara det jag skrivit** så finns den kvar.

## Teknik

En enda fristående HTML-fil. Ingen build, inga beroenden, inga API-nycklar,
ingen server. All CSS och JavaScript ligger i filen, så den fungerar offline —
ladda ner den och dubbelklicka, eller öppna länken ovan.

Ritytan är fyra staplade canvaslager: papper med linjatur, förlaga, bläck och
en överlagring för pennmarkör och dragordning. Varje penndrag spelas in som
punkter med tidsstämpel, vilket är det som gör uppspelningen möjlig.

Anpassat för smartboard: ett finger i taget, så att en handlove som landar mitt
i ett drag inte kapar det, och penna tar över från finger.

## Integritet

Ingenting lämnar datorn. Inställningar och sparade bokstäver ligger i
webbläsarens lokala lagring. Ingen elevdata samlas in, ingen inloggning behövs,
ingenting skickas till någon server.

## Upphov

Skapad av Magnus MacNeil.
