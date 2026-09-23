# Modul 3

## 1. Opret tre brugerroller (admin, developer og guest) - med forskellige rettigheder:

Oprettelse af forskellige grupper først:

<img width="1296" height="815" alt="Skærmbillede 2026-09-21 142151" src="https://github.com/user-attachments/assets/4f73c1f7-6688-4af8-ae6b-fe545f404109" />

<img width="1297" height="816" alt="Skærmbillede 2026-09-21 145414" src="https://github.com/user-attachments/assets/b7a30bb7-8274-4faa-bcc9-47e490cb57c0" />

Oprettelse af respektive brugere i sammenhæng med opgaven:

<img width="1293" height="811" alt="Skærmbillede 2026-09-21 145029" src="https://github.com/user-attachments/assets/62dc7fda-eda7-4f4f-a7c6-e911959bf533" />

Derefter en tilføjelse af brugerne til tilsvarende grupper:

<img width="1291" height="811" alt="Skærmbillede 2026-09-21 150440" src="https://github.com/user-attachments/assets/dc9a8508-4c20-4764-8161-518d63c8ded5" />

Justere "adminuser" til at få øvrig adgang på tværs af alle mapper - som en slags "over-bruger" til at håndtere de andre gruppemappers' indhold og monitorering:

<img width="1294" height="813" alt="Skærmbillede 2026-09-23 121001" src="https://github.com/user-attachments/assets/fd3876bf-8656-45c2-87c8-5fcf9265ef85" />


Justering af eger rettighederne/permissions til de respektive folders:

<img width="649" height="409" alt="Skærmbillede 2026-09-23 105806" src="https://github.com/user-attachments/assets/3a3d6aa1-8b2f-406f-b143-5c8db2c0b8fc" />

Og de tilhørende bruger permissions til diverse "arbejdsmapper":

<img width="1296" height="813" alt="Skærmbillede 2026-09-23 110040" src="https://github.com/user-attachments/assets/84c147df-329e-4cbe-a37f-1a77dc709e1b" />

Et test af, hvordan et scenarie med en aktivt logget ind "guest" bruger rolle ville se ud, når de forsøgte at navigere rundt mappe hierarkiet med den indstillede rolle rettigheder:

<img width="649" height="408" alt="Skærmbillede 2026-09-23 110458" src="https://github.com/user-attachments/assets/a24ed48b-dccc-4551-bf1d-7515179c95f1" />

Et overblik over, hvordan de respektive grupper, gruppernes rettigheder og mappe strukturen forholder sig:

<img width="1297" height="816" alt="Skærmbillede 2026-09-23 110618" src="https://github.com/user-attachments/assets/6fa8bb66-a920-437b-86af-7e36fa440e9b" />


## 2. Konfigurere grupper, så developers har skriveadgang (write) til et fælles projektområde og guests kun har læseadgang (read):






## 3. Konfigurere sudo-rettigheder granulært, så admin gruppen kan kun udfører specifikke kommandoer i forhold til root:







## 4. Tabel over rollestruktur


| Bruger | Grupper | Rettigheder | Begrundelse |
|--------|---------|-------------|-------------|
|adminuser|  admin, developers, guests|  read, write, execute| Vedkommende har adgang og privilegier på tværs af alle grupper, så de kan monitorere brugerne, deres adgang og mappernes indhold |
|developeruser1|developers| read, write, execute | Udviklerne er udelukkende afgrænset til deres eget arbejdsområde med minimum privilege princippet i mente|
|developeruser2|developers| read, write, execute |  (samme argument som ovenstående)            |
|guestuser| developers, guests | read-only            | Besøgende roller ("guests"), bør næsten have ingen betydelige privilegier, udover at læse filer i deres egen mappe og eventuelt tage et kig i "developers" mappen, hvis der f.eks. er tale om en ekstern konsulent eller klient |

## 5. Bilag


Projektstyring:


<img width="1905" height="1020" alt="Skærmbillede 2026-09-21 141910" src="https://github.com/user-attachments/assets/5854fe30-beed-4304-a414-d06d73ea926f" />



<img width="955" height="472" alt="Skærmbillede 2026-09-23 132810" src="https://github.com/user-attachments/assets/87c307f6-412a-4d15-8e02-738a03c80e48" />


