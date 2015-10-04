# Drejebog-skabelon
Drejebogen er en nøje beskrivelse af hvad vi får at vide, hvad vi får se og hvad vi kommer til at høre på rusturen.

# Tips
LaTeX kan være en gevaldig hjælp, eller din værste fjende. Sæt dig ind i LaTeX, så bliver det meget nemmere at skrive længere opgaver. Denne repo indeholder drejebogen for DTU rusturen på Center Sjælland i 2014. Du er velkommen til at genbruge/modificere den på din rustur.

# Farvekodet navne
Det er en god idé at oprette kommandoer for hver vektor, så farvekoder er ens over alt og nemt kan ændres ét sted. En kommando kan oprettes i sin preamble som:
\newcommand{\NAVN}{{\colorbox{darkred}{\textbf{Vektor Navn}}}\xspace}
Nu kan kommandoen benyttes som følgende: ``Bilen afhentes af \NAVN og derefter blah...''

Her er en god liste over særskilte farver.
Definer farverne som ``cNAME'', så de nemt kan huskes og bruges andre steder (fx tabeller hvor vektoren har ansvar).
\definecolor{headline}  {RGB}{ 68, 90,196}
\definecolor{blue}      {RGB}{ 43,  0,255}
\definecolor{farve1}    {RGB}{100,230,204} 
\definecolor{farve2}    {RGB}{255,180,100} 
\definecolor{farve3}    {RGB}{204,153,204} 
\definecolor{farve4}    {RGB}{153,180,255} 
\definecolor{farve5}    {RGB}{204,204,204}
\definecolor{farve6}    {RGB}{146,235,100} 
\definecolor{farve7}    {RGB}{255,153,153} 
\definecolor{farve8}    {RGB}{255,255,102} 
\definecolor{farve9}    {RGB}{218,180,142} 
