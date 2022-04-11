#Estructura de una pagina simple
Tutorial para el desarrollo de una pagina web simple, desde la estructura de las carpetas asi como guias de codificación.

**Table of Contents**
[TOC]

## :file_folder: Estructura de directorio
---------------			
* :open_file_folder: App
  * :open_file_folder: assets
    * :open_file_folder: css
    * :open_file_folder: img
    * :open_file_folder: js
  * :page_facing_up: index.html

## :zap: Archivo index.html
### Navbar
```html
<header class="header" id="header">
  <nav class="nav container">
    <a class="nav__logo">Logo</a>
    <div class="nav__menu">
      <ul class="nav__list">
        <li class="nav__item">Home </li>
        <li class="nav__item">Page 1 </li>
        <li class="nav__item">Page 2 </li>
      </ul>
    </div>
    <div class="nav__btns">
      <div class="nav__changebg"></div>
      <!-- Responsive -->
      <div class="toggle"></div>
    </div>
  </nav>
</header>
```
### Body
``` html
<main id="main">
  <section> Seccion 1</section>
  <section> Seccion 2</section>
  <section> Seccion 3</section>
</main>
```

## :zap: Estructura CSS
#### Variables globales
```css
/* VARIABLES CSS  */

:root {
	--header-height: 3rem;

	/* Colors */
	--hue-color: 250;

	/* HSL color mode */
	--first-color: hsl(var(--hue-color), 69%, 61%);
	--first-color-second: hsl(var(--hue-color), 69%, 61%);
	--first-color-alt: hsl(var(--hue-color), 57%, 53%);
	--first-color-lighter: hsl(var(--hue-color), 92%, 85%);
	--title-color: hsl(var(--hue-color), 8%, 15%);
	--text-color: hsl(var(--hue-color), 8%, 45%);
	--text-color-light: hsl(var(--hue-color), 8%, 65%);
	--input-color: hsl(var(--hue-color), 70%, 96%);
	--body-color: hsl(var(--hue-color), 60%, 99%);
	--container-color: #fff;
	--scroll-bar-color: hsl(var(--hue-color), 12%, 90%);
	--scroll-thumb-color: hsl(var(--hue-color), 12%, 80%);

	/* Font and typography */
	--body-font: "Poppins", sans-serif;

	/* .5rem = 8px, 1rem = 16px, 1.5rem = 24px */
	--big-font-size: 2rem;
	--h1-font-size: 1.5rem;
	--h2-font-size: 1.25rem;
	--h3-font-size: 1.125rem;
	--normal-font-size: 0.938rem;
	--small-font-size: 0.813rem;
	--smaller-font-size: 0.75rem;

	/* Font weight */
	--font-medium: 500;
	--font-semi-bold: 600;

	/* Margenes Bottom */
	--mb-0-25: 0.25rem;
	--mb-0-5: 0.5rem;
	--mb-0-75: 0.75rem;
	--mb-1: 1rem;
	--mb-1-5: 1rem;
	--mb-2: 2rem;
	--mb-2-5: 2.5rem;
	--mb-3: 3rem;

	/* z-index */
	--z-tooltip: 10;
	--z-fixed: 100;
	--z-modal: 1000;
}
/* Variables Dat theme */

body.dark-theme{
	/* HSL color mode */
	--first-color-second: hsl(var(--hue-color), 30%%, 8%);
	--title-color: hsl(var(--hue-color), 8%, 95%);
	--text-color: hsl(var(--hue-color), 8%, 75%);
	--input-color: hsl(var(--hue-color), 29%, 16%);
	--body-color: hsl(var(--hue-color), 28%, 12%);
	--container-color: hsl(var(--hue-color), 29%, 16%);

	--scroll-bar-color: hsl(var(--hue-color), 12%, 48%);
	--scroll-thumb-color: hsl(var(--hue-color), 12%, 36%);
}

/* font size for large devices */
@media screen and (min-width: 968px) {
	:root {
		--big-font-size: 3rem;
		--h1-font-size: 2.25rem;
		--h2-font-size: 1.5rem;
		--h3-font-size: 1.25rem;
		--normal-font-size: 1rem;
		--small-font-size: 0.875rem;
		--smaller-font-size: 0.812rem;
	}
}
```
### Configuracion base
``` css
/* Base */
* {
	box-sizing: border-box;
	padding: 0;
	margin: 0;
}
html {
	scroll-behavior: smooth;
}
body {
	margin: 0 0 var(--header-height) 0;
	font-family: var(--body-font);
	font-size: var(--normal-font-size);
	background-color: var(--body-color);
	color: var(--text-color);
}
h1,
h2,
h3,
h4 {
	color: var(--title-color);
	font-weight: var(--font-semi-bold);
}
ul {
	list-style: none;
}
a {
	text-decoration: none;
}
img {
	max-width: 100%;
	height: auto;
}
```
### Responsive
#### :computer: Large
```css
/* For Large devices */
@media screen and (min-width:1024px) {
  #code
}
```
#### :computer: Large
```css
  /* For Large devices */
@media screen and (min-width: 768px) {
  #code
}
```
#### :computer: Medium
```css
  /* For Medium devices */
@media screen and (min-width: 568px) {
  #code
}
```
#### :iphone: Small
```css
/* For small devices */
@media screen and (max-width: 350px) {
  #code
}
```