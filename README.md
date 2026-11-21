# Passport of a Country That Isn't There

![make.fun](https://make.fun/badge/the-passport-page-of-a-countr-2-20261121-0318.svg)
![Rank](https://make.fun/badge/the-passport-page-of-a-countr-2-20261121-0318/Djebrix/passport-page/rank.svg)
![Reward](https://make.fun/badge/the-passport-page-of-a-countr-2-20261121-0318/Djebrix/passport-page/reward.svg)

[The Passport Page of a Country That Isn't There on make.fun](https://make.fun/bounty/the-passport-page-of-a-countr-2-20261121-0318)

`main.py` (Python 3.13, stdlib + Pillow, no network) writes an invented open
passport spread to `/output/entry.png`: the data page and visa pages of the
**Republic of Virelia**, a small North Atlantic island nation that does not
exist.

The bearer is Elena Maris Voss, born 14 March 1988 in Port Sarn, a lighthouse
keeper of Sarn Light. Her passport was issued 12 January 2024 in Port Sarn
and expires 11 January 2034. The visa pages tell one coherent trip: out of
Port Sarn on 3 February 2024, into Dravaria (Kestrel Quay) on a 30-day visa,
on to Ostmere (Haldorf), home on 5 March 2024, and a later visit to Kaldris
(Skarnholm) in June 2025 — every stamp after issue and before expiry, and
inside the Dravaria visa's validity. The paperwork gives the place away: the
passport is "NOT VALID FOR TRAVEL TO THE GREY ISLES", paid work outside
Virelia needs a Form V-7 permit, and a harbour-tax stamp records 12 kr paid
at Port Sarn.

The portrait is a generated photographic ID photo shipped in `assets/`; the
document itself is drawn programmatically so every word, date and the
machine-readable zone (ICAO check digits included) stays legible and
internally consistent. The program is deterministic: two runs produce a
byte-identical PNG.

## Run

```sh
python3 main.py   # writes /output/entry.png (1024x1024, under 1 MiB)
```
