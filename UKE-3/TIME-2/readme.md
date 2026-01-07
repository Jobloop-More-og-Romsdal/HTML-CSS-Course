# FARGER, POSISJONER OG BAKGRUNNER
Vi skal nå bli kjent med ulike typer farger.

## FARGER
- `#`: HEX farger bruker seks hexadesimaler. #. De kan være hvilken som helst farge!
- `rgb()`: RGB farger bruker rgb(0-255, 0-255, 0-255). Veldig bra når du vet de eksakte RGB verdiene du trenger.
- `rgba(red, green, blue, alpha)`: RGBA farger, rgba(0-255, 0-255, 0-255, 0-1) lik RGB kan være hvilke som helst farge, og samtidig ha gjennomsiktighet!
- `hsla(hue, saturation%, lightness%, alpha)`: Lettere å endre farge, shading, styrken, og gjennomsiktigheten. Mens RGB/RGBA må du finne nye tall.
- `red/green/blue/etc...`: Standard navn mennesker ofte bruker for å referere til en spesiell farge. Enkel å huske, men kan ikke endres.

## POSISJONER
- position: static;
Alle elementer er alltid statisk hvis du ikke sier noe annet.
Elementet følger bare en 'normal flyt' på siden, altså at nettsiden oppfører seg som normalt, og tags som top, left, right, bottom har ingen effekt på denne.

- position: relative;
    -- top: 20px; 
    -- left: 20px;
    -- right: 20px;
    -- bottom: 20px;
Elementet har fortsatt en normal flyt, men top, left, right og bottom vil flytte elementet fra sin opprinnelige plass i forhold til seg selv og Plassen den opprinnelig hadde, er fortsatt reservert.

- position: fixed; 
    -- top: 0; 
    -- left: 0;
Elementet flytter seg ikke når du scroller
Posisjoneres i forhold til viewport (skjermen)
Brukes ofte til menyer, chat-knapper eller cookie-banner.
Eksempel: Vis posten.no sin nettside i inspect HTML
#posten-chatbot-button {
    position: fixed;
    bottom: 20px;
    right: 20px;
}

- position: sticky; 
    -- top: 0;
Kombinasjon av relative + fixed ved at det oppfører seg som en relative først.
For at denne skal funke må du ha enten top, left, right eller noen av de andre.
og ingen av Forelder elementene har overflow: hidden

Perfekt for menyer og overskrifter.

Når du scroller forbi et punkt → blir den fastlåst

## BAKGRUNNER
- background-color: #fff; - Setter en bakgrunnsfarge

- background-size: 
    - auto; Original størrelse, ingen skalering. Dette er standarden
    - cover; - Bakgrunnsbildet blir skalert for å dekke hele størrelsen på elementet den er i.
    - 200px 100px; 50% etc...; Manuell endring
    - contain; Brukes gjerne for logoer og ikoner hvor du må se alt og 'cropping' og endring i apsekt  ratio ikke er lov.

- background-image: url; setter bildet, enten med en ekstern eller intern link.

- background-repeat:
    - repeat; Standard. Bildet gjentas både horisontalt og vertikalt for å fylle hele elementet.
    - no-repeat; Bildet vises kun en gang, og gjentas ikke.

- background-attachment: fixed;


- background: #ff5733 url('image.jpg') no-repeat center center; DETTE ER KORTFORM. Da setter du alt i en enkelt regel :)

### <img>-tag vs Bakgrunnsbilde
   <img> brukes når bildet er en del av innholdet. Det gjør det lettere for Skjermlesere å forstå det og SEO (Search Engine Optimisation) kan bruke alt-teksten.

    Bakgrunnsbilde brukes når bildet er en dekorasjon eller bakgrunn, og det er ikke en del av det faktiske innholdet.







