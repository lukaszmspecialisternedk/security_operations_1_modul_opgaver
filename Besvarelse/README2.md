# Modul 2

## 1. Redegør for diverse Linux Filesystem Hierarchy Standard (FHS) mapper:

- /etc : Denne mappe er her, hvor de fleste konfigurationsfiler befinder sig i et Linux distro system. (Host specific system configuration)

- /var : "/var" (variable) mappen indeholder database og spool filer.

- /var/log : Mappen Indholder diverse system specifikke log filer.

- /home : Den enktelte brugers hovedemappe og forgreninger. (Home directory)

- /usr : Sekundært filhierarki for brugeren. Udelukkende "read-only data. (Unix System Resources)

- /tmp : Mappen for midlertidige filer. (Temporary files)

- /bin : Mappen som bevar diverse essentielle bruger kommandoer. (Essenital User Command Binaries)

- /sbin : "/sbin" er en user relateret mappe, der er rettet mod superbruger/root bruger privilegier. (Superuser binaries)

- /boot : "/boot" indeholder filer der forbundet til bootloaderen og Linux kernen (kernel). (Static files for the bootloader)

- /lib : (Shared libraries)
  
- /proc : "filsystem" mappe. der levere proces og kerne information i filer. (Process information)
  
- /root : Ligesome hovedemappen for en enkelt bruger, men blot for "root" istedet.




## 2. Oprettelse af en mappe med bestemte gruppe permissions (uden brug af "chmod 777" - all user access):

Til start, oprettes en test mappe for denne opgave:

<img width="1314" height="837" alt="Skærmbillede 2026-09-18 124247" src="https://github.com/user-attachments/assets/7d7b94e6-e3f8-47d4-813c-d325a137658b" />

Herunder, som eksempel, ændrer jeg gruppe permissions til kun at være kun "read-only" (o=r ; "others"="read") for alle andre brugere end mappens owner (newuser):

<img width="1309" height="829" alt="Skærmbillede 2026-09-18 125626" src="https://github.com/user-attachments/assets/5e341251-6d26-43f3-8940-6fe95e2c7fdb" />

<img width="1297" height="814" alt="Skærmbillede 2026-09-18 125932" src="https://github.com/user-attachments/assets/30214cf2-8dba-49a7-ba88-d9b9db404e82" />

Jeg skifter til "newuser2" og prøver at læse mappen - men gruppens permissions blokere denne kommando:

<img width="1315" height="823" alt="Skærmbillede 2026-09-18 130020" src="https://github.com/user-attachments/assets/354043c8-1fe0-4bbf-b1f5-bec233277d37" />

Grunden til at "change mode (chmod) 777" bør undgåes er fordi denne indstilling giver alle gruppe permissions til alle vilkårlige brugere (rwxrwxrwx : read(r), write(w), execute(x)). Fra et sikkerhedsperspektiv, er det en sløset måde at håndtere rettigheder til brugere på. Det indebærer desuden en risiko for at en udefrakommende angriber/indtrænger kan eller kunne udefører farlige handlinger eller skaffe sig adgang til filer eller mapper de ikke bør have adgang til. 


## 3. Identificere forkert konfigureret rettigheder i et udleveret testmiljø:




## 4. Anvend Access Control List (ACL) til at give midlertidig, afgrænset adgang til en mappe uden at ændre dens grundlæggende gruppestruktur:
