# Sveigjanleg hönnun vefs  (_Responsive Web Design_)
 
### Markmið:

Nemendur öðlast skilning á:

* hönnun svegjanlegs viðmóts vefsíðu (_Responsive Web Design_)
* hvernig hægt er að vinna með CSS _@media_ skipunina til að breyta skipulagi vefsíðu miðað við skjástærð 

Skipulag vefsíðu með mörgum dálkum gengur ekki upp í litlum farsímaskjáum. Til að hafa áhrif á skipulag HTML síðu setjum við inn viðmið (_breakpoints_) í CSS stílsíðuna.  Við notum **_@media screen_** skipunina til að birta mismunandi skipulag eftir skjástærðum.  

- [Kóðadæmi með viðmiðum (_@media & breakpoints_) ](Namsefni-4/README.md)

## 4.1 Sveigjanlegt dálkaskipulag, 1, 2, 4

Afritaðu (_copy_) _Verkefni 3.2_ yfir í nýja möppu t.d. **Verkefni-4.1** og gerðu vefsíðuna sveigjanlega.  <br>
Notaðu **_@media screen_** skipunina til að birta mismunandi skipulag eftir skjástærðum.

* Viðmið: 0 – 599px,
  * allir dálkar með 100% breidd (1fr)
* Viðmið: 600px – 767px,
  * 2 og 4 dálkar með 50% breidd (1fr 1fr)
* Viðmið: 768px – 959px,
  * 2 dálkar 50% breidd (1fr 1fr),
  * 3 dálkar 33.33% breidd (1fr 1fr 1fr) 
  * 4 dálkar 25% breidd (4, 1fr)

- [Sýnidæmi 4.1](Namsefni-4/Dæmi41.md)

---

## 4.2 Sveigjanleg vefsíða

Afritaðu vefsíðu og stílsíðu sem þú gerðir í **Tímaverkefni 3.1** og vistaðu verkefnið í nýja möppu sem þú getur nefnt **verkefni-4.2**. 

Nú er komið að gera vefsíðuna sveigjanlega. Notaðu CSS Grid til að hanna eigið dálkaskipulag. Vefsíður þurfa að birtast í öllum helstu skjástærðum, búðu til viðmið (_breakpoint_) til að stjórna skipulagi vefsíðunnar í stílsíðunni. 

- [Sýnidæmi 4.2](Namsefni-4/Dæmi42.md)

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
