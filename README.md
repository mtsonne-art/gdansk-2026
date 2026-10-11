# Gdańsk 2026

Side til Ove og Evas tur til Gdańsk (sidst i november / start december 2026) og deres fødselsdagsgave. Bygget som Drengetur 2027: én `index.html` uden server, klar til Netlify.

## Sådan udfylder du informationen

Alt står i `<script>`-blokken øverst i `index.html` under **DATA – RET HER**:

- `TRIP` – afrejse- og hjemrejsedato (sat til 29/11–3/12 2026). Giver nedtælling og antal nætter.
- `FLIGHTS` – ud- og hjemrejse (Wizz Air W6 1778 / W6 1777). Udfyld `dep`/`arr` med tiderne fra bookingen – så forsvinder den forventede tid.
- `BOOKING_REF` – bookingnummer for flyene.
- `HOTEL` – navn, adresse, telefon, link, ind-/udtjekning, bookingnummer. Sæt `lat`/`lon` (fra Google Maps), så kommer hotellet på kortet, og gåafstande regnes fra hotellet.
- `GIFT` – restaurantens navn, dato, tid, adresse, link og en tekst. Hilsenen (`greeting`) kan rettes.

Julemarkedets datoer og tider står i `MARKET`, rav-afsnittet i `AMBER`, og gaderne på kortet i `ROADS` (tegnet i hånden, ikke målfast).

Tomme felter vises som "Udfyldes snart".

## Fødselsdagsgaven

Første gang man åbner "Fødselsdagsgave", kommer der fyrværkeri og danske flag. Det huskes i browseren (localStorage `gdk-gave-aabnet`), så næste gang vises gaven direkte. Der er en knap til at se fyrværkeriet igen. Vil du teste "første gang" igen, så åbn siden i et privat vindue.

## Ikke offentlig

Siden har `noindex` (meta-tag, `X-Robots-Tag` og `robots.txt`), så søgemaskiner ikke viser den. En Netlify-adresse kan dog åbnes af alle, der kender linket.
