# Tenglar í vefsíðu (_e. links_).

HTML – tög geta í flestum tilvikum haft viðbætur sem nota má til að stýra enn betur eðli
þeirra og gefa þeim aukna möguleika. Þessar viðbætur eru kallaðar á ensku _attributes_ sem
á íslensku gæti útlagst sem eigindi. Hverju eigindi fylgir svo ákveðið gildi _value_.

Til að tengjast öðrum vefsíðum þurfum við að útbúa svokallaðan tengil (link). Það er gert
með eftirfarandi hætti:

```HTML
<a href="http://www.tskoli.is"> Tækniskólinn </a>
```

Best er að brjóta þetta niður í eftirfarandi einingar:

**a** er skipun. **href=** er eigindi og `https://www.tskoli.is` er gildið, textinn sem birtist á vefsíðu er <a href="https://www.tskoli.is"> Tækniskólinn</a>

---

### Hulduklasar  _Pseudo-classes_

```CSS
    /* unvisited link */
    a:link {
        color: #FF0000;
    }

    /* visited link */
    a:visited {
        color: #00FF00;
    }

    /* mouse over link */
    a:hover {
        color: #FF00FF;
    }

    /* selected link */
    a:active {
        color: #0000FF;
    }
```

[Sjá nánar á w3schools](https://www.w3schools.com/css/css_pseudo_classes.asp)


---

![hulduklasar](images/v2.4.jpg)

### Bjargir

* [Verkefnalýsing 1](../../)
* [Námsefni 1](../)
* [HTML](README.md)
* [CSS](stylesheet.md)
* [Litir í vefsíðu](litir.md)
* [Yfirlit (_Cheat seets_)](https://cheatsheets.shecodes.io/)