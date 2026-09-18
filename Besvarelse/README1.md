1. Installere OS uden GUI:
Jeg valgte at installere en Debian 13 VM, da det var ikke en OS jeg har arbejdet med den førhen og lærer noget nyt. Jeg forsøgte at installere dem uden GUI og kørte installation også via BIOS oprindeligt.

<img width="659" height="425" alt="Skærmbillede 2026-09-14 161811" src="https://github.com/user-attachments/assets/d159aad7-5b35-4942-9356-7ac5eeca1443" />

<img width="411" height="377" alt="Skærmbillede 2026-09-14 134701" src="https://github.com/user-attachments/assets/3a4a0037-8f5e-4b52-893b-16e6b9411cd9" />

<img width="663" height="437" alt="Skærmbillede 2026-09-17 095724" src="https://github.com/user-attachments/assets/bfba7763-7b87-4f55-b084-1cf83ee1dfaa" />

<img width="531" height="412" alt="Skærmbillede 2026-09-17 095637" src="https://github.com/user-attachments/assets/00d6549a-f2ca-429d-a81b-33e4d2e9e4a7" />

<img width="689" height="432" alt="Skærmbillede 2026-09-16 093846" src="https://github.com/user-attachments/assets/2dc0d144-036a-43b8-89e5-0d00e0b26046" />


2. Statisk IP adresse og sigende hostname:

Konfiguration af statisk IP addresse på Debian VM'en

<img width="418" height="305" alt="Skærmbillede 2026-09-17 131017" src="https://github.com/user-attachments/assets/198ec86e-b9e8-48fd-ad8f-eb7244870978" />

Ændring af hostname til et sigende navn på maskinen "newuser-my-pc":

<img width="549" height="342" alt="Skærmbillede 2026-09-17 134150" src="https://github.com/user-attachments/assets/33302b95-d35f-4fd7-9e33-4c6c1a2342a7" />

Blev nødtil at konfigurere netværksindstillinger, da ping test af den statiske IP og Google.com DNS test ikke virkede oprindeligt: 

<img width="655" height="422" alt="Skærmbillede 2026-09-17 131905" src="https://github.com/user-attachments/assets/7d5351ad-e4e9-45c6-85fd-6a7c63986103" />

<img width="953" height="409" alt="Skærmbillede 2026-09-17 133256" src="https://github.com/user-attachments/assets/fc01883c-6495-4b63-b442-0d356020eddd" />

<img width="549" height="347" alt="Skærmbillede 2026-09-17 133841" src="https://github.com/user-attachments/assets/c67c8fff-7e39-431c-bb6c-50109f78b283" />

Test fra selve laptop for at checke om der var netværkskommunikation:

<img width="425" height="283" alt="Skærmbillede 2026-09-17 142635" src="https://github.com/user-attachments/assets/fde18dee-8241-4164-b12f-1120d42ca1aa" />


3. Opret en non-root bruger og deaktivere root adgang via SSH:

Anvendte terminal vindue med kommandoen "adduser" for at oprette en ny bruger:

<img width="656" height="417" alt="Skærmbillede 2026-09-17 142523" src="https://github.com/user-attachments/assets/a20caffb-f726-479b-a78a-32fd440c576e" />

<img width="656" height="419" alt="Skærmbillede 2026-09-17 144557" src="https://github.com/user-attachments/assets/f63f45f2-2134-4f00-9099-9bafc16d952b" />

<img width="653" height="419" alt="Skærmbillede 2026-09-17 161712" src="https://github.com/user-attachments/assets/1a396e26-765c-42ab-b2de-9103af98ff8d" />


Deaktivering af "root" adgang via SSH i "sshd_config" filen:


<img width="546" height="344" alt="Skærmbillede 2026-09-17 143108" src="https://github.com/user-attachments/assets/42ee937a-e6e7-4d8f-bd47-7395445fe9dd" />


4. Opret SSH adgang via nøgle-baseret authentication:

Installation af "openssh-server" pakken på Debian:

<img width="552" height="347" alt="Skærmbillede 2026-09-17 141934" src="https://github.com/user-attachments/assets/390cf390-945d-4230-b6f8-da517b1d097b" />

<img width="563" height="345" alt="Skærmbillede 2026-09-17 134332" src="https://github.com/user-attachments/assets/86bdf569-ea2f-4d31-91a9-c0201c4eae3b" />

Diverse konfigurationer af "sshd_config" filen til hærde adgangen til serveren:

<img width="652" height="418" alt="Skærmbillede 2026-09-17 150246" src="https://github.com/user-attachments/assets/335866e8-2ebe-42a1-9e20-cd05ded39e49" />

<img width="652" height="421" alt="Skærmbillede 2026-09-17 150159" src="https://github.com/user-attachments/assets/ed2cbde3-d788-4ddf-808d-572c4dd0b984" />

Anvendte "ssh-copy-id" til at overfører en ed22519 pubkey til Debian serveren's "auth_keys" mappe og etablere SSH key authentication på tværs af de to forskellige maskiner/enheder (VMs). I denne sammenhæng valgte jeg at anvende Debian og Kali til opgavens formål:

<img width="407" height="326" alt="Skærmbillede 2026-09-17 152645" src="https://github.com/user-attachments/assets/a64ca724-d0d8-4656-b309-b83194704f70" />

Oprindelige forbindelses test af SSH key auth for at se om den virker som forventet:


<img width="655" height="416" alt="Skærmbillede 2026-09-17 145337" src="https://github.com/user-attachments/assets/62ca6fcd-5514-4d4c-9875-289dc025aea8" />


Skiftede SSH's default port fra "22" til "2222" for at gøre den mindre åbenlys. Port 22 er en af de mest almindelige/oplagte porte, der typisk bliver scannet eller angrebet. Kunne alternativt været noget væsentligt mere obskurt for at gøre det sværere at dektere (f.eks: 22222, 23455, 20200, 25000 osv.):

<img width="1330" height="850" alt="Skærmbillede 2026-09-18 101202" src="https://github.com/user-attachments/assets/fa43d569-e5b5-429e-9cf0-0d46fb768aaa" />


Oprettelse af SSH pub keys på "lokal maskine" (Kali) til test af SSH public key authentication: 

<img width="656" height="417" alt="Skærmbillede 2026-09-17 153455" src="https://github.com/user-attachments/assets/46bdd448-f3cd-4e84-894b-7849c1d9a566" />

<img width="651" height="412" alt="Skærmbillede 2026-09-17 151424" src="https://github.com/user-attachments/assets/22cd55b0-2b41-4cb9-87cf-28700e8c8adf" />

<img width="653" height="419" alt="Skærmbillede 2026-09-17 151404" src="https://github.com/user-attachments/assets/16315bd2-f301-48b6-aa26-afc8d3d30534" />

Diverse indstillinger i sshd_config filen i sammenhæng med løsningen:

<img width="653" height="410" alt="Skærmbillede 2026-09-17 155209" src="https://github.com/user-attachments/assets/9df30a38-8404-4aaa-8b9c-795da1cd3f49" />

5. Diverse bilag:
   
Projektstyring

Trello tasks progression på modul 1:

<img width="956" height="389" alt="Skærmbillede 2026-09-17 154041" src="https://github.com/user-attachments/assets/ed99361d-93c3-43fb-b110-b727ba33d99f" />

<img width="956" height="365" alt="Skærmbillede 2026-09-17 144301" src="https://github.com/user-attachments/assets/c28cba73-11ae-4081-b0c4-ecca6dbacc62" />

<img width="956" height="389" alt="Skærmbillede 2026-09-17 154041" src="https://github.com/user-attachments/assets/7a53ac69-ee78-4735-b6c2-e0a82bf43f60" />

