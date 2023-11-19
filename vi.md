> Två lägen i vi, edit eller command.
> I edit så skriver man in text, avbryt editläge med esc. Då återgår man till kommandoläge.
> Det går att ställa in så man får en -- INSERT -- när man är i editläge, om det inte är default.
> Att flytta runt eller söka och andra aktiviter sker i kommandoläge.

Spara och avsluta:
:q	avsluta går inte om du gjort förändringa och inte sparat dessa.
:q!	avsluta utan att spara.
:w	för att spara, men inte avsluta.
:w!	för att forcera en sparning, kan behövas för readonly filer.
:wq	stapla write och quit.
:wq!	stapa write quit och force.

På konstiga terminaler kan : vara svårt att hitta, finns ett alternativ
ZZ 	sparar om det behövs och avslutar.


Flytta runt i texten
h	pil vänster, flytta markören ett steg till vänster.
j	pil ned, flytta markören ned en rad.
k	pil upp, flytta markören upp en rad.
l	pil höger, flytta markören ett steg till höger.
0	gå till början av raden.
$	gp till slutet av raden.
w	hoppa ett ord till höger.
/sök<cr>	Söker framåt i texten efter "sök" och flyttar markören dit.
?sök<cr>	Söker bakåt i texten efter "sök" och flyttar narkören dit.
n	repetera sök, framåt eller bakåt.
Z.	paginera så att aktuell rad är i mitten av terminalen.

Skriva:
i	Startar editläge, med insert vid aktuellt position. Flyttar eftervarande text bortåt.
I	Startar editläge, med insert efter att flyttat markören till början av raden.
a	Startar editläge, med append vid aktuellt positionm Flyttar eftervarande text bortåt.
A	Startar editläge, med append efter att flyttat markören till slutet av raden.
o	Öppnar en ny rad nedan i editläge
O	Öppnar en ny rad nedan i editläge

Byta ut text:
cw	byt ett ord 
1cw	byt ett ord 
2cw	byt ut två ord
r	byt ut en bokstav
1r	byt ut en bokstav
2r	byt ut två bokstäver
C	byt till radens slut.
ct<sök>	byt ut text fram till <sök> (bokstav)
cf<sök> byt ut text innklusive <sök> (bokstav)

Ta bort text:
dd	ta bort en rad 
1dd	ta bort en rad
2dd	ta port två rader
D	ta bort till slutet av raden

Paste: (När man tagit bort något kan man infoga detta någon annanstans)
P	infoga framför/ovan
p	infoga efter/nedan

Ångra/Gör om:
u	ångrar senaste förändring
CTRL-r	återställ senaste ångrade

Misc:
.	gör om senaste
~	ändra versal till gemen och gemen till versal (funkar bra med . (ovan))

