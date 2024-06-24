## Stílsíða - _Cascading style sheet_ (CSS)

Þegar HTML staðalinn var hannaður tók hann mestmegnis til þess að hægt væri að deila textaskjölum milli nettengdra tölva. Frumnotendur voru vísindamenn sem þurftu að geta deilt með sér þekkingu. Blessaða mennina óraði ekki fyrir framhaldinu ☺.

Þegar svo gervöll heimsbyggðin komst upp á lagið með notkun netsins og raunverulegir möguleikar þess fóru að koma í ljós þá varð mjög snemma ljóst að HTML staðallinn dygði bara ekki til að mæta auknum útlitskröfum.

Stílsnið (Cascading Style Sheets) eru sérstök snið sem notuð eru til að skilgreina umbrot og útlit HTML síðna. Stílsnið henta vel til að greina á milli innihalds (HTML) og útlits (CSS). Aðskilnaður innihalds og útlits HTML var boðaður af W3C.

Útlitshönnun HTML síðna tekur á sig alveg nýjar víddir og möguleikar á skapandi vinnu stóraukast við notkun stíla við vefsíðugerð.

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

* &gt;body> Hjúpað (Inline)
Stílar settir í HTML tög og gilda einungis fyrir tagið sem stílarnir eru í.
* &gt;head> Staðbundið (Local)
Stílar settir í haus, gildir fyrir allt HTML skjalið.
* &gt;link> Víðvært (Global)
Stílar eru settir í annað skjal sem stílsíða og hefur endinguna .css - allar
vefsíður sem tengdar eru stílsíðunni hafa sömu eiginleika og útlit.
Samanburður: Hjúpaðir **–** Staðbundið **–** Víðvært

Hjúpaðir stílar hafa forgang yfir staðbundna stíla og staðbundnir stílar yfir víðværum stílum. Þegar vefsíða birtist í vafra þá er ferlið í grófum dráttum svona:

* Vafrinn les inn í vinnsluminni tölvunnar fyrst það sem tengist síðunni ss myndir og stílsnið, síðan koma skipanir úr &gt;head> hlutanum ofaná og síðast uppsetningin sem sett er inní &gt;body> tagið ofaná allt saman.

Við munum nánast eingöngu tengja stílsíðu við vefsíður, &gt;link> (Víðvært/Global). Hinar aðferðirnar eigum við að forðast að nota (sjá nánari lýsingu á þeim hér aftast).

Skoðum aðeins Víðværu leiðina aðeins betur!

### Víðvært (global)

Styrkur stílsíðna felast í því að geta búið til stíla í sérskjali sem síðan er tengd við hverja þá HTML síðu sem setja skal undir sama útlit eða uppsetningu. Varla þarf að fjölyrða um hve öflugt þetta er og nægir að nefna samþætt útlit vefsvæðis. Ef breyta á einhverju þarf ekki að fara á hverja síðu fyrir sig heldur er nóg að breyta stílum í stílsíðunni. Til að nota víðværa stílsíðu þá þarf að vista það með endingunni **.css**

Til að geta notað stílana í CSS skjalinu þá þurfum við að setja &gt;link> tagið í HTML skjal sem vísar í CSS skjalið. Dæmi um hvernig stílsíða er tengd vefsíðu þá er notað HTML tagið &gt;link>:

#### &gt;!DOCTYPE HTML>

```HTML
    <html>
    <head>
    <meta charset="utf-8" />
    <title>Víðvært letursnið</title>
    <link href="stilsida.css" rel="stylesheet" />
    </head>

```


**href=”stilsida.css”** er slóðin að skjalinu stilsida.css (hafið HTML og CSS skjalið í sömu möppu). Í skjalinu stilsida.css koma þá stílarnir sem við notum:

```CSS
    h1 { color:red; } /*allar fyrirsagnir <h1> í öllum HTML skjölum 
                        eru í rauðum lit */
```
```
/* */ afmarkar athugasemdir í CSS skjali. Sá texti sem settur er á milli /* */ birtist ekki á vefsíðu. Þetta gerir hönnuði mögulegt að punkta hjá sér skýringar eða taka út hluta kóðans. 

&lt;!-- --> gegnir sama hlutverki innan HTML skjals.
```


Grunnmálfræði CSS samanstendur af veljara (selector) og stíl (declaration). Veljari (selector) getur verið HTML tag sem þú vilt stíla. Hver stíll (declaration) er með eigindi (property) og gildi (value). Semikomman aðgreinir stílana.

Veljarinn (Selector) kemur á undann, síðan kemur slaufusvigi { því næst skipun (Declaration), sem aftur er skipt í eigindi (property) og gildi (value) sem eru aðskilin með tvípunkti : og loks öfugur slaufusvigi }

> Til að gera slaufusviga: { = Alt Gr takkinn + 7 og } = Alt Gr takinn + 0
```
h1 {color:blue; font-size:12px;}

Þetta þýðir: Fyrir öll <h1> tög sem koma fyrir í HTML skjali þá skulu þau vera blá á
litinn (color:blue) og hafa leturstærðina 12px (font-size:12px).

Veitið athygli að tvípunktinum ( : ) sem aðgreinir eigindið og gildið sem það fær.

Semíkomma ( ; ) aðgreinir svo hvern stíl.


Þægilegt er að skipta línum upp eftir hverja skipun svo auðveldara sé að lesa úr

skipunum og minnka hættu á ritvillum:

**h
{
color:blue;
font-size:12px;
}**

### Sýnidæmi nr 1:

Þessi tvö skjöl þurfa að vera í sömu möppu, style.css og daemi1.html svo að
linkurinn <link> virki á milli þeirra. Bæði skjölin eru unnin og vistuð með editor.

Í CSS skjali sem ég gef heitinu style 1 .css skrifa ég eftirfarandi stílsnið(ekkert annað,
ekkert HTML):

```
p {color:red;} /* Allar málsgreinar <p> eru með rauðan texta*/
```
í HTML skjali sem heitir t.d. daemi1.html:

<!DOCTYPE HTML>
<html>
<head>
<title>Dæmi nr. 1</title>
**<link href="style1.css" rel="stylesheet" />**
<meta charset="UTF-8" />
</head>
<body>
<h1>Fyrirsögn</h1>
<p>Þessi texti í málsgrein verður rauður<p>
</body>
</html>


### Class og id

Ein aðferð við að bæta við stílum umfram þá sem eru sjálfgefnir eins og HTML tög
býður uppá er að nota class og id (nánar um id síðar). Sjá nánar:
[http://www.w3schools.com/css/css_id_class.asp](http://www.w3schools.com/css/css_id_class.asp)

Class

Hægt er að nota class eigindið á hvaða HTML tag sem er, oftar en einu sinni.

Þú býrð til class í CSS skjali með að skrifa punkt og svo eitthvert heiti (ekki byrja class
heiti á númeri).

Til að nota class í HTML skjalinu þá þarf að skrifa **class=”** heitið **”** í opna HTML tagið
þar sem þú vilt nota það.

Sýnidæmi:

Segjum svo að þú ert með tvær eða fleiri málsgreinar <p> í HTML skjali en þú vilt að
önnur þeirra sé með öðrum lit (red) og stærð (12px). Þetta er hægt að leysa með að
búa til class:

Kóðinn í CSS skjali:

```
p { font-size:10px } /* fyrir allar málsgreinar á vef */
```
```
.specialtext {
color:red;
font-size:12px;
}
```
Kóðinn í HTML skjali:

```
<body>
<h1 class=”specialtext” >Þessi fyrirsögn verður rauð og 12px
leturstærð</h1>
```
```
<p>Þessi málsgrein er með 10px leturstærð og ekki rauð</p>
```
```
<p class=”specialtext” > Þessi málsgrein er rauð á lit og með 12px
leturstærð </p>
</body>
```

<span>

Við notum <span> tagið þegar okkur vantar tag utan um ákveðinn texta. Þetta HTML
tag er sérstaklega gert til að vinna með class. Skoðum dæmi:

HTML: <p>Ég hef <span class=“blue_eyes“> ljósblá</span> augu </p>

CSS: **.blue_eyes** { color: #77aaff; }

### Útkoman: Ég hef ljósblá augu

Úreltar skipanir í HTML.

> Athugið að <font>, <center>, <u>, <s>, <font> <big><mall> <b><i> ásamt fleiri
tögum eru úreltar HTML 4 skipanir. Í dag eru þessar skipanir orðnar að eigindum
annara taga í CSS stílsniði.

#### GLÓSUR

Skoðum nú ýmislegt sem oft er spurt um, hvernig geri ég hitt og þetta í stílsniði?

Hvernig set ég mismunandi leturgerðir?

```CSS
    h3 {font-family:times}
    p {font-family:courier}
    p.sansserif {font-family:sans-serif}
```

```HTML
<body>
    <h3>Fyrirsögn, stærð 3</h3>
    <p>Malsgrein</p>
    <p class="sansserif">Önnur malsgrein</p>
</body>
```
Hvernig ákvarða ég stærð leturs?

```CSS
    h1 {font-size: 1 6px}
    h2 {font-size:130%}
    p {font-size:0.875em}
```

Hvernig móta ég útlit leturs?

```CSS
    h1 {font-style:italic}
```

```CSS
    h2 {font-style:normal}
    p {font-style:oblique}
```
Hvernig set ég bil milli stafa?

```CSS
    h1 {letter-spacing:-3px}
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
    p {text-indent:2em}
```
Hvernig móta ég útlit bókstafa(texta) (Hér er verið að nota class)?

```CSS
    p {text-transform:uppercase}
    p {text-transform:lowercase}
    p {text-transform:capitalize}

```

