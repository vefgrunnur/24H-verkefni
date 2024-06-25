# Tenglar í vefsíðu (_e. links_).

HTML – tög geta í flestum tilvikum haft viðbætur sem nota má til að stýra enn betur eðli
þeirra og gefa þeim aukna möguleika. Þessar viðbætur eru kallaðar á ensku “attributes” sem
á íslensku gæti útlagst sem eigindi. Hverju eigindi fylgir svo ákveðið gildi (value).

Til að tengjast öðrum vefsíðum þurfum við að útbúa svokallaðan tengil (link). Það er gert
með eftirfarandi hætti:

<a href=”http://www.tskoli.is”> Tækniskólinn </a>

Best er að brjóta þetta niður í eftirfarandi einingar:

```
<a er skipun. href= er eigindi og “http://www.tskoli.is” er gildið, >
```
Tækniskólinn er textinn sem birtist á vefsíðunni </a> taginu lokað

Takið eftir að eigindið og gildið er sett inn í opnunartagið sem í þessu tilviki er <a>. Þetta
verður alltaf að gera, ef eigindið og gildið er sett ekki rétt uppsett verður það óvirkt.
Hér er href eigindi (attribute) af taginu a og **“http://www.tskoli.is”** er gildið (value), sem
eigindið tekur með sér.

Tenglar innan sömu HTML síðu:
Mjög gott getur verið að hafa tengla á einhvern ákveðinn hluta innan vefsíðu. Þetta gerir
vefhönnuði mögulegt að nálgast efnisatriði á auðveldan hátt. Í HTML er þetta gert með <a>
taginu. Ef við viljum til dæmis vera með link á síðunni sem sendir notandann efst á síðuna er
eftirfarandi kóði settur efst á síðuna:

```
< body id =“top“ ></a>
```
Hér er svo id eigindið sem geymir hina eiginlegu tilvísun á ákveðna staðsetningu í skjalinu,
þið sjáið að með a taginu er id eigindið.
Til að komast að akkerinu er notast við eftirfarandi kóða: **<a href=”#top”>** Efst á síðu</a>

Dæmi:

```
<!DOCTYPE HTML>
<html>
<head>
<meta charset="utf-8">
<title>The Odessey</title>
</head>
<body id="top"> <!--hér er akkeri efst á vefsíðunni -->
<p>
<a href="#thesecond">Skoða Fit the second</a>
</p>
<p>
<a href="#thethird">Skoða Fit the third</a>
</p>
```

```
<h1>The Odyssey</h1>
<h2>Fit the first</h2>
<p> A maid servant then brought them water in a beautiful golden ewer
and poured it into a silver basin for them to wash their hands, and
she drew a clean table beside them </p>
<p> An upper servant brought them bread, and offered them many good things
manner of meats and set cups of gold by their side, and a man – servant
brought them wine and poured it out for them. </p>
<p><!--með því að hafa akkeri í sér málgrein <p> þá er aukalínubil fyrir ofan
millifyrirsögnina -->
<a id="thesecond">&nbsp;</a>
</p>
<h2>Fit the second</h2>
<p> An upper servant brought them bread, and offered them many good things
of what there was in the house, the carver fetched them plates af all
manner of meats and set cups of gold by their side, and a man – servant
brought them wine and poured it out for them. </p>
<p>Then the suitors came in and took their places on the benches and
seats. Forthwith men servants poured water over their hands, maids
went round with the bread – baskets, pages filled the mixing - bowls
with wine and water, and they laid their hands upon the good things
that were before them.</p>
<p><a id="thethird">&nbsp;</a></p>
<h2>Fit the third</h2>
<p>Then the suitors came in and took their places on the benches and
seats. Forthwith men servants poured water over their hands, maids
went round with the bread – baskets, pages filled the mixing - bowls
with wine and water, and they laid their hands upon the good things
that were before them.</p>
<h2>Contact us</h2>
<p>Did you enjoy reading this excerpt ?<br />
You can find the entire text of The Odyssey in the University Bookstore, </p>
<h4> University Bookstore<br />
1111 Central Gate Drive<br />
Somecity, U.S.A<br />
</h4>
<p><a href="#top">Efst á síðu</a></p>
</body>
</html>
```
Stílsniði beitt á tengla
Til að beita áhrifum stílsniðs á tengla þá eru notaðir svokallaðir "gerfi"-klasar (pseudo-class).
Þetta er aðferð til að hafa áhrif á undirtög sumra html-taga. Gott dæmi um slíkt eru einmitt
viðbæturnar við tengi-tagið <a>. Þar eru fyrir eigindin link, visited, hover og active.

Dæmi: í stílsíðu
a:link {color: #F00}
a:visited {color: #0F0}
a:hover {color: #F0F}
a:active {color: #00F}

Í HTML síðu
<a href="einhversida.html">Hér er tengill sem skiptir um lit</a>


