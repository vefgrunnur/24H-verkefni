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

* Sýnidæmi:

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
