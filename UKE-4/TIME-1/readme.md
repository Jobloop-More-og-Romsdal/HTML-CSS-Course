## FORM
<form>
  <!-- Input-felter kommer her -->
</form>

Viktige attributter:
action – hvor dataene sendes
method – hvordan dataene sendes (GET eller POST)

## INPUT
Tekstfelt
<input type="text" placeholder="Navn">
Passord
<input type="password" placeholder="Passord">
E-post
<input type="email" placeholder="E-post">

## LABEL
viktig for brukervennlighet (universiell utforming)

## SUBMIT (KNAPP/VS/INPUT)
#### Fordeler med <button></button>
Kan ha tekst, bilder, ikoner, emoji, styling med HTML inni CSS.
Enklere å style...
JavaScript kan ha egne id eller class og brukes i event listeners
<button type="submit"><span>Send</span> ✅</button>

### Fordeler med <input type="submit">
Simpelt og raskt å lage
Støttes av alle nettlesere. Gammeldags, men helt trygt
Litt mindre kode, og ingen closing tag
<input type="submit" value="Send">
(value er hva som står i knappen)