# VAJA-2-Modeliranje-z-UML

Ta diagram, ki predstavlja Load Balancer (Izravnalnik obremenitve) je poenostavljen primer v okolju Docker.

Uporabnik in Zunanji sistem sta zunanja akterja, ki sodelujeta z izravnalnikom obremenitve.
Load Balancer predstavlja sistem za izravnavo obremenitve, ki omogoča več primerov uporabe oz. funkcionalnosti:
  - Balance Load: ponazarja funkcijo uravnoteženja obremenitve, ki vključuje spremljanje strežnikov.
  - Upravljanje konfiguracije: predstavlja zmožnost konfiguriranja izravnalnika obremenitve.
  - Spremljanje strežnikov: označuje funkcijo nadzora strežnika.
  - Preusmeri promet: ponazarja možnost preusmeritve prometa.
  - Autentifikacija uporabnikov: predstavlja preverjanje pristnosti uporabnikov, ki je morda potrebno za določene konfiguracije.

Akterji in primer uporabe:
  - Uporabnik pošilja zahtevke na Uravnoteženje obremenitve, Upravljanje konfiguraci pa konfigurira Uravnoteženje obremenitve.
  - Preusmeri promet zahteva Autenifikacijo uporabnika
