# Uppsetning HTML vefsíðu 

```HTML

<!DOCTYPE html><!-- Nýasta útgáfa HTML. Ef yfilýsingin er ekki tekin fram notar vafrinn 4. útgáfuna -->
<html lang="is">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <!-- Hér kemur efni sem birtist í vafra (browser) -->
</body>
</html>

``` 

Mundu að eftirfarandi þarf ávallt að vera til staðar í HTML skjali:

-   **\<!DOCTYPE HTML\>** tilgreinir hvaða útgáfu af HTML staðli vafrinn
    á að nota, þetta er HTML 5 skilgreining.

-   **\<html skipunum\>** á alltaf að loka með **\</\...\>** og enda
    skjalið **\</body\>\</html\>** undantekningar eru nokkrar t.a.m. **\<meta\>, \<img\>,\<br\>, \<hr\> og \<input\>**

-   Vistið skjalið með endingunni **.html** til að hægt sé að opna það í
    vafra (browser).

-   Það má **EKKI hafa** **íslenska stafi** í heiti skjalsins eða hafa
    **stafabil** í heitinu.

-   Þú skoðar html síðuna í vafra með því að smella á html skjalið þar
    sem þú vistaðir það.

* [Sjá nánari umfjöllun](HTML-CSS/README.md)
________________________________________________________

# CSS stílsetning

Grunnmálfræði CSS samanstendur af veljara (selector) og stíl (declaration). Veljari (selector) getur verið HTML tag sem þú vilt stíla. Hver stíll (declaration) er með eigindi (property) og gildi (value). Semikomman aðgreinir stílana.

Veljarinn (Selector) kemur á undann, síðan kemur slaufusvigi { því næst skipun (Declaration), sem aftur er skipt í eigindi (property) og gildi (value) sem eru aðskilin með tvípunkti : og loks öfugur slaufusvigi }

> Til að gera slaufusviga: { = Alt Gr takkinn + 7 og } = Alt Gr takinn + 0

![css selector](selector.gif)

Valtag (_selector_) bendir á HTML þáttinn (_element_) sem þú vilt stíla.

Hver skipun inniheldur eigindi og gildi.

Valtagið inniheldur eina eða fleiri skipanir sem eru aðgreindar með semikommum.

Margar CSS skipanir eru aðgreindar með semikommum og þær eru umvafðar með slaufusviga.

Dæmi:

```CSS

.header h1 {
    color: #fff;
    line-height: 1.2;
    font-weight: normal;
}

```

#### Stílsíða tengd við HTML vefsíðu

```HTML
    <!--link er í head taginu -->
    <link rel="stylesheet" type="text/css" href="styles.css">

```

### Bjargir

* [Verkefnalýsing 1](../)
* [HTML, sjá nánari umfjöllun](HTML-CSS/README.md)
* [CSS, sjá nánari umfjöllun](HTML-CSS/stylesheet.md)
* [Vefforitun bók, kafli 4](https://bok.vefforritun.is/04.element)