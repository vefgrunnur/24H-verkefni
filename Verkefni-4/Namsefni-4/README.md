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
@media only screen and (min-width: 600px) {  /* skjáir (screen) sem eru stærri en 600px */
	  body {
		background-color: blue;
		color:white;
	  }
} 
/* spjaldtölva, tablet */
@media only screen and (min-width: 768px) {  /* skjáir (screen) sem eru stærri en 768px */
	  body {
		background-color: lime;
		color: black;
	  }
}
/* Fartölva, laptop */
@media only screen and (min-width: 960px) {  /* skjáir (screen) sem eru stærri en 960px */
	  body {
		background-color: red;
		color: yellow;
	  }
}

/* Tölvuskjár, computer screen */
@media only screen and (min-width: 1280px) {  /* skjáir (screen) sem eru stærri en 1280px */
	body {
		max-width: 1280px;
		margin: 0 auto;
		border: 2px solid yellow;
	}
}

``` 

### Lesefni

- https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_grid_layout
- https://bok.vefforritun.is/18.skalanlegir
