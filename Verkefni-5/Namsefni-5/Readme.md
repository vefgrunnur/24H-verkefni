#Tenglar (_links_)

Mjög gott getur verið að hafa tengla sem vísa á ákveðinn hluta innan vefsíðu. Þetta gerir notanda mögulegt að nálgast efnisatriði á auðveldan hátt. 

Í HTML er þetta gert með ID eigindinu. 

```HTML
    <body id =“top“ >Efst á síðu</a>
```

ID eigindið sem geymir hina eiginlegu tilvísun á ákveðna staðsetningu í skjalinu. Vafrinn notar # táknið til að finna ID skilgreininguna.

```HTML
    <a href="#top">Efst á síðu</a>
```

* [Dæmi um innri tengla](Daemi/relative_links.html) (_relative links_)

Stílsniði beitt á tengla
Til að beita áhrifum stílsniðs á tengla þá eru notaðir svokallaðir "huldu"-klasar (pseudo-class).
Þetta er aðferð til að hafa áhrif á undirtög sumra html-taga. Gott dæmi um slíkt eru einmitt
viðbæturnar við tengi-tagið <a>. Þar eru fyrir eigindin link, visited, hover og active.

Dæmi: í stílsíðu

```CSS
a:link {color: #F00}
a:visited {color: #0F0}
a:hover {color: #F0F}
a:active {color: #00F}
```

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
