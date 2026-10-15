# Design system (stránka 2. Foundation)

- **Téma:** pouze tmavé; barvy a rozestupy jsou Figma proměnné (variables), písmo Figtree, limetkový akcent.
- **Komponenty:** Button, LoadMoreButton, FilterChip, SearchField, LeaderboardRow, ArtistCard, StatCard, Heart, BackButton, CompactRow, GenreRow, ErrorState, DragHandle, FadeIn, SplashZnačka a navigace (MobileTabBar, DesktopTopBar, DesktopSidebar). MobileTabBar má varianty Mobile (390 px) a Folded (360 px).
- **Formát čísel:** 2 desetinná místa, česká čárka; streamy v **mld.**; procenta s mezerou před `%` (`49,11 %`).
- **Přechody prototypu:** navigace používá výhradně *Dissolve* 0,25 s (ease in-and-out). Přepnutí srdíčka je okamžitá změna varianty.
- **Responzivita:** tlačítka a řádky se přizpůsobují šířce (auto-layout, Fill/Hug); bez překryvů; spodní lišta na mobilních zařízeních je ukotvená u dolního okraje; na desktopu zůstává postranní navigace.
- **Interaktivita:** stavy rozbalení (Země, Jazyk, Typ umělce, Streamy, Žánry) a pořadí v Oblíbených jsou řízené booleovskými proměnnými prototypu (kolekce Filtry).
- **Obrázky:** ilustrace umělců vyplňují karty a jsou oříznuté tak, aby byly vidět hlavy. Nejsou roztažené.
