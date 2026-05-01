# moebius-techare.github.io
Moebius hemsida

# Allmänt

Hur fungerar Möbius hemsida?

Jo, allt styrs genom ett program som heter Hugo. Hugo är inte IUPAK:s kamel utan något annat. Nämligen ett program som tar .md-filer (en sådan som du läser just nu) och genererar en html-sida.

Om du kikar vad det finns för mappar så är det ganska många och det kan se läskigt ut, men det är egentligen bara några stycken som du behöver känna till:

- `content`: I denna mapp ligger alla filer som kommer att bli till hemsidan. Den som heter `index` kommer att bli hemsidan, i.e. `moebius.nu` kommer att displaya det som står i `index.md` och ligger i contentmappen. De andra kommer att bli till exempel `moebius.nu/links`. Notera att det av varje fil finns två varianter, `.en.md` och `.sv.md`. Som du säkert gissat så styr dessa den engelska och den svenska versionen av sidorna.

- `public`: Hit kommer hemsidan som genereras, så man ska inte in och peta här, utan snarare bara läsa härifrån. För att testköra hemsidan lokalt, kör `hugo serve` i root-foldern, alltså där alla dessa mappar ligger. 

- `themes`: Här ligger temat, den är kopierat från en annan repo och fungerar genom någon slags magi.

- `config`: Här kan man knepa lite om man vill ha fler grejer i menyn och så och lite annat bus. 

- `static`: Här ligger alla bilder och andra dokument.

För att publicera hemsidan så är det bara att ändra det man vill göra och sen pusha, man behöver inte köra `hugo` utan det sköter github automagiskt.

Hoppas detta hjälper dig, du framtida Möbiot

*Sör'n*
2025

# Lägga till nya tentor / adding new exams

Tentorna ligger i `static/Exams` och sedan en mapp per kurs. Lägg in tentorna där och namnge dem enligt vad andra tentor heter, alltså `Kurs ååmmdd` och `Kurs ååmmdd losn` för lösningar. Sedan är det bara att göra en pull-request och github löser resten.


The exams are in `static/Exams`  and then one folder per course. Add the exams there and name them accordingly, i.e. `Course yymmdd` and `Course yymmdd losn` for solutions. The you just do a pull-request and github solves everything automatically.
