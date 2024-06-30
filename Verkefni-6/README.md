# Myndvinnsla og innsetning mynda í vefsíðu

### Markmið

Nemendur geta:

* unnið myndir fyrir vef í [myndvinnsluforriti](https://www.photopea.com/)
* látið myndir af sömu stærð raðast inn eftir skjástærð 
* notað &lt;picture> tagið til að birta stóra mynd sem vafrinn sækir eftir skjástærð 

![Octocat](github-octocat.svg)

#### Meðfylgjandi verkefnalýsingunni eru tvær .zip skrár

* [Vefsíða og stílsíða](Namsefni-6/demosite.zip)  
* [Myndir](Namsefni-6/originals.zip)

.zip skrárnar hleður þú á tölvuna þína. Myndirnar á að setja í vefsíðuna, en fyrst þarf að breyta stærð myndanna í myndvinnsluforriti þannig að þær í réttri stærð og fljótar að hlaðast inn á vefsíðuna. 

- Um er að ræða eina stóra mynd á forsíðu sem þarf að vera í fjórum mismunandi stærðum. 
- Myndin er síðan sótt inn á vefsíðuna í ` picture ` taginu.
- Mynd af Freysteini er með bakgrunn sem þarf að taka út og bakgrunnurinn gerður gegnsær (_transparent_). 
- Síðan eru 6 myndir sem eiga allar að vera í sömu stærð og þær eiga síðan að birtast eftir skjástærð þrjár í röð, síðan tvær í röð og í einum dálki í farsímaskjáum. 

1. **Stór forsíðumynd**
    * Myndin er vistuð í fjórum stærðum og vafrinn velur rétta stærð miðað breidd skjásins. 
    * Viðmið: [0 - 767px] – [768px - 960px] – [960px - 1280px] – [1280px - 2000px]
    * Með &lt;picture> taginu í vefsíðu er hægt að sortera myndir eftir breidd skjásins
    * [Forsíðumynd](myndir/mynd1.jpg)
1. **Mynd með gagnsæjum (_transparent_) bakgrunni**
    * Hreinsið út bakgrunn úr mynd í myndvinnsluforriti 
    * [Mynd með gagnsæjum bakgrunni](myndir/mynd2.jpg)
1. **Myndaröð** 
    * 6 myndir eru vistaðar í sömu stærð  (500 x 500px) og þeim raðað mismunandi upp í vefsíðu eftir breidd skjásins
    * [Myndaröð](myndir/mynd3.jpg)

* Vefmyndir geta verið þjappaðar saman í .jpg (kb) sem er langmest notað í vefsíðum. 
* Myndir í .png formati geta verið með gagnsæjan bakgrunn og ~ 25% þjöppun
* Myndir í .gif formati geta verið með gagnsæjan bakgrunn en með 0% þjöppun

**[Photopea](https://www.photopea.com/)** er myndvinnsluforrit (_app_) sem keyrir í vafra.

* Myndir skornar:  _Toolbar -> Crop Tool_
* Myndir settar í rétta stærð: _Image -> Canvas size_.
* Þjöppun fyrir vef  í Photopea  -> _Export -> .jpg eða .png_
    
Myndir sem settar eru á vefsíðu eiga ekki að vera breiðari en ramminn sem myndin birtist í. En nú getur stærð rammans verið mismunandi og þá er mikilvægt að **hafa eftirfarandi grunnstillingu á img taginu í stílsíðu** 

```CSS
        img { 
            max-width:100%;
            height: auto;
        }
```

#### Æfingaverkefni 5%

1. **Stór forsíðumynd 2%**
    * Myndin er vistuð í fjórum stærðum og vafrinn velur rétta stærð miðað breidd skjásins. 
    * Viðmið: [0 - 767px] – [768px - 960px] – [960px - 1280px] – [1280px - 2000px]
1. **Myndaröð – 6 myndir 2%**
    * 1 mynd: [0 - 768px] – 2 myndir: [768px - 960px] – 3 myndir: [960px - 1600px] – miðjusett: (max-width 1600px)
1. **Mynd með gegnsæjum bakgrunni	(_.png_) 1%**

#### Tímaverkefni 10%

> Skil á verkefni 6 lokast þegar síðasta kennslutíma verkefnisins er lokið

Skilaðu öllum vinnugögnum sem tilheyra verkefninu í **Innu/VEFÞ1VG/Verkefni 6**. 

#### Einkunn verður birt í Innu

---

### Bjargir

[How To Use Photopea 2024 (Tutorial for Beginner Designers)](https://www.youtube.com/watch?v=JIdvvG9ZX7c)

