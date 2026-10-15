# Design system (stránka 2. Foundation)

- **Téma:** pouze tmavé; barvy a rozestupy jsou Figma proměnné (variables).
- **Komponenty:** FilterChip (vybraný / nevybraný), Button (primary / secondary), StatCard, MobileTabBar, Zpět, karty umělců, řádky TOP 500, datové sloupce (bar chart).
- **Formát čísel:** 2 desetinná místa, česká čárka; streamy v **mld.**; procenta s mezerou před `%` (`49,11 %`).
- **Přechody prototypu:** výhradně *Dissolve* 0,25 s (ease in-and-out), bez pohybu.
- **Responzivita:** tlačítka a řádky se přizpůsobují šířce (auto-layout, Fill/Hug); bez scroll indikátorů a překryvů; na desktopu zůstává postranní navigace.
- **Interaktivita:** stavy rozbalení (Země, Jazyk, Streamy, Žánry) jsou řízené booleovskými proměnnými prototypu.
- **Obrázky:** vyplňují karty tak, aby byly vidět hlavy umělců; chybějící foto nahrazuje placeholder.
