# Sveigjanleg hönnun vefs  (_Responsive Web Design_)
 
### Markmið:

Nemendur öðlast skilning á:

* hönnun svegjanlegs viðmóts vefsíðu (_Responsive Web Design_)
* hvernig hægt er að vinna með CSS _@media_ skipunina til að breyta skipulagi vefsíðu miðað við skjástærð 

Skipulag vefsíðu með mörgum dálkum gengur ekki upp í litlum farsímaskjáum. Til að hafa áhrif á skipulag HTML síðu setjum við inn viðmið (_breakpoints_) í CSS stílsíðuna.  Við notum **_@media screen_** skipunina til að birta mismunandi skipulag eftir skjástærðum.  

- [Kóðadæmi með viðmiðum (_@media & breakpoints_) ](Namsefni-4/README.md)

## 4.1 Sveigjanlegt dálkaskipulag, 1, 2, 4

Afritaðu _Verkefni 3.2_ yfir í nýja möppu t.d. **Verkefni-4.1** og gerðu vefsíðuna sveigjanlega.  <br>
Notaðu **_@media screen_** skipunina til að birta mismunandi skipulag eftir skjástærðum.

* Viðmið: 0 – 599px,
  * allir dálkar með 100% breidd (_grid-template-columns:(1fr);_)
* Viðmið: 48rem (768px – 959px)
  * 2 og 4 dálkar með 50% breidd (_grid-template-columns:(1fr 1fr);_)
* Viðmið: 60rem (960px - 1279px)
  * 3 dálkar 33.33% breidd (_grid-template-columns:repeat(3, 1fr);_)
* Viðmið: 80rem (1280px - 1599px)
  * 4 dálkar 25% breidd (_grid-template-columns:repeat(4, 1fr);_)
* Viðmið: 100rem (1600px)
  * Efni vefsíðunnar er miðjusett
 

- [Sýnidæmi 4.1](Namsefni-4/Dæmi41.md)

---

## 4.2 Sveigjanleg vefsíða með _"Grid-template-columns"_

Afritaðu eina vefsíðu og stílsíðu úr verkefni 3.3 og vistaðu í nýja möppu sem þú getur nefnt **verkefni-4.2**. 

Nú er komið að gera vefsíðuna sveigjanlega. Notaðu CSS Grid til að hanna eigið dálkaskipulag. Vefsíður þurfa að birtast í öllum helstu skjástærðum, búðu til viðmið (_breakpoint_) til að stjórna skipulagi vefsíðunnar í stílsíðunni. 

* Viðmið: 0 – 599px,
  * allir dálkar með 100% breidd (1fr)
  * í efnisyfirliti eru tenglar með _display:block_
* Viðmið: 37.5rem (600px)
  * Efnisyfirlit með _Flex direction: row;_
* Viðmið: 48rem (768px)
  * &lt;main> í einum dálki (_grid-template-columns:(1fr);_)
    * &lt;article> í einum dálk
    * &lt;section> með &lt;aside> í tveimur dálkum (_grid-template-columns:(1fr 1fr);_)
* Viðmið: 60rem (960px)
  * &lt;main> í tveimur dálkum (_grid-template-columns:(2fr 1fr);_)
  * &lt;section> með &lt;aside> í einum dálki (_grid-template-columns:(1fr);_)
* Viðmið: 80rem (1280px)
  * Efni vefsíðunnar er miðjusett

- [Sýnidæmi 4.2](Namsefni-4/Dæmi42.md)

## 4.3 Sveigjanleg vefsíða með _"Grid-template-area"_

Afritaðu vefsíðu 4.2 og stílsíðuna og notum **"grid template area** til að skipuleggja nýju vefsíðuna. 

> `aside` tögin eru tekin út úr `section` taginu, þannig að `article` og `aside` eru saman í `main` taginu.

Til að nota grid area verðum við að nefna klasa sem eru tengdir ákveðnum tögum og gefa þeim síðan _grid area_ staðsetningu td.

| HTML tag | CSS klasi | Grid area name |
| --- | --- | --- | 
| main | .main | grid-area: main |
| aside | .aside1 | grid-area: aside1 | 
| aside | .aside1 | grid-area: aside1 | 



* Viðmið: 0 – 599px,
  * efnisyfirlit er eins og í vefsíðu 4.1 
  * ```CSS
    main {
      display: grid;
      grid-template-areas: 
      "article"
      "aside1"
      "aside2";
    }
    ```

* Viðmið: 37.5rem (600px)
  * Efnisyfirlit með _Flex direction: row;_
* Viðmið: 48rem (768px)
  * ```CSS
    main {
      display: grid;
      grid-template-areas: 
      "article article"
      "aside1 aside2";
    }
    
```
  * &lt;main> í einum dálki (1fr)
    * &lt;article> í einum dálk
    * &lt;section> með &lt;aside> í tveimur dálkum (1fr 1fr)
* Viðmið: 60rem (960px)
  * &lt;main> í tveimur dálkum (2fr 1fr)
  * &lt;section> með &lt;aside> í einum dálki (1fr)
* Viðmið: 80rem (1280px)
  * Efni vefsíðunnar er miðjusett

---

### Lykilmatsþáttur

#### Tímaverkefni 20%

* **Vefsíða með viðmiðum**
    * Farsímar (_Mobile_): 0 – 37.5rem (600px)  _eins dálks hönnun_  
    * Spjaldtölvur (_Tablet_): 48rem (768px) _tveggja dálka hönnun_
    * Fartölvur (_Laptop_): 60rem (960px) _3 dálka hönnun_
    * Borðtölvur (_Desktop_): 80rem (1280px) _4 dálka hönnun_
    * Efni vefsíðunnar er miðjusett (_margin:auto;_) í stærri skjáum (100rem)
*  **Efnisyfirlit sveigjanlegt**
    * Efnisyfirlit (nav) á að vera svegjanlegt með _display:flex_

> Skil á verkefni 4 lokast þegar kennslutíma tímaverksefnisins er lokið

#### Einkunn verður birt í Innu

#### [Námsefni](https://github.com/vefgrunnur/24H-verkefni/tree/main/Verkefni-4/Namsefni-4)
