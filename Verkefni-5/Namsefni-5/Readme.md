# Í VINNSLU

##Tenglar innan sömu HTML síðu:

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




* [Sýnidæmi](Dæmi)
* [Vefsíður til að vinna með](verkefni-5)

### Leturstillingar í CSS

```CSS

body {
    font-family: Helvetica, sans-serif; /* vafrinn velur Helvetica ef það er til, annars system font (sans-serif) */ 
    font-style: normal;      /* italic , obligue */
    font-weight: normal;     /* bold , 100 - 900 */
    font-size: 1em;          /* 1px , 1rem , 100% */
    line-height: 1.5;         /* tekur mið af einingunni sem er á font-size, staðlað 1.3 */
}

/* hér er öllum stílum sópað saman í eina skipun "font:"*/
body {
    font:italic bold 100%/120% Georgia, Times, serif;
    /*font-style, -weight, -size/-lineheight -family */
}


```

### Bakgrunnsmynd í vefsíðu

```CSS

body {
    background-color: #6ff;
    background-image:url(flott-logo.svg);
    background-repeat: no-repeat;     /* repeat-x eða repeat-y */
    background-position: 200px 300px; /* föst staðsetning frá vinstra horni efst */
    background-position: center middle;
    /* X lárétt: left, center, right. Y lóðrétt: top, middle, bottom */
    background-attachment: fixed; /* scroll */	
}
/* allar bakgrunns-skipanir í einni */
body {			
	background: rgb(3,3,3) url(image.jpg) 0px -5px scroll no-repeat;
            /*  litur,   mynd,  staðsetning X-Y,  fixed,  repeat -x -y */

}

```
