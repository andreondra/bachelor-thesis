# Zadání
## Návrh v bodech
- téma: emulace výpočetního systému - herní konzole NES
- úvodní část: technická specifikace a historie NES
- analytická část: definice emulace, rešerše existujících implementací, dokumentací a datasheetů
- návrhová část: návrh použitých technologií, typu a přesnosti emulace (možno spojit rovnou s implementační?)
- implementační část:
    - implementace procesoru 6502 - standardní i nestandardní instrukce, obsluha přerušení, univerzální rozhraní sběrnice,
    - implementace grafického čipu PPU (2C02) - renderování pozadí i popředí (spritů),
    - implementace rozšíření procesoru (2A03 - obsahující navíc zvukový čip APU) - implementace syntezátorů a jejich korektní synchronizace,
    - implementace periferií - herních ovladačů,
- ladicí část: kontrola věrnosti emulace prostřednictvím testovacích programů, (srovnání výsledků s reálným systémem)

## Textový návrh
Navrhněte a realizujte softwarový emulátor herní konzole Nintendo Entertainment System. Zmapujte existující implementace, dostupné dokumentace a katalogové listy. Na základě rešerše navrhněte vhodné technologie a způsob řešení emulace. Využijte OOP a jednotlivé komponenty implementujte jako třídy. 

V analýze i následné implementaci se zaměřte na: 
- procesor 6502: standardní i nestandardní instrukce a obsluhu přerušení. Třídu navrhněte univerzálně tak, aby se dala využít i v jiných emulátorech systémů používající stejný procesor.
- grafický čip 2C02: renderování pozadí i popředí.
- rozšíření procesoru 2A03: zpracování zvuku (APU), implementace syntezátorů a jejich synchronizace.
- periferie: herní ovladače.
- rozhraní emulátoru: mělo by poskytovat přehledné grafické rozhraní poskytující nejen uživatelské, ale i vývojářské rozhraní (zobrazení stavu komponent, obsahů pamětí...).

Zahrňte i ladicí část, kde zkontrolujete věrnost emulace pomocí testovacích obrazů ROM. Výsledky srovnejte s reálným systémem.