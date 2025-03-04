# ShoesShelf

Zadání od zaměstnavatele:

Navrhněte relační databázový model pro aplikaci pro správu velkého botníku v bowlingové herně

**Datový model musí obsahovat:**

- několik databázových tabulek a vazby mezi nimi
- atributy včetně vhodných datových typů
- cizí a vlastní klíče
- primární klíče, případné unikátní indexy budou-li třeba

**Aplikace musí umožňovat zjistit:**

Evidence typů bot i konkrétních párů bot určitého typu, jejich velikostí, datum zařazení do botníku, pořizovací cena, celkový počet vypůjčení pro daný pár, termín poslední dezinfekce, druh a závažnost poškození a zda je daný pár bot aktuálně zapůjčený nebo ne. Aplikace bude poskytovat podklad pro nákup nových bot jako náhrady za poškozené (kolik bot, jaké velikosti a typy). Aplikace bude vyhodnocovat, které typy bot jsou nejoblíbenější a navrhovat k zakoupení především takové typy, ovšem parametricky i s ohledem na pořizovací cenu.

# ShoesShelf - projekt dle zadání

Analytický návrh řešení: relační databázový model pro správu botníku v bowlingové herně. Aplikace má několik tabulek s cizími i vlastními klíči, je naplněna daty. Na záložce SHOES je předvedeno filtrování dat. Záložky mají řazení a stránkování. Aplikace je navržena v angličtině. Analytické schopnosti programu jsou na záložce Reports:

• Rental Report: aplikace udává množství vypůjčení bot stejného typu a velikosti, řazeno podle oblíbenosti, tedy od největšího počtu vypůjčení a pak podle ceny;

• Disinfection Report: aplikace vypisuje každý pár bot s uvedením data jen poslední desinfekce. V případě zařazení nového páru bot bez dezinfekce, se v Reportu u tohoto páru vyskytne záznam "Not yet disinfected";

• Substitution Report: aplikace navrhuje nákup bot s kritickou mírou poškození. V případě, že jsou v botníku 3 páry např. pánských bot stejné značky a velikosti s kritickým poškozením, navrhne aplikace k zakoupení 3 takové páry.

Detail jednotlivého páru bot vypíše veškeré jeho vlastnosti včetně typu, velikosti, data zařazení do botníku, pořizovací ceny, celkového počtu vypůjčení pro daný pár, termínu poslední dezinfekce, druhů a závažnosti poškození, a zda je daný pár bot aktuálně zapůjčený.

V aplikaci je implementován autentizační systém. **Přidání, úprava a odstranění záznamů je umožněno účtu administrátora (přednastaveno).**

HTML úprava je navržena s použitím knihoven Bootstrap a je interaktivní.
