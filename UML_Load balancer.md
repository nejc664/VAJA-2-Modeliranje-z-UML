@startuml

actor "Uporabnik" as User
actor "Zunanji sistem" as System

rectangle "Load Balancer" {
  usecase (Uravnoteženje obremenitve) as UC1
  usecase (Upravljanje konfiguracije) as UC2
  usecase (Spremljanje strežnikov) as UC3
  usecase (Preusmerjanje prometa) as UC4
  usecase (Avtenifikacija uporabnikov) as UC5
}

User --> UC1 : Pošilja zahtevke
System --> UC4 : Pošilja zahtevke

UC1 --> UC3 : Nadzornik
UC2 --> UC1 : Konfiguracija
UC2 --> UC3 : Konfiguracija
UC4 --> UC5 : Zahteva
UC5 --> UC1 : Preverjanje pristnosti

@enduml


