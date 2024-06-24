# Sveigjanleg hönnun vefs  (_Responsive Web Design_)
 
### Markmið:

Nemendur öðlast skilning á:

* hönnun svegjanlegs viðmóts vefsíðu (_Responsive Web Design_)
* hvernig hægt er að vinna með CSS _@media_ skipunina til að breyta skipulagi vefsíðu miðað við skjástærð 

Skipulag vefsíðu með mörgum dálkum gengur ekki upp í litlum farsímaskjáum. Til að hafa áhrif á skipulag HTML síðu setjum við inn viðmið (_breakpoints_) í CSS stílsíðuna.  Við notum **_@media screen_** skipunina til að birta mismunandi skipulag eftir skjástærðum.  

#### [Sýnidæmi](Namsefni-4#vi%C3%B0mi%C3%B0-breakpoints---mobile-up)

## 4.1 Sveigjanlegt dálkaskipulag, 1, 2, 4

Afritaðu (_copy_) _Verkefni 3.2_ yfir í nýja möppu t.d. **Verkefni-4.1** og gerðu vefsíðuna sveigjanlega.  Notaðu **_@media screen_** skipunina til að birta mismunandi skipulag eftir skjástærðum.

* Viðmið: 0 – 599px,
  * allir dálkar með 100% breidd (1fr)
* Viðmið: 600px – 767px,
  * 2 og 4 dálkar með 50% breidd (1fr 1fr)
* Viðmið: 768px – 959px,
  * 2 dálkar 50% breidd (1fr 1fr),
  * 3 dálkar 33.33% breidd (1fr 1fr 1fr) 
  * 4 dálkar 25% breidd (4, 1fr)

#### [Sýnidæmi 4.1](Namsefni-4/Dæmi41.md)

---

## 4.2 Sveigjanleg vefsíða

Afritaðu vefsíðu og stílsíðu sem þú gerðir í **Tímaverkefni 3.1** og vistaðu verkefnið í nýja möppu sem þú getur nefnt **verkefni-4.2**. 

Nú er komið að gera vefsíðuna sveigjanlega. Notaðu CSS Grid til að hanna eigið dálkaskipulag. Vefsíður þurfa að birtast í öllum helstu skjástærðum, búðu til viðmið (_breakpoint_) til að stjórna skipulagi vefsíðunnar í stílsíðunni. 

#### [Sýnidæmi 4.2](Namsefni-4/Dæmi42.md)

---

### Lykilmatsþáttur

#### Æfingaverkefni 5%

* **2% 4.1 Viðmið 2, 3 og 4 dálkum**
    * 0 – 767px. Allir dálkar skiptast í einn dálk (1fr)
    * 768px. 2 og 4 dálkar skiptast í 2 dálka (1fr 1fr)
    * 960px – + (Allir dálkar skiptast rétt, 2, 3 og 4 dálkar)
* **2% 4.2.1 Vefsíða með viðmiðum**
    * Mobile: 0 – 599px  _eins dálks hönnun_  
    * Tablet: 600px – 767px _tveggja dálka hönnun_
    * Desktop: 768px – 959px _3 eða 4 + dálka hönnun_
    * 960px + Efni vefsíðunnar er miðjusett (_max-width_) í vafranum
*  **1% 4.2.2 Valmynd sveigjanleg**
    * Valmynd (nav) skal vera svegjanleg (_display:flex_)

#### Tímaverkefni 15%

> Skil á verkefni 3 lokast þegar síðasta kennslutíma verkefnisins er lokið

#### Einkunn verður birt í Innu

_Gangi þér vel_
