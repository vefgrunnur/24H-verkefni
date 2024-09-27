# Svegjanleg hönnun

### Viðmið (_Breakpoints_) - "_Mobile up_"

```CSS

/* Fyrst koma stílar sem gilda í öllum skjástærðum ss. leturgerð og litir */
/* Farsími lóðrétt, Molile vertical */

body {
	font-family: sans-serif;
	background-color: lightblue;
	color: darkblue;
}
/* Farsími lárétt, Mobile Horisontal */
@media only screen and (min-width: 37.5rem) {  /* skjáir (screen) sem eru stærri en 600px */
	  body {
		background-color: blue;
		color:white;
	  }
} 
/* spjaldtölva, tablet */
@media only screen and (min-width: 48rem) {  /* skjáir (screen) sem eru stærri en 768px */
	  body {
		background-color: black;
		color: lime;
	  }
}
/* Fartölva, laptop */
@media only screen and (min-width: 60rem) {  /* skjáir (screen) sem eru stærri en 960px */
	  body {
		background-color: red;
		color: yellow;
	  }
}

/* Tölvuskjár, computer screen */
@media only screen and (min-width: 80rem) {  /* skjáir (screen) sem eru stærri en 1280px */
	body {
		max-width: 76rem; /* 4rem spássía */
		margin: 0 auto;  /* efni body miðjusett */ 
	}
}

``` 

### Grid svæðaskipulag

- https://bok.vefforritun.is/18.skalanlegir
- https://bok.vefforritun.is/21.grid#20.4.2

