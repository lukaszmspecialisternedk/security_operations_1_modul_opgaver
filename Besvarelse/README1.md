1. Installere OS uden GUI:
Jeg valgte at installere en Debian 13 VM, da det var ikke en OS jeg har arbejdet med den førhen og lærer noget nyt. Jeg forsøgte at installere dem uden GUI og kørte installation også via BIOS oprindeligt.

<img width="659" height="425" alt="Skærmbillede 2026-09-14 161811" src="https://github.com/user-attachments/assets/d159aad7-5b35-4942-9356-7ac5eeca1443" />

<img width="411" height="377" alt="Skærmbillede 2026-09-14 134701" src="https://github.com/user-attachments/assets/3a4a0037-8f5e-4b52-893b-16e6b9411cd9" />

<img width="663" height="437" alt="Skærmbillede 2026-09-17 095724" src="https://github.com/user-attachments/assets/bfba7763-7b87-4f55-b084-1cf83ee1dfaa" />

<img width="531" height="412" alt="Skærmbillede 2026-09-17 095637" src="https://github.com/user-attachments/assets/00d6549a-f2ca-429d-a81b-33e4d2e9e4a7" />

<img width="689" height="432" alt="Skærmbillede 2026-09-16 093846" src="https://github.com/user-attachments/assets/2dc0d144-036a-43b8-89e5-0d00e0b26046" />

<img width="663" height="431" alt="Skærmbillede 2026-09-14 161843" src="https://github.com/user-attachments/assets/7bef1fee-1493-41e3-8883-79dcf8fb6c95" />


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




4. Opret SSH adgang via nøgle-baseret authentication:

Oprettelse af SSH pub keys på "lokal maskine" (Kali) til test af SSH public key authentication: 

<img width="656" height="417" alt="Skærmbillede 2026-09-17 153455" src="https://github.com/user-attachments/assets/46bdd448-f3cd-4e84-894b-7849c1d9a566" />

<img width="651" height="412" alt="Skærmbillede 2026-09-17 151424" src="https://github.com/user-attachments/assets/22cd55b0-2b41-4cb9-87cf-28700e8c8adf" />

<img width="653" height="419" alt="Skærmbillede 2026-09-17 151404" src="https://github.com/user-attachments/assets/16315bd2-f301-48b6-aa26-afc8d3d30534" />

Anvendte "ssh-copy-id" til at overfører en ed22519 pubkey til Debian serveren, som følgende trin til at etablere public key authentication på tværs af de to VMs:




5. Diverse bilag:
   
Projektstyring

Trello tasks progression på modul 1:

<img width="956" height="389" alt="Skærmbillede 2026-09-17 154041" src="https://github.com/user-attachments/assets/ed99361d-93c3-43fb-b110-b727ba33d99f" />

<img width="956" height="365" alt="Skærmbillede 2026-09-17 144301" src="https://github.com/user-attachments/assets/c28cba73-11ae-4081-b0c4-ecca6dbacc62" />

<img width="959" height="379" alt="Skærmbillede 2026-09-17 142749" src="https://github.com/user-attachments/assets/d0715ded-7e83-4ff5-b8a2-136db218fb7c" />
