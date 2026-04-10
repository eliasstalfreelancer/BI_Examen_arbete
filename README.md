# BI_Examen_arbete 
## fråge sättning om Behovsanalys. (Fick Betyg: G)

Introduktion
Du är BI-analytiker på ett företag som vill bli mer datadrivet. Idag tar rapporter lång tid att få fram och olika personer räknar på olika sätt, vilket leder till olika “versioner av sanningen”. Målet är att skapa en Self-Service BI-lösning där rätt målgrupper får rätt insikter, i rätt format.

I den här uppgiften ska du göra en behovsanalys: vilka målgrupper som finns, vilka beslut de behöver stöd för och vilka typer av insikter och verktyg som är mest lämpliga.

Företaget vill få bättre kontroll på:
hur försäljning och lönsamhet utvecklas över tid
vilka regioner/butiker som presterar bäst/sämst
vilka produktkategorier som driver intäkter och marginal
skillnader mellan kundsegment (t.ex. privat/SMB/företag)

Ledningen vill att detta ska lösas på ett standardiserat sätt så att organisationen kan arbeta mer enhetligt med data.

Du behöver inte bygga något i Power BI i denna uppgift.

Case: Nordic Retail
Du jobbar på Nordic Retail, ett företag som säljer produkter i Norden via både fysiska butiker och partners.

Om företaget (bakgrund)

Nordic Retail är en handelsaktör som säljer konsumentprodukter inom Clothing, Electronics, Home och Sports. Företaget har verksamhet i Sverige, Norge och Danmark och kombinerar egna butiker, outlets och partner-butiker (totalt ca 45 försäljningsställen).

Kunderna består av både privatkunder och företagskunder, uppdelat i segmenten Consumer, SMB (small & medium-sized buisnnesses) och Enterprise. Sortimentet omfattar cirka 250 produkter från flera varumärken, organiserat i 4 kategorier och 12 underkategorier.

Företaget har idag många rapporter som tas fram manuellt. Olika team räknar på olika sätt, vilket skapar “olika versioner av sanningen”. Ledningen vill därför standardisera hur nyckeltal definieras och följas upp – så att samma frågor alltid ger samma svar.

Beställarbrief (”mejl från chefen”)

Från: Försäljningschef / COO
 Till: BI-analytiker (du)

Vi behöver bättre kontroll på försäljning och lönsamhet i vår verksamhet i Norden. Idag tar det för lång tid att få svar och vi får ofta olika siffror beroende på vem som räknar.

Jag vill att du gör en behovsanalys: vilka målgrupper vi ska bygga för, vilka beslut de behöver ta, och vilka KPI:er, filter och nivåer (grain) som krävs för att rapporteringen ska bli användbar i vardagen.

Viktigt: vi vill kunna jämföra länder/regioner/butiker, se vilka kategorier/subkategorier som driver resultat, och kunna förstå skillnader mellan kundsegment.

Du behöver inte bygga något i Power BI i den här uppgiften – men din specifikation ska vara så tydlig att någon kan bygga rapporten efter den.


Till dig som elev (hur du ska tänka)

Målet är inte “så många KPI:er som möjligt”, utan rätt KPI:er för rätt beslut – och att de går att definiera tydligt.
När du väljer KPI:er:
Undvik fluff som “bra försäljning”. Skriv hellre: Nettoomsättning (efter rabatt), Bruttovinst, Bruttomarginal %, Antal orderrader/ordrar, Snittordervärde.
Skriv 1 mening definition per KPI: vad ingår/inte ingår (t.ex. “efter rabatt”, “per order” vs “per orderrad”).
När du väljer filter/grain:
Tänk “vad behöver användaren klicka på för att förstå varför siffran är som den är?”
Exempel på vanliga dimensioner här: datum, land/region, butik, kategori/subkategori, produkt, kundsegment.
Exempel grain: “per dag och butik”, eller “per månad och kategori".


Målgrupper:
Du ska utgå från följande målgrupper (du får lägga till fler om du vill, men minst tre måste användas):
Ledning (Executive): vill ha överblick, trend och KPI:er för beslut.
Regionchef: vill jämföra regioner/butiker och hitta avvikelser.
Butikschef / Operations: vill följa daglig/veckovis försäljning och top/bottom-produkter.
Kategoriansvarig: vill se vilka produkter/kategorier som driver lönsamhet och volym.

Data (översikt)
I senare moment i kursen kommer du få ett datalagerutdrag som innehåller:
försäljningstransaktioner (datum, produkt, kund, butik, antal, pris, rabatt)
produkter (kategori, subkategori, varumärke, standardkostnad, listpris)
kunder (segment, stad/region/land)
butiker (stad/region/land + ev. lat/long)
Du behöver inte kunna exakta kolumnnamn i den här uppgiften – fokusera på vilka insikter som går att få ut.

Din uppgift (för IG/G)
Du ska skriva en behovsanalys som är kort, tydlig och användbar.

1) Välj målgrupper (minst 3)
Välj minst tre målgrupper från listan ovan.

2) Behov per målgrupp
För varje målgrupp ska du beskriva:
Affärsfrågor (3–5 st) - Formulera 3–5 frågor målgruppen vill kunna besvara (tänk: frågor som leder till beslut). Ex: Vilka kategorier driver mest profit den här månaden – och skiljer det sig mellan länder?
KPI:er (3–6 st) - Lista 3–6 KPI:er som stödjer frågorna. - För varje KPI: skriv en kort definition (1 mening) så att det är tydligt vad den betyder.
KPI:er ska vara mätbara och tydligt kopplade till affärsfrågorna (undvik vaga KPI:er som “bra försäljning”) Ex: Nettoomsättning: “Summa försäljning efter rabatt, exkl. moms".
Filter/slicers (2–4 st) - Vilka filter behöver målgruppen kunna använda för att analysera datan? - Exempel: datum, region, butik, kategori, segment, varumärke.

3) Verktygsval (SSBI)
Svara kort på följande:
Varför är Power BI ett bra val för detta case? (max 5–8 rader)
När räcker Excel/PowerPivot, och när blir det olämpligt? (max 5–8 rader)
Om rapporterna ska delas i organisationen: hur skulle du leverera detta i praktiken? (t.ex. Power BI Service, export/PDF, åtkomst/behörighet på en övergripande nivå – max 5–8 rader)
Fokus här är resonemang kring lämpliga verktyg för rätt målgrupp, inte licensdetaljer.

#  Upgift 2
## Fråge sättning om Dashboard. (Fick Betyg: G)
Introduktion
Du är BI-analytiker på ett företag som vill bli mer datadrivet. Idag tar rapporter lång tid att få fram och olika personer räknar på olika sätt, vilket leder till olika “versioner av sanningen”. Målet är att skapa en Self-Service BI-lösning där rätt målgrupper får rätt insikter, i rätt format.

I den här uppgiften ska du göra en behovsanalys: vilka målgrupper som finns, vilka beslut de behöver stöd för och vilka typer av insikter och verktyg som är mest lämpliga.

Företaget vill få bättre kontroll på:
hur försäljning och lönsamhet utvecklas över tid
vilka regioner/butiker som presterar bäst/sämst
vilka produktkategorier som driver intäkter och marginal
skillnader mellan kundsegment (t.ex. privat/SMB/företag)

Ledningen vill att detta ska lösas på ett standardiserat sätt så att organisationen kan arbeta mer enhetligt med data.

Du behöver inte bygga något i Power BI i denna uppgift.

Case: Nordic Retail
Du jobbar på Nordic Retail, ett företag som säljer produkter i Norden via både fysiska butiker och partners.

Om företaget (bakgrund)

Nordic Retail är en handelsaktör som säljer konsumentprodukter inom Clothing, Electronics, Home och Sports. Företaget har verksamhet i Sverige, Norge och Danmark och kombinerar egna butiker, outlets och partner-butiker (totalt ca 45 försäljningsställen).

Kunderna består av både privatkunder och företagskunder, uppdelat i segmenten Consumer, SMB (small & medium-sized buisnnesses) och Enterprise. Sortimentet omfattar cirka 250 produkter från flera varumärken, organiserat i 4 kategorier och 12 underkategorier.

Företaget har idag många rapporter som tas fram manuellt. Olika team räknar på olika sätt, vilket skapar “olika versioner av sanningen”. Ledningen vill därför standardisera hur nyckeltal definieras och följas upp – så att samma frågor alltid ger samma svar.

Beställarbrief (”mejl från chefen”)

Från: Försäljningschef / COO
 Till: BI-analytiker (du)

Vi behöver bättre kontroll på försäljning och lönsamhet i vår verksamhet i Norden. Idag tar det för lång tid att få svar och vi får ofta olika siffror beroende på vem som räknar.

Jag vill att du gör en behovsanalys: vilka målgrupper vi ska bygga för, vilka beslut de behöver ta, och vilka KPI:er, filter och nivåer (grain) som krävs för att rapporteringen ska bli användbar i vardagen.

Viktigt: vi vill kunna jämföra länder/regioner/butiker, se vilka kategorier/subkategorier som driver resultat, och kunna förstå skillnader mellan kundsegment.

Du behöver inte bygga något i Power BI i den här uppgiften – men din specifikation ska vara så tydlig att någon kan bygga rapporten efter den.


Till dig som elev (hur du ska tänka)

Målet är inte “så många KPI:er som möjligt”, utan rätt KPI:er för rätt beslut – och att de går att definiera tydligt.
När du väljer KPI:er:
Undvik fluff som “bra försäljning”. Skriv hellre: Nettoomsättning (efter rabatt), Bruttovinst, Bruttomarginal %, Antal orderrader/ordrar, Snittordervärde.
Skriv 1 mening definition per KPI: vad ingår/inte ingår (t.ex. “efter rabatt”, “per order” vs “per orderrad”).
När du väljer filter/grain:
Tänk “vad behöver användaren klicka på för att förstå varför siffran är som den är?”
Exempel på vanliga dimensioner här: datum, land/region, butik, kategori/subkategori, produkt, kundsegment.
Exempel grain: “per dag och butik”, eller “per månad och kategori".


Målgrupper:
Du ska utgå från följande målgrupper (du får lägga till fler om du vill, men minst tre måste användas):
Ledning (Executive): vill ha överblick, trend och KPI:er för beslut.
Regionchef: vill jämföra regioner/butiker och hitta avvikelser.
Butikschef / Operations: vill följa daglig/veckovis försäljning och top/bottom-produkter.
Kategoriansvarig: vill se vilka produkter/kategorier som driver lönsamhet och volym.

Data (översikt)
I senare moment i kursen kommer du få ett datalagerutdrag som innehåller:
försäljningstransaktioner (datum, produkt, kund, butik, antal, pris, rabatt)
produkter (kategori, subkategori, varumärke, standardkostnad, listpris)
kunder (segment, stad/region/land)
butiker (stad/region/land + ev. lat/long)
Du behöver inte kunna exakta kolumnnamn i den här uppgiften – fokusera på vilka insikter som går att få ut.

Din uppgift (för IG/G)
Du ska skriva en behovsanalys som är kort, tydlig och användbar.

1) Välj målgrupper (minst 3)
Välj minst tre målgrupper från listan ovan.

2) Behov per målgrupp
För varje målgrupp ska du beskriva:
Affärsfrågor (3–5 st) - Formulera 3–5 frågor målgruppen vill kunna besvara (tänk: frågor som leder till beslut). Ex: Vilka kategorier driver mest profit den här månaden – och skiljer det sig mellan länder?
KPI:er (3–6 st) - Lista 3–6 KPI:er som stödjer frågorna. - För varje KPI: skriv en kort definition (1 mening) så att det är tydligt vad den betyder.
KPI:er ska vara mätbara och tydligt kopplade till affärsfrågorna (undvik vaga KPI:er som “bra försäljning”) Ex: Nettoomsättning: “Summa försäljning efter rabatt, exkl. moms".
Filter/slicers (2–4 st) - Vilka filter behöver målgruppen kunna använda för att analysera datan? - Exempel: datum, region, butik, kategori, segment, varumärke.

3) Verktygsval (SSBI)
Svara kort på följande:
Varför är Power BI ett bra val för detta case? (max 5–8 rader)
När räcker Excel/PowerPivot, och när blir det olämpligt? (max 5–8 rader)
Om rapporterna ska delas i organisationen: hur skulle du leverera detta i praktiken? (t.ex. Power BI Service, export/PDF, åtkomst/behörighet på en övergripande nivå – max 5–8 rader)
Fokus här är resonemang kring lämpliga verktyg för rätt målgrupp, inte licensdetaljer.

