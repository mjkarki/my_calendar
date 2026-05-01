# Kalenterisovellus

Single Page Application (HTML5, CSS, JavaScript) ilman ulkoisia riippuvuuksia.

## Ominaisuudet

- Kuluvan kuukauden näkymä ruudukkona
- Jokainen rivi alkaa viikon numerolla (ISO-viikonumero)
- Eurooppalainen viikkojärjestys: viikko alkaa **maanantaista**, päättyy sunnuntaihin
- Navigointi:
  - Edellinen / seuraava kuukausi
  - Edellinen / seuraava vuosi
  - "Tänään" -painike palauttaa nykyiseen kuukauteen
- Nykyinen päivä korostettu
- Muut kuukaudet näkyvät vaaleampana
- Responsiivinen (mobiili & työpöytä)

## Kehitysistunto

### Alkuperäinen tavoite
Luo kalenterisovellus, joka näyttää kuluvan kuukauden ruudukkona, jossa:
- Jokainen ruudukon rivi alkaa viikon numerolla
- Päivät eurooppalaisessa järjestyksessä (ma-su)
- Mahdollisuus siirtyä edelliseen tai seuraavaan kuukauteen ja vuoteen

### Tehdyt muokkaukset

| Pyyntö | Muutos |
|--------|--------|
| Rivikorkeus kavennettu 20% | `aspect-ratio: 1` → `1.25` |
| Sininen väri → vaalea violetti | `#0066cc` → `#b19cd9` |
| Soluille reunus | `border: 1px solid #e0e0e0` |
| Reunuksen väri vaalennettu 20% | `#e0e0e0` → `#e6e6e6` |
| Solujen pyöristys poistettu | `border-radius` poistettu |
| Sarakkeiden kaksoisreunus korjattu | `border-right` vain joka 8. solulta |
| Violetin sävy punaisemmaksi | `#b19cd9` → `#c99cd9` |
| Rivikorkeus suhteeksi 1:0.5 | `aspect-ratio: 2` |

## Käyttö

Avaa `index.html` selaimessa.

### Pikanäppäimet
- **Ctrl + ←** – Edellinen kuukausi
- **Ctrl + →** – Seuraava kuukausi  
- **Alt + ←** – Edellinen vuosi
- **Alt + →** – Seuraava vuosi
- **Home** – Siirry tänään
