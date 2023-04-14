# Emulátor konzole Nintendo Entertainment System
Repozitář obsahuje zdrojový kód textu bakalářské práce, která se zabývá vývojem emulátoru herní konzole s důrazem na využití ve vzdělávání. Samotná implementace je k dispozici v [samostatném repozitáři](https://github.com/andreondra/use).

Bakalářská práce vznikala v letech 2022-2023 na FIT ČVUT.

## Zkompilované PDF
- Nejnovější PDF je k dispozici v záložce [Actions](https://github.com/andreondra/bachelor-thesis/actions). Každý commit spustí kompilaci, která vyprodukuje artefakt: ZIP archiv obsahující PDF práce.
- PDF pouze z commitů do hlavní větve ("stabilní" vydání) je k dispozici jako [release s tagem latest](https://github.com/andreondra/bachelor-thesis/releases/tag/latest).

## Vlastní kompilace
- Je nutné použít `biber` místo `bibtex`. TeXstudio používá jako výchozí právě `bibtex`, je to třeba přepnout v nastavení: `Options > Configure TeXstudio > Build > Default Bibliography Tool`.
- Dále je nutné v TeXstudio přidat parametr `--shell-escape` pro PdfLaTeX: `Options > Configure TeXstudio > Commands`.
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
  - bytefield.sty,
  - tikz-timing.sty,
  - tip: na Fedoře lze TeXové balíčky nainstalovat pomocí dnf: `dnf install "tex(balicek.pripona)"`.
- Požadované další systémové balíčky na Fedoře 37:
  - texlive-collection-langczechslovak,
  - texlive-biblatex-iso690.
- Alternativní řešení: instalace kompletní distribuce: texlive-scheme-full

### Ubuntu
- V distribuci Ubuntu lze nainstalovat celou distribuci texlive pomocí `apt install texlive-full`. Případně lze použít balík `texlive-base` doplněný o `texlive-lang-czechslovak`, `texlive-latex-extra` a `texlive-science`.
- Dále je nutné doinstalovat biber: `apt install biber`.

## Tipy
- tilda (~) na české klávesnici: `pravý Alt` + `Shift` + `` ` ``

## Licence
(C) 2023, Ondřej Golasowski
