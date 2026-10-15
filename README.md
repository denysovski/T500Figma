# TÓN – Data za hudbou

Semestrální práce **KIT/KPGWD 2026**. Klikací prototyp webové a mobilní aplikace, která z TOP 500 nejstreamovanějších umělců na Spotify dělá srozumitelný žebříček, porovnání a příběh z dat.

**Figma soubor:** <https://www.figma.com/design/a9Dnz0faB4rotRgaXwEfVf>

## O projektu

TÓN je aplikace nad otevřenou datovou sadou TOP 500 umělců na Spotify. Posluchačům hudby a fanouškům interpretů ukazuje, kdo patří ke světové špičce, umožňuje umělce porovnat a projít žánry i země původu. Prototyp je česky a pouze v tmavém režimu, vznikl pro desktop, mobil, tablet a skládací zařízení (složené i rozložené) a ke všem obrazovkám obsahuje wireframy. Data pocházejí ze snapshotu z 17. 7. 2026: 500 umělců, 23 žánrů a 43 zemí.

## Zdroje dat

- **Most Streamed Artists on Spotify** (Kaggle, rishavsvault) – <https://www.kaggle.com/datasets/rishavsvault/most-streamed-artists-on-spotify>
- **World Bank, World Development Indicators** – počet obyvatel `SP.POP.TOTL`, rok 2024, CC BY 4.0 – <https://data.worldbank.org/indicator/SP.POP.TOTL>

Sady se spojují přes zemi původu umělce. Podrobnosti v [`data/README.md`](data/README.md).

## Struktura repozitáře

```
README.md          tento soubor
docs/              popis obrazovek, design systému a uživatelských toků
data/              popis zdrojů dat a odvozených čísel
exports/           sem patří PDF/PNG exporty z Figmy (viz exports/README.md)
```

## Autor

Daniel Svoboda · KIT/KPGWD · 2026
