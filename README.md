# Aangepaste Promo Sectie voor Shopify

Deze Shopify-sectie toont een promotiebanner met productafbeeldingen, een knop, en een productbadge. De sectie is responsive en bevat een Swiper-carousel voor mobiele weergave.

Bekijk de sectie live op de volgende pagina:

[https://esmeetestdigifist.myshopify.com/?_ab=0&_fd=0&_sc=1](https://esmeetestdigifist.myshopify.com/?_ab=0&_fd=0&_sc=1)

**Wachtwoord**: esmeevanleeuwen

## Functies

- **Responsive Design**: Past zich aan voor zowel desktop als mobiel (met een carousel op mobiel).
- **Productbadge**: Bevat productnaam, prijs en een kleine afbeelding.
- **Eenvoudig te bewerken**: Tekst, afbeeldingen en productinformatie zijn te wijzigen via de Shopify-editor.

## Installatie

1. **Liquid-bestand toevoegen**:
   - Ga naar **Online Store** > **Themes** > **Edit Code**.
   - Voeg een nieuw sectie-bestand toe en plak de Liquid-code.

2. **Swiper CSS en JS** toevoegen:
   Voeg de volgende links toe aan de sectie of `theme.liquid`:

    ```html
    <link rel="stylesheet" href="https://unpkg.com/swiper/swiper-bundle.min.css">
    <script src="https://unpkg.com/swiper/swiper-bundle.min.js"></script>
    ```

## Gebruik

1. **Desktopweergave**:
   - Links: Tekst met een kop, knop en beschrijving.
   - Rechts: Productafbeelding met overlay badge voor productinformatie.

2. **Mobiele weergave**:
   - Swiper-carousel met navigatieknoppen en afbeeldingen.

## Aanpasbare Instellingen

In de Shopify-editor kun je de volgende items aanpassen:

- **Koptekst**
- **Afbeelding links en rechts**
- **Productnaam en prijs**
- **Productafbeelding in de badge**

## Swiper Initialisatie

```javascript
document.addEventListener('DOMContentLoaded', function () {
    var swiper = new Swiper('.swiper-container', {
        loop: true,
        pagination: false,
        navigation: {
            nextEl: '.swiper-button-next',
            prevEl: '.swiper-button-prev',
        },
        slidesPerView: 1,
        spaceBetween: 10,
    });
});
