<!-- De instructie vind je in: [docs/INSTRUCTIONS.md](docs/INSTRUCTIONS.md) -->

# De Buurtcampus - Detailpagina V2.0
<!-- Geef je project een titel en schrijf in één zin wat het is -->

Net als in mijn vorige project, [all-human-accessible-website](https://github.com/itsValyria/all-human-accessible-website), heb ik voor deze opdracht een detailpagina gemaakt van het buurtplatform waar De Hallen op zoek naar is.

Deze opdracht is gebaseerd op de volgende **user story**: <br>
```Als buurtbewoner van Amsterdam West wil ik meer informatie over een initiatief kunnen bekijken, zodat ik kan zien of ik mij bij het initiatief wil aansluiten.```

## Beschrijving
<!-- In de Beschrijving staat hoe je project er uit ziet, hoe het werkt en wat je er mee kan. -->
<!-- Voeg een mooie poster visual toe 📸 -->
<!-- Voeg een link toe naar Github Pages 🌐-->
!TODO Poster visual <br>
!TODO Poster visual comparison

Zoals al kort beschreven hierboven, is deze website een versie 2.0 van mijn eerder gemaakte opdracht [all-human-accessible-website](https://github.com/itsValyria/all-human-accessible-website). 

Deze pagina was nodig zodat mensen meer informatie kunnen zien van een buurtinitiatief, om te besluiten of ze zich willen aansluiten. Ook kunnen ze via Google maps gelijk de locatie zien, zodat ze weten waar het is en of het bereikbaar is voor hen. Verder staan er ook contactgegevens van de initiatieven voor als er vragen zijn.

Ik ben aan een tweede versie begonnen omdat wij nu met een [style guide](https://github.com/itsValyria/look-and-feel-living-styleguide) werken, en ik de veranderingen wilde toepassen, samen met een nieuwe lay-out.

Benieuwd naar het eindresultaat? Klik [hier](https://itsvalyria.github.io/look-and-feel-corporate-identity/)!

## Kenmerken
<!-- Bij Kenmerken staat welke technieken zijn gebruikt en hoe. Wat is de HTML structuur? Wat zijn de belangrijkste dingen in CSS? Wat is er met Javascript gedaan en hoe? Misschien heb je een framwork of library gebruikt? -->

Deze web pagina maakt gebruik van verschillende fundamentele principes op het web, namelijk **HTML**, **CSS** en **JavaScript**.

**Mobile First CSS**
Ik heb deze site mobile first gebouwd, wat inhoudt dat ik eerst het design voor de mobiel ben gaan bouwen, en dit daarna door middel van CSS omgezet heb naar een volledig responsive web page.
Hieronder kun je zien welke **Media Queries** ik heb gebruikt om deze site responsive te maken.

```css
/* Size M Device - Tablet */

@media (min-width: 768px) and (max-width: 1023px) {}

/* Size L-XL Device - Laptop-Desktop */

@media (min-width: 1024px) {}
```

**JavaScript**

Ook heb ik mijn eerste 'hamburger menu' gebouwd, ook wel een uitklapmenu. Dit is fijn voor de overzichtelijkheid, met name op mobiel en tablet. 
Door op een knopje te klikken, word er een extra class toegevoegd aan de navigatie bar waardoor deze visible wordt.

```js
window.addEventListener('load', () => {
    const ham = document.querySelector('.header__icon');
    const nav = document.querySelector('.header__nav');

    ham.addEventListener('click', () => {
        nav.classList.toggle('header__nav--visible');
    });
});
```
```css
.header__nav--visible {
  max-height: 20vh;
}
```

## Licentie

This project is licensed under the terms of the [MIT license](./LICENSE).
