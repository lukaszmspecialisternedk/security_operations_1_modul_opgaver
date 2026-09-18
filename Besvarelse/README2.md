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




## 2. Oprettelse af en mappe med bestemte gruppe permissions (uden brug af "chmod 777"):

Til start, oprettes en test mappe for denne opgave:

<img width="1314" height="837" alt="Skærmbillede 2026-09-18 124247" src="https://github.com/user-attachments/assets/7d7b94e6-e3f8-47d4-813c-d325a137658b" />








## 3. Identificere forkert konfigureret rettigheder i et udleveret testmiljø:




## 4. Anvend Access Control List (ACL) til at give midlertidig, afgrænset adgang til en mappe uden at ændre dens grundlæggende gruppestruktur:
