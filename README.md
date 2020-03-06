# Drejebogsskabelon

Udarbejdet af Rasmus Aagaard (s164419) i 2019, med udgangspunkt i og inspiration fra skabelon udarbejdet af Henriette Steenhoff (s134869) i 2015. Videre udviklet af Niels Kjær Ersbøll (s183903) i 2020.

Link til en ikke-redigerbar version af skabelonen kan findes på [Overleaf](https://www.overleaf.com/read/dgwdvqshrfnb)

## Generelt om skabelonen

Man vil i denne skabelon finde en masse ting, som er specifikt for rusturen, som skabelonen er bygget op efter. Det er tiltænkt at man selvfølgelig læser det kritisk igennem og retter til, så det passer med tidspunkter, fordeling af ansvar, hvilke dage man er afsted osv.

## Navnekoder

Navnekoder angives med kommandoen `\navnekode` som tager tre parametre: selve navnekoden, altså hvad du vil skrive for at få det frem, farven og navnet. F.eks. `\navnekode{\DAK}{orange}{Dr Dakkensmirtz}`.

Alle farver til navnekoder er taget fra [latexcolor.com/](http://latexcolor.com/)

En idé kan være at give holdene en navnekode, som er deres tværvektors navnekode, bare med modsat store/små bogstaver. Eksempelvis, hvis vektorens navnekode er `\MEME` ville holdets navnekode være `\meme`, eller omvendt.

## Kontaktinformation

Udfyld `latex/forrest/kontaktinfo.tex` med relevant information fra [Studiestartswikien](https://studiestartswiki.pf.dk/rusturshytter:start). Tag evt. inspiration fra tidligere drejebøger, som kan findes nederst på siden for en given hytte.

## Tidsplaner

Der kan findes et eksempel på en tidsplan i filen `latex/dage/01_ankomst/01_tidsplan.tex`. For at indsætte flere linjer på tidsplanen kan man med fordel sætte sin cursor på en linje i tidsplanen, holde `Shift+Alt` nede og trykke på op eller ned piletasterne. Dette vil kopiere den aktuelle linje.

## Materialeliste

Til at lave materialeliste bruges filen `matlist.tex` som findes i `latex/settings/matlist.tex`. Formatet til dette er således at man bruger `mats`-miljøet (`\begin{mats}{}{}`) og derefter angiver dag og aktivitet, f.eks. `\begin{mats}{Lørdag}{Bustur}`. Herefter angiver man materialer ved brug af `\mat{}{}`, hvor parametrene angiver størrelsesorden og materiale, f.eks. `\mat{750}{Knæklys}`. Eksempler på dette kan findes rundt omkring i drejebogen. `matlist.tex` samler så samtlige materialelister bagerst i drejebogen, så det er nemt at få overblik over, hvad man skal bruge på hvilke dage og til hvilke aktiviteter.

## Tips til at få ting til at passe ind på én side

Der forekommer ofte meget lange tabeller, som der ikke er plads til på en enkelt side. Her kan man bruge `\begin{landscape}` til at få siden til at vende horisontalt frem for vertikalt.

Det er også en mulighed at gøre teksten mindre ved brug af `\tiny` eller lignende. Det kan stadig godt læses i praksis og navnekoderne hjælper med at finde ud af hvilket hold det er, når man står med et telefon flashlight kl 23:30 om natten på natløb.

## Subfiles

Skabelonen udnytter `subfile` LaTeX pakken til at gøre det nemmere at redigere i dokumenterne. Når man compiler en fil i LaTeX, vil det kun være den ene side som bliver skabt og ikke hele dokumentet. Ved dette sparer man både tid og resourcer. For at compile hele dokumentet skal man gå ind i `main.tex` og compile. For at tilføje flere filer oprettes `.tex` filen og der skrives i `main.tex` `/subfile{[stien.til.filen.tex]}`, eksempel:

`main.tex`

```tex
\subfile{latex/forrest/morgenrejsning.tex}
```

I den nye fil er det vigtigt at tilføje de følgende komandoer rundt om indholdet, hvor `[../../main.tex]` er den relative sti til `main.tex` filen

`latex/forrest/morgenrejsning.tex`

```tex
\documentclass[../../main.tex]{subfiles}
\begin{document}

%%%
% Indholdet af dokumentet her
%%%

\end{document}
```
