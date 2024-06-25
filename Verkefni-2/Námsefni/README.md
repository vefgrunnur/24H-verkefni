# Box módelið

![box model](images/box-model.png)

Útskýring:

- Content - Innihald kassans, þar sem texti og myndir birtast
- Padding - Autt svæði í kringum innihald. Bilið er gegnsætt
- Border - Rammi utanum bil og innihald
- Margin - Spássía utan rammans, spássían er gegnsæ

## Block-level Elements

Blokk eining byrjar alltaf á nýrri línu og tekur upp alla breidd sem til er (100% breidd).

```HTML
<h1> - <h6> | <p> | <header>| <main> | <aside> | <article>  | <footer> | <form> | <section> | <div>
```

## Inline Elements

**&lt;span>** fellur td. inní textalínu. ekki hægt að setja gildi á bil (padding) ofan og neðan við (_top + bottom_) en virðir hliðarbil (_left + right_) 

```HTML

<span> | <a> | <img> 

```

## Display eigindið

```CSS

.daemi1 {display: none;}
.daemi2 {display: inline;}
.daemi3 {display: block;}
.daemi4 {display: inline-block;}

```

**display: none;** er almennt notað með JavaScript til að fela og sýna þætti án þess að eyða þeim og endurskapa þá.

The &lt;script> element uses display: none; as default. 

Heimild: 
* https://www.w3schools.com/css/css_boxmodel.asp
* https://www.w3schools.com/cssref/pr_class_display.asp

## Float

* https://www.w3schools.com/cssref/pr_class_float.php

## Flexbox

* https://www.w3schools.com/css/css3_flexbox.asp


#### Gildum hlaðið á eigindi 

```CSS

div {
	margin: 10px 20px 30px 40px; 
	   /*-top(1) -right(2) -bottom(3) -left(4) 
	   á bæði við margin og padding */
	
	padding: 10px 20px; 
		/*top+bottom og left+right 
		á bæði við margin og padding */
	
	border: 5px solid #f0f; 
	        /*-weight, -style, -color */
	/* 7 gildi eru í border-style: solid, dotted, dashed, double, ridge, inset, outset,*/
	/*ath! að veja aðeins eitt gildi á border-style:*/
}

```

#### Yfirlit

* [Verkefnalýsing 2](../../)
* [Námsefni 2](../)
* [Tenglar (links)](tenglar.md)