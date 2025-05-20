# Simulacija rezervacije stolova u restoranu

Ovaj program simulira rezervaciju stolova u restoranu pomoću višedretvenog programa u C-u. Za međusobno isključivanje u kritičnom odsječku koristi se **Lamportov algoritam**.

---

## Opis

- Program prima dva argumenta naredbenog retka:
  - Broj dretvi (klijenata koji rezerviraju stolove)
  - Broj stolova u restoranu
- Svaka dretva svakih 1 sekundu nasumično bira stol.
- Dretva ulazi u kritični odsječak koristeći Lamportov algoritam i pokušava rezervirati odabrani stol.
- Ako je stol slobodan, dretva ga rezervira; inače, rezervacija ne uspijeva.
- Program završava kada su svi stolovi rezervirani.

---

## Kako koristiti

### Kompajliranje

gcc -pthread -o program main.c
