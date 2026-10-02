# Modul 4


## 1. Konfigurer nftables, så al indgående trafik som udgangspunkt blokeres:

Installation af nftables:

<img width="652" height="413" alt="Skærmbillede 2026-09-24 204554" src="https://github.com/user-attachments/assets/7de101ca-27ab-46ae-a14d-e3b3626c3880" />

Konfiguration af nftables fil:

<img width="656" height="414" alt="Skærmbillede 2026-09-24 205346" src="https://github.com/user-attachments/assets/041b9bb8-ee35-401d-bc89-6c87a3a1a4f9" />

Nulstilling af alt indgående og udegående traffik (ingress/egress):

<img width="659" height="421" alt="Skærmbillede 2026-09-24 205837" src="https://github.com/user-attachments/assets/90751436-0f92-4bfc-82ac-a6c41a5aac84" />

## 2. Åbn udelukkende de porte, systemet reelt har brug for:

Åbner som udgangspunkt kun for nødvendige porte, som 443 og 80 for webtraffik:

<img width="656" height="417" alt="Skærmbillede 2026-09-24 210154" src="https://github.com/user-attachments/assets/80d1d538-72df-4548-bca0-7fe3e2b5e4c6" />

Tjekker om internettet kan stadig tilgåes via webbrowser efter justering i nftables:

<img width="654" height="415" alt="Skærmbillede 2026-09-24 212832" src="https://github.com/user-attachments/assets/32b186f7-4042-4905-b974-ab85dfbef5e4" />

## 3. Begræns SSH-adgang til et defineret IP-interval, hvis scenariet tillader det:

Justere konfigurationsfilen til at kun et bestemt IP interval og SSH adgang indsnævres:

<img width="644" height="406" alt="Skærmbillede 2026-09-24 214041" src="https://github.com/user-attachments/assets/bb61fb7e-360a-4579-89d8-20a73d666fa1" />

Genstart af nftables:

<img width="646" height="409" alt="Skærmbillede 2026-09-24 214152" src="https://github.com/user-attachments/assets/b26ff5d9-9995-457a-a44f-e71d9f8593bd" />

Tjekker om SSH adgang kan tilgåes af en maskine med det bestemte interval.

Virker med Kali VM:

<img width="959" height="487" alt="Skærmbillede 2026-09-24 214530" src="https://github.com/user-attachments/assets/9d8b45eb-1eaa-4d05-83c1-5764e5859f13" />

Timer ud på Windows 11 OS (host maskine til virtualisering):

<img width="626" height="294" alt="Skærmbillede 2026-09-24 214844" src="https://github.com/user-attachments/assets/db696518-a6ff-490f-8a32-ed377297114a" />

## 4. Dokumentér hver åben port med begrundelse: hvilken tjeneste, hvorfor den er nødvendig, og hvilken risiko den introducerer:

Portene 443 og 80 er åbne for at kunne tillade websurfing med maskinens webbrowser. SSH blev tildelt en ny port (2222) for at tilsløre dens lokation, men stadig kunne tillade remote access på tværs af en klient maskine (Kali VM).  

## 5. Bilag
Projektstyring:
