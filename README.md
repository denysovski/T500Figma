# TÓN – Data za hudbou

> Semestrální práce **KIT/KPGWD 2026** · Daniel Svoboda
> Klikací prototyp webové a mobilní aplikace, která z TOP 500 nejstreamovanějších umělců na Spotify dělá srozumitelný žebříček, porovnání a příběh z dat.

**Figma soubor:** <https://www.figma.com/design/a9Dnz0faB4rotRgaXwEfVf>  (File key `a9Dnz0faB4rotRgaXwEfVf`)

## O projektu

| | |
|---|---|
| Téma | Aplikace nad otevřenou datovou sadou – TOP 500 umělců na Spotify |
| Pro koho | Posluchači hudby a fanoušci interpretů |
| K čemu | Zjistit, kdo patří ke světové špičce, porovnat umělce, projít žánry a země |
| Rozsah dat | 500 umělců · 23 žánrů · 43 zemí |
| Snapshot dat | 17. 7. 2026 |
| Jazyk a vzhled | Česky, pouze tmavý režim |
| Výstup | Funkční prototyp ve Figmě + wireframy ke všem obrazovkám |

## Zdroje dat

- **Most Streamed Artists on Spotify** (Kaggle, rishavsvault) – <https://www.kaggle.com/datasets/rishavsvault/most-streamed-artists-on-spotify> (žánr, země, jazyk, typ, streamy celkem / Lead / Featured / Sólo).
- **World Bank, World Development Indicators** – počet obyvatel `SP.POP.TOTL`, rok 2024, CC BY 4.0 – <https://data.worldbank.org/indicator/SP.POP.TOTL>.

Sady se spojují přes zemi původu umělce; z toho vznikají obrazovky *Země na hlavu* (streamy na 1 mil. obyvatel). Podrobnosti v [`data/README.md`](data/README.md).

## Struktura Figma souboru

| Stránka | Obsah |
|---|---|
| 1. Cover | Titul, zadání, zdroje dat, počty obrazovek |
| 2. Foundation | Design tokeny (barvy, typografie, rozestupy) a komponenty |
| 3. Wireframes | Wireframy všech obrazovek, rozdělené po zařízeních |
| 4. Desktop | 26 obrazovek, 1440 px |
| 5. Mobile | 32 obrazovek, 390 × 844 |
| 6. Tablet | 32 obrazovek, 768 × 1024 |
| 7. Fold | 31 + 31 obrazovek, složený 360 × 800 a rozložený 674 × 841 |

Celkem **152 reálných obrazovek** a **152 wireframů** (počty i názvy si odpovídají). Detail v [`docs/screens.md`](docs/screens.md).

## Návod pro učitele – jak prototyp spustit

1. Otevřete odkaz na Figma soubor výše (stačí prohlížeč, účet není nutný pro zobrazení; pro komentáře je potřeba přihlášení).
2. V levém panelu *Pages* vyberte stránku zařízení (**4. Desktop**, **5. Mobile**, **6. Tablet**, **7. Fold**).
3. Klikněte na úvodní obrazovku (`01 Splash`, na desktopu `01`) a stiskněte **Present** (▶ vpravo nahoře) nebo klávesu `Ctrl/⌘ + Alt + Enter`.
4. Prototyp se ovládá kliknutím – spodní lišta / postranní menu, filtry, karty umělců, tlačítka *Porovnat*, *Zpět*. Přechody jsou jednotně **Dissolve 0,25 s**.
5. Doporučená trasa: Splash → Onboarding → Domů → TOP 500 → Filtry (Země, Jazyk – „Další“ rozbalí celý seznam) → Detail **Drake** (záložky Streamy / Podobní) → Porovnat (Drake vs. Taylor Swift) → Statistiky → Žánr Hip-Hop → Země původu → Víš, že… → Země na hlavu → Irsko.
6. Zařízení přepnete změnou stránky; **Fold** obsahuje dvě plátna (složený a rozložený).
7. Wireframy najdete na stránce **3. Wireframes** (sekce *WF · Mobile / Desktop / Tablet / Fold*). Obsahují „Metodickou poznámku“ k obrazovce.

### Poznámky k prototypu

- Do detailu umělce vede proklik pouze u **Drake** (ostatní řádky jsou ukázkové).
- Hover (ztmavení) funguje jen při najetí myší.
- Data: číslo streamů je v **mld.** s dvěma desetinnými místy a českou čárkou (např. `137,49 mld.`).
- Zdroje dat jsou uvedeny pouze na Coveru a v Nastavení.

## Struktura repozitáře

```
README.md          tento soubor
docs/              popis obrazovek, design systému a uživatelských toků
data/              popis zdrojů dat a odvozených čísel
exports/           sem patří PDF/PNG exporty z Figmy (viz exports/README.md)
```

## Autor

Daniel Svoboda · KIT/KPGWD · 2026
