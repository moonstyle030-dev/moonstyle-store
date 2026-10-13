# MOONSTYLE — Premium Streetwear Store

Dit is een mobile-first, premium static e-commerce prototype voor MOONSTYLE.

## Bestanden
- index.html — complete storefront
- styles.css — responsive design system
- script.js — filters, cart, newsletter popup, search, size guide
- privacy.html / terms.html — concept privacybeleid en algemene voorwaarden
- 404.html — aangepaste niet-gevonden-pagina
- robots.txt / sitemap.xml — zoekmachinebestanden
- assets/ — aangeleverde productfoto's en MOONSTYLE-logo

## Shopify
De productkaarten laten eerst de klant een maat kiezen. `script.js` koppelt de
gekozen kleur- en maatcombinatie aan een Shopify-variant en stuurt de volledige
winkelwagen naar de Shopify-checkout via een Shopify-cart permalink.

De Shopify-catalogus bevat drie producten (hoodie, broek en complete set), elk
met vijf kleuren en de maten XS–2XL. Voorraadtracking staat uit. De variant-ID's
en winkel-URL in `script.js` zijn specifiek voor de MOONSTYLE Shopify-winkel.
Pas ze aan als je producten, varianten of Shopify-winkel veranderen.

Voor live bestellingen moet in Shopify ook de checkout, verzendtarieven,
belastingen en betaalprovider correct zijn ingesteld. Test een bestelling eerst
met Shopify's testmodus voordat je de website breed publiceert.

## Klantaccounts
De storefront toont geen inlog- of registratielinks. Shopify-klantaccounts blijven
beschikbaar via Shopify's beveiligde accountpagina en checkout.

## Websiteverbeteringen
- De storefront en juridische pagina's hebben beschrijvende meta-omschrijvingen, canonical URLs en social-preview metadata.
- Het MOONSTYLE-logo wordt gebruikt als favicon en tijdelijke social-previewafbeelding.
- Productafbeeldingen onder de hero worden lazy-loaded en asynchroon gedecodeerd.
- De website biedt een browseropslagmelding; analytics en advertentietrackers zijn uitgeschakeld.
- De FAQ-link werkt, afbeeldingen hebben alt-tekst en de nieuwsbriefvelden controleren invoer.
- De formulieren zijn nog niet gekoppeld aan een nieuwsbriefbackend: adressen worden niet verzonden en er wordt geen kortingscode uitgegeven. De honeypot is alleen een basisfilter; echte spambeveiliging vereist server-side verwerking.
- `privacy.html` en `terms.html` zijn concepten. Vul de echte juridische verkopersgegevens, leverings- en retourvoorwaarden in en laat ze controleren voordat je verkoopt.
- De productafbeeldingen zijn al relatief klein; de onderstaande-lui laadstrategie verbetert de initiële paginalading. Een aparte compressie/export kan later nog extra besparen.
- GitHub Pages wordt via HTTPS gepubliceerd. Houd in de repository-instellingen **Enforce HTTPS** ingeschakeld.

## Beveiliging en analytics
Er zijn geen privé-API-sleutels nodig in de frontend. Shopify-domeinen en variant-ID's in JavaScript zijn publieke verwijzingen, geen wachtwoorden. Zet nooit geheime tokens, wachtwoorden of betaalgegevens in openbare HTML, CSS, JavaScript of GitHub-bestanden.
Analytics zijn niet ingesteld: er is geen provider of tracking-ID opgegeven. Voeg pas analytics toe nadat een provider is gekozen en de privacy- en toestemmingsinformatie daarmee overeenkomt.

## Live zetten
Upload de bestanden naar je hosting of Vercel/Netlify. Voor productie:
1. Vervang de voorbeeldmaten door de echte maattabel.
2. Voeg echte productprijzen/SKU's toe.
3. Koppel Shopify checkout.
4. Vervang Instagram/TikTok placeholders door de echte accounts.
5. Vul `privacy.html` en `terms.html` aan met de definitieve juridische verkopers-, verzend- en retourgegevens en laat ze controleren.

De productfoto's in `assets/` zijn de door jou aangeleverde afbeeldingen.


## Added products
- Moon Zip — Grey
- Moon Zip — Brown
- Moon Zip — Cream
- Moon Zip — Beige
- Moon - pants Grey
- Moon - pants Brown
- Moon - pants Cream
- Moon - pants beige

## Matching outfits
- Grey, Brown, Cream, Beige, and Black complete sets use their dedicated outfit photos.
- Each matching outfit is listed as a separate product and priced at €50.

The four supplied product images are stored in `assets/moon-zip-*.jpg`.
