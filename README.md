# Emulátor konzole Nintendo Entertainment System

Repozitář obsahuje zdrojový kód bakalářské práce, která se zabývá vývojem emulátoru herní konzole s důrazem na využití ve vzdělávání.

Bakalářská práce vznikala v letech 2022-2023 na FIT ČVUT.

## Kompilace
- Je nutné použít `biber` místo `bibtex`. TeXstudio používá jako výchozí právě `bibtex`, je to třeba přepnout v nastavení: `Options > Configure TeXstudio > Build > Default Bibliography Tool`.
- Před kompilací je nutno spustit generování bibliografie.
- Pro TeXstudio je nutné doinstalovat český slovník pro kontrolu pravopisu.

### Fedora
- Požadované balíčky oproti vestavěné instalaci na Fedoře 37:
  - czech.ldf,
  - dirtree.sty,
  - lipsum.sty,
  - epigraph.sty,
  - nextpage.sty,
  - minted.sty,
  - tip: na Fedoře lze TeXové balíčky nainstalovat pomocí dnf: `dnf install "tex(balicek.pripona)"`.
- Požadované další systémové balíčky na Fedoře 37:
  - texlive-collection-langczechslovak,
  - texlive-biblatex-iso690.
- Alternativní řešení: instalace kompletní distribuce: texlive-scheme-full

## Tipy
- tilda (~) na české klávesnici: `pravý Alt` + `Shift` + `` ` ``

## PDF
Při každém commitu proběhne kompilační pipeline a vygeneruje se export v PDF. Seznam artefaktů je k dispozici na kartě `Actions`.
