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

#### GLÓSUR

Hér eru dæmi um hvernig hægt er að stíla tög.

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



#### Úreltar skipanir í HTML.

Athugið að &lt;font>, &lt;center> ásamt fleiri tögum eru úrelt HTML 4 tög. Í dag eru tögin orðin að eigindum annara taga í CSS stílum.