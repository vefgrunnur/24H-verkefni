# HTML staðallinn

HTML (_HyperText Markup Language_) er ívafsmál notað til þess að sníða stiklutexta. Það
inniheldur fjöldann allan af svonefndum tögum (_tags_) sem eru notuð til að merkja á rökréttan
hátt hvaða hlutar skjalsins þýða hvað, til dæmis hver fyrsta fyrirsögnin á síðunni er.

> Þekkja má HTML tög á því að þau byrja öll á < og enda á > tákninu.

Allar vefsíður byrja á taginu < **html** > og enda á </ **html** >. Munurinn á opnunartaginu og
lokunartaginu er skástrikið **/**. Hvert tag hefur svo að sjálfsögðu sitt ákveðna hlutverk í
uppsetningunni. Tæmandi listi yfir helstu tög sem notuð eru við html ritun er t.d. að finna á
vefnum [https://www.w3schools.com/tags/](https://www.w3schools.com/tags/)


Þegar vefsíða er skoðuð nánar  í vafra (_hægri smella á mús og velja "inspector"_) kemur í ljós HTML kóði vefsíðunnar.

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

### Fyrisagnir &lt;h1> til &lt;h6>

Í HTML staðlinum er boðið upp á 7 leturtög &lt;h1> til &lt;h6> og &lt;p>, Sjálfgefið hafa tögin
ákveðnu hlutfalli af leturstærð &lt;body> tagsins. Body er sjálfgefið (_user agent_) 1em eða 16px.

&lt;p> tagið stendur fyrir málsgrein (paragraph). Leturtögin eru "_block element_" sem eru með 100% breidd og með línubil fyrir ofan og neðan tögin. Förum nánar í eiginleika taga í 2. verkefni.

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

### Upptaling í lista &lg;ul>

Til að búa til lista upptalningu þá þarf að nota samvinnu tveggja taga, &lg;ul> og &lg;li> &lg;ul>
stendur fyrir “unordered list” eða óraðaðann lista, &lg;li> stendur fyrir “list item” eða lista
eintak.

#### Ónúmeraður listi &lt;ul>

```HTML

<ul>
<li> Janúar </li>
<li> Febrúar </li>
<li> Mars < /li>
<li> Apríl </li>
<li> Maí </li>
</ul >
```

Ef þið prófið þetta dæmi sjáið þið að hvert atriði í listanum fær ● (depill) fyrir framan sig. Það
er sjálfgefið tákn.

#### Númeraður listi &lt;ol>

Einnig er hægt að fá númeraða röð, þá notum við &lt;ol> eða “ordered list”, raðaður listi, þá
koma númerin 1, 2, 3 og áfram hækkandi niður listann &lt;li>.

Dæmi:

```HTML

<ul>
<li> Janúar </li>
<li> Febrúar </li>
<li> Mars < /li>
<li> Apríl </li>
<li> Maí </li>
</ul >
```
---

### Textatög

Til að leggja áherslu á innihald texta er HTML staðallinn með nokkur sértög. 

```HTML
<strong> | <em> | <sup> | <sub> | <blockqoute>

```

- **&lt;strong>** Texti með áherslu (feitletraður)
- **&lt;em>** Skáletraður texti.
- **&lt;sup>** tagið fær textann til að birtast <sup>ofan við miðlínu<sub> 
- **&lt;sub> fær textann til <sub>að birtast neðan við</sub> miðlínu </p>
- **&lt;hr>** Býr til línu

---

### Sértákn.

Sumir stafir og tákn eru frátekin í HTML og þá þarf að rita þau á annan hátt í kóðanum. Það
er t.d. ekki hægt að nota `<` (minna) eða `>` (meira) táknin í texta þar sem vafrarinn mun rugla
þeim saman við html tögin. 

- `<` er ritað &lt;
- `>` er ritað &gt;
- autt bil er ritað &nbsp;
- sértáknið &copy; er ritað `&copy;`
- **&lt;hr>** Býr til línu
- &lt;br> tagið býr til 1 línubil í texta, fer í næstu línu.

Listi yfir sértákn: http://www.w3schools.com/html/html_entities.asp

---

### Ritun

Tög mega ekki víxlast, því þá virka skipanir ekki rétt.

---

### Bjargir

* [Verkefnalýsing 1](../../)
* [Námsefni 1](../)
* [CSS, sjá nánari umfjöllun](stylesheet.md)
* [Yfirlit yfir HTML skipanir (_HTML Cheat seets_)](https://cheatsheets.shecodes.io/html)