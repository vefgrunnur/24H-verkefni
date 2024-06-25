# Skjálitir.

Litir Í tölvuskjá eru samsettir úr mismiklu magni af Rauðu, Grænu og Bláu ljósi. Litir sem eru í
vefsíðu eru skilgreindir í stílsíðu með þrennskonar hætti.

Hér er sýnt hvernig unnt er að skrá liti með nafni, í sextánda kerfinu og RGB milljón litakerfinu.

```CSS
h1 { color: red; } /* sérsniðin litur í CSS staðlinum */
h2 { color: #dda0dd; } /* Hexadecimal tölur fyrir R=dd, G=a0, B=dd */
h3 { color: rgb(20,100,255); /* rgb er skilgreiningin sem mælt er með að nota í dag */ }
```
Á meðan tölvuskjáir gátu aðeins birt 256 liti þá höfðu menn fyrir því að skilgreina þá alla
með nafni. Þeir voru kallaðir _„websafe“_ litir.

Dæmi: Aqua, gray, navy, silver, black, green, olive, teal, blue, lime, purple, white, fuchsia, -maroon, red, yellow.

Hexadecimal talnakerfið er ólíkt tugakerfinu á þann veg að það notar 16 aðgreinanleg “tákn”
til að túlka tölur. Kerfið nefnist sextándakerfi á íslensku. Þessi “tákn” eru:

```
(lægsta gildi) 0 1 2 3 4 5 6 7 8 9 A B C D E F (hæsta gildi)
```
**#**, _hash_ táknið verður að standa fyrir frama tölugildið til að vafrinn lesi kóðann rétt

- #FFFFFF = Hvítur
- #000000 = Svartur
- #FF0000 = Rauður
- #00FF00 = Grænn
- #0000FF = Blár

Það er hægt að stytta tölugildin 6 í 3 ef tölurnar tvær sem skilgreina R, G og B eru þær sömu

- #FF0000 = #F00 = Rauður
- #00FF00 = #0F0 = Grænn
- #0000FF = #00F= Blár

**RGB** litir samanstanda af öllum þeim litbrigðum sem tölvuskjár getur sýnt og augað
nemur. Ljósmagnið er mælt frá 0 upp í 255.

- rgb(0,0,0) = svart
- rgb(127,127,127) = grátt
- rgb(255,255,255) = hvítt

Sjá nánar á: [http://www.w3schools.com/css/css_colors.asp](http://www.w3schools.com/css/css_colors.asp)


