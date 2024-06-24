# HTML staðallinn

HTML (_HyperText Markup Language_) er ívafsmál notað til þess að sníða stiklutexta. Það
inniheldur fjöldann allan af svonefndum tögum (_tags_) sem eru notuð til að merkja á rökréttan
hátt hvaða hlutar skjalsins þýða hvað, til dæmis hver fyrsta fyrirsögnin á síðunni er.

## Þekkja má HTML tög á því að þau byrja öll á < og enda á > tákninu.

Allar vefsíður byrja á < **html** > og enda á </ **html** > taginu. Munurinn á opnunartaginu og
lokunartaginu er skástrikið **/**. Hvert tag hefur svo að sjálfsögðu sitt ákveðna hlutverk í
uppsetningunni. Tæmandi listi yfir helstu tög sem notuð eru við html ritun er t.d. að finna á
vefsíðunni [http://www.w3schools.com/html5/html5_reference.asp](http://www.w3schools.com/html5/html5_reference.asp)

Hér er sýnidæmi um afar einfalda vefsíðu:

Þegar vefsíðan er skoðuð nánar (bakvið tjöldin) kemur í ljós HTML kóði vefsíðunnar.

```HTML
<!DOCTYPE HTML>
<html lang="is">
<head>
    <meta charset="utf-8" >
    <title> Fyrsta vefsíðan mín </title>
</head>
<body>
    <h1>Halló heimur!</h1>
</body>
</html>

```

* _&lt;!DOCTYPE HTML>_
    * Efst á HTML síðuna er sett skilgreining á hvernig skjal þetta er (_Document Type Defenition_). Í þessu tilfelli er um að ræða skilgreining fyrir HTML5 staðalinn.
* Utan um allt efni vefsíðunnar er &lt;html> &lt;/html>.
* &lt;head>
    * Allt sem er sett á milli &lt;head> og &lt;/head> tagið hefur áhrif á vefsíðuna en birtist ekki í vafranum. Fleiri skipanir fara í inn á milli &lt;head> taga t.d. javascript skriftur fara í &lt;script> tagið og vísanir í tengd skjöl fara í &lt;link> tagið.
* &lt;title>
    * &lt;title> birtir texta efst í gluggaröndinni í vefskoðaranum og einnig í eftirlæti ef síðan er valin af notanda.
* &lt;meta>
    * Stafasettið charset=“utf-8" er notað m.a. fyrir íslenska stafi.
* &lt;body> 
    * Allt efni sem birtist í vafra fer á milli &lt;body> og &lt;/body> tagsins. Hér á milli eru einnig flest önnur HTML tög skrifuð.

Þegar maður byrjar að skrifa HTML kóða fyrir vefsíðu þá er gott er að sjá fyrir sér
mannslíkamann sem skiptist í höfuð &lt;head> og bol &lt;body>. Öll ofangreind tög í sýnidæminu
eru nauðsynleg og mynda beinagrind vefsíðunnar. Athugaðu að það þessi tög eiga og mega
aðeins koma fyrir einu sinni fyrir hverja vefsíðu.

Æskilegur ritháttur er að nota eingögnu lágstafi í tögum: <body> texti </body>. Einnig er
þarft að hafa tög inndregin þegar tög eru fléttuð inn í önnur tög, það auðveldar yfirlestur
kóðans. Autt bil verður mest aðeins eitt stafabil í vafra, það hefur engin sjónræn áhrif í vafra
ef það er mikið bil á milli taga eða texta. Að ýta nokkrum sinnum um á bilstöng eða
vendihnapp hefur engin áhrif.

Tög mega ekki víxlast, því þá virka skipanir ekki rétt.

### Fyrisagnir &lt;h1> til &lt;h6>

Í HTML staðlinum er boðið upp á 7 leturtög &lt;h1> til &lt;h6> og &lt;p>, Sjálfgefið hafa tögin
ákveðnu hlutfalli af leturstærð &lt;body> tagsins. Body er sjálfgefið (_user agent_) 1em eða 16px.

&lt;p> tagið stendur fyrir málsgrein (paragraph). Leturtögin eru "_block element_" sem eru með 100% breidd og með línubil fyrir ofan og neðan tögin. Förum nánar í eiginleika taga í 2. verkefni.

&lt;br> tagið býr til 1 línubil í texta, fer í næstu línu (einsog að smella á vendihnappinn).

Dæmi:

```HTML
<!DOCTYPE HTML>
<html>
<head>
    <meta charset="utf-8">
    <title> Fréttavefurinn <title>
</head>
<body>
    <h1> Ísland óbyggilegt eftir 10 ár </h1>
    <h2>Þetta er undirfyrisögn </h2>
    <p>Þetta er dæmi um málsgrein ....</p>
</body>
</html>
```
**<sub> og <sup>**

<sup> tagið fær textann til að birtast ofan við miðlínu og <sub> fyrir neðan. Dæmi:

```
<p> Þetta tag fær textann til <sup> að birtast ofan við </sup> miðlínu </p>
```
```
<p><sub>Þetta tag fær textann til birtast neðan við miðlínu</sub> </p>
```

**<strong>** (^) Texti með áherslu (feitletraður)
**<em>** (^) Skáletraður texti.
**<hr>** (^) Býr til línu

# Upptaling í lista <ul>

Til að búa til lista upptalningu þá þarf að nota samvinnu tveggja taga, <ul> og <li> <ul>
stendur fyrir “unordered list” eða óraðaðann lista, <li> stendur fyrir “list item” eða lista
eintak.

Dæmi:

< **body** >
< **ul** >
< **li** > Janúar < **/li** >
< **li** > Febrúar < **/li** >
< **li** > Mars < **/li** >
< **li** > Apríl < **/li** >
< **li** > Maí < **/li** >
< **/ul** >
< **/body** >

Ef þið prófið þetta dæmi sjáið þið að hvert atriði í listanum fær ● (depill) fyrir framan sig. Það
er sjálfgefið tákn.

# Númeraður listi <ol>

Einnig er hægt að fá númeraða röð, þá notum við <ol> eða “ordered list”, raðaður listi, þá
koma númerin 1, 2, 3 og áfram hækkandi niður listann <li>.

Dæmi:

< **body** >
< **ol** >
< **li** > Janúar < **/li** >
< **li** > Febrúar < **/li** >
< **li** > Mars < **/li** >
< **li** > Apríl < **/li** >
< **li** > Maí < **/li** >
< **/ol** >
< **/body** >


# Sértákn.

Sumir stafir og tákn eru frátekin í HTML og þá þarf að rita þau á annan hátt í kóðanum. Það
er t.d. ekki hægt að nota < (minna) eða > (meira) táknin í texta þar sem vafrarinn mun rugla
þeim saman við html tögin. Einnig ætti heldur ekki að nota merkið og önnur merki beint á
síðu (betra fyrir leitarvélar).

```
< er ritað &lt;
> er ritað &gt;
autt bil er ritað &nbsp;
er ritað^ &copy;^
Listi yfir sértákn: http://www.w3schools.com/html/html_entities.asp
```
## Að búa til og vista fyrstu vefsíðuna.

Vistið skjalið með endingunni .html til að hægt sé að opna það í vafrara (browser).

Þú skoðar html síðuna með því einfaldlega að smella á html skjalið þar sem þú vistaðir það.

---

## Stílsíða - _Cascading style sheet_ (CSS)

Þegar HTML staðalinn var hannaður tók hann mestmegnis til þess að hægt væri að deila textaskjölum milli nettengdra tölva. Frumnotendur voru vísindamenn sem þurftu að geta deilt með sér þekkingu. Blessaða mennina óraði ekki fyrir framhaldinu ☺.

Þegar svo gervöll heimsbyggðin komst upp á lagið með notkun netsins og raunverulegir möguleikar þess fóru að koma í ljós þá varð mjög snemma ljóst að HTML staðallinn dygði bara ekki til að mæta auknum útlitskröfum.

Stílsíður (Cascading Style Sheets) innihalda sérstök snið sem notuð eru til að skilgreina umbrot og útlit HTML síðna. Stílsíður henta vel til að greina á milli innihalds (HTML) og útlits (CSS).Útlitshönnun HTML síðna tekur á sig alveg nýjar víddir og möguleikar á skapandi vinnu stóraukast við notkun stíla við vefsíðugerð.

* Mun auðveldara er að uppfæra útlit yfir heilt vefsvæði þar sem öllum
útlitstengdum reglum er haldið til haga í einu eða fáum skjölum.
* CSS býður upp á fullkomnari stjórn á útliti skjala.
* CSS býður upp á möguleika sem bæta aðgengi fatlaðra að innihaldi skjala.
* Með CSS má aðgreina mismunandi útlit á sama innihald (HTML ) fyrir t.d.
prentverk eða lófatölvu og vísa þá í mismunandi CSS skjal fyrir hvern og einn
miðil.

World Wide Web Consortium staðlaráðið, sem sér um HTML staðalinn tók þá ákvörðun að smíða viðbætur við staðalinn í stað þess að breyta honum og missa hann hugsanlega út í vitleysu. Stílsíður eru nú alsráðandi í útlitshönnun vefsíðna.

Sjá nánar á [http://www.w3.org/Style/CSS/](http://www.w3.org/Style/CSS/)


Þrjár leiðir eru færar til að setja stíla á HTML vefsíðu.

* &lt;body> Hjúpað (Inline)
Stílar settir í HTML tög og gilda einungis fyrir tagið sem stílarnir eru í.
* &lt;head> Staðbundið (Local)
Stílar settir í haus, gildir fyrir allt HTML skjalið.
* &lt;link> Víðvært (Global)
Stílar eru settir í annað skjal sem stílsíða og hefur endinguna .css - allar
vefsíður sem tengdar eru stílsíðunni hafa sömu eiginleika og útlit.
Samanburður: Hjúpaðir **–** Staðbundið **–** Víðvært

Hjúpaðir stílar hafa forgang yfir staðbundna stíla og staðbundnir stílar yfir víðværum stílum. Þegar vefsíða birtist í vafra þá er ferlið í grófum dráttum svona:

* Vafrinn les inn í vinnsluminni tölvunnar fyrst það sem tengist síðunni ss myndir og stílsnið, síðan koma skipanir úr &lt;head> hlutanum ofaná og síðast uppsetningin sem sett er inní &lt;body> tagið ofaná allt saman.

### Víðvær tenging (_global_)

Styrkur stílsíðna felast í því að geta búið til stíla í sérskjali sem síðan er tengd við hverja þá HTML síðu sem setja skal undir sama útlit eða uppsetningu. Varla þarf að fjölyrða um hve öflugt þetta er og nægir að nefna samþætt útlit vefsvæðis. Ef breyta á einhverju þarf ekki að fara á hverja síðu fyrir sig heldur er nóg að breyta stílum í stílsíðunni. Til að nota víðværa stílsíðu þá þarf að vista það með endingunni **.css**

Til að geta notað stílana í CSS skjalinu þá þurfum við að setja &lt;link> tagið í HTML skjal sem vísar í CSS skjalið. Dæmi um hvernig stílsíða er tengd vefsíðu þá er notað HTML tagið &lt;link>:

#### &lt;!DOCTYPE HTML>

```HTML
    <html>
    <head>
    <meta charset="utf-8">
    <title>Víðvært letursnið</title>
    <link href="styles.css" rel="stylesheet">
    </head>

```

**href=”styles.css”** er slóðin að skjalinu styles.css (hafið HTML og CSS skjalið í sömu möppu). Í skjalinu styles.css koma þá stílarnir sem við notum:

```CSS
    h1 { color:red; } /*allar fyrirsagnir <h1> í öllum HTML skjölum 
                        eru í rauðum lit */
```

> /*  */ afmarkar athugasemdir í CSS skjali. Sá texti sem settur þar á milli hefur ekki áhrif á útlit vefsíðu. Þetta gerir hönnuði mögulegt að punkta hjá sér skýringar eða taka út hluta kóðans. 

> &lt;!-- --> gegnir sama hlutverki innan HTML skjals.

### Sýnidæmi:

Þessi tvö skjöl þurfa að vera í sömu möppu, style.css og index.html svo að
tengingin &lt;link> virki á milli þeirra.

Í CSS skjali sem ég gef heitinu styles.css skrifa ég eftirfarandi stíl

```CSS
  p {color:red;} /* Allar málsgreinar <p> eru með rauðan texta*/
```

í HTML skjali sem heitir t.d. index.html:

```HTML
<!DOCTYPE HTML>
<html>
    <head>
        <meta charset="UTF-8">
        <title>Dæmi nr. 1</title>
        <link href="styles.css" rel="stylesheet">
    </head>
    <body>
        <h1>Fyrirsögn</h1>
        <p>Þessi texti í málsgrein verður rauð<p>
    </body>
</html>
```

Hvernig set ég mismunandi leturgerðir?

```CSS
    body {font-family: sans-serif}
    h3 {font-family: courier}
    .serif {font-family: serif}
```

```HTML
<body>
    <h1>Allt letur í vefsíðunni er sans-serif</h1>
    <h3>Millifyrirsögn í Courier</h3>
    <p>Málsgrein</p>
    <p class="serif">Önnur málsgrein með serif leturgerð</p>
</body>
```
Hvernig ákvarða ég stærð leturs?

```CSS
    h1 {font-size: 2rem}
    h2 {font-size:130%}
    p {font-size:16px}
```

Hvernig móta ég útlit leturs?

```CSS
    h1 {font-style:italic}
    h2 {font-style:normal}
    p {font-style:oblique}
```
Hvernig set ég bil milli stafa?

```CSS
    h1 {letter-spacing:3px}
    h4 {letter-spacing:0.5em}
```
Hvernig ákvarða ég þykkt leturs?

```CSS
    p.normal {font-weight:normal}
    p.thick {font-weight:bold}
    p.thicker {font-weight:900}
```

```HTML
<body>
    <p class="normal">This is a normal paragraph</p>
    <p class="thick">This is a thick paragraph</p>
    <p class="thicker">This is a thicker
    paragraph</p>
</body>
```

Hvernig jafna ég texta?

```CSS
    h1 {text-align:center}
    h2 {text-align:left}
    h3 {text-align:right}
```

Hvernig meðhöndla ég texta á mismunandi vegu?

```CSS
    h1 {text-decoration:overline}
    h2 {text-decoration:line-through}
    h3 {text-decoration:underline}
    a {text-decoration:none}
```

Hvernig dreg ég inn texta?

```CSS
    p {text-indent:2rem}
```
Hvernig móta ég útlit bókstafa (texta)?

```CSS
    p {text-transform:uppercase}
    p {text-transform:lowercase}
    p {text-transform:capitalize}

```

Bjargir

* [Yfirlit yfir CSS skipanir (_CSS Cheat seets_)](https://cheatsheets.shecodes.io/)


> Athugið að &lt;font> og &lt;center> ásamt fleiri tögum eru úrelt HTML 4 tög. Í dag eru tögin orðin að eigindum annara taga í CSS stílum.