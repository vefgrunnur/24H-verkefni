# Tenglar (_links_)

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

## Hulduklasar (_pseudo-class_)

Til að gera vafrann móttækilegan (_responsive_) þá eru til svokallaðir _hulduklasar_ sem bregðast við notkun notandans.

```CSS
    a:link {color: #F00}
    a:visited {color: #0F0}
    a:hover {color: #F0F}
    a:active {color: #00F}
```

* ```:link``` upphaflegur litur. Blár er staðallitur og texti undirstrikaður
* ```:visited``` annar litur gefur til kynna að notandi hefur notað tenginguna
* ```:hover``` ATHUGIÐ! virkar ekki á snertiskjá
* ```:active``` virkar þegar tengill er snertur eða valinn

Það eru fjölmargir aðrir hulduklasar sem notaðir eru í CSS stílsíðu og við förum nánar í notkun þeirra í næsta áfanga. [Sjá nánar.](https://www.w3schools.com/css/css_pseudo_classes.asp)

---

### Leturstillingar í CSS

```CSS

body {
    font-family: Helvetica, sans-serif; /* vafrinn velur Helvetica ef það er til, annars system font (sans-serif) */ 
    font-style: normal;      /* italic, obligue */
    font-weight: 500;     /* normal, bold, 100 - 900 */
    font-size: 1rem;          /* 16px, 1em, 100% */
    line-height: 1.5;         /* tekur mið af einingunni sem er á font-size */
}

/* hér er öllum stílum sópað saman í eina skipun "font:"*/
body {
    font:normal 500 1rem/1.5 Helvetica, sans-serif;
    /*font-style, -weight, -size/-lineheight -family */
}


```

### Bakgrunnsmynd í vefsíðu

Þar sem meirihluti vafranotkunar er á farsímaskjáum þá ber að forðast flókanr og litríkar ljósmyndir. Best að sleppa þeim eða notast við hlutlausa fleti.

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
