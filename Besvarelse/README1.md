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
<img width="549" height="347" alt="Skærmbillede 2026-09-17 133841" src="https://github.com/user-attachments/assets/b40b2a95-06d3-4e6f-8d03-a5cc4afbf7a9" />

<img width="953" height="409" alt="Skærmbillede 2026-09-17 133256" src="https://github.com/user-attachments/assets/bd6d6129-156a-41c5-b53b-1c04589e66df" />

<img width="655" height="422" alt="Skærmbillede 2026-09-17 131905" src="https://github.com/user-attachments/assets/7d5351ad-e4e9-45c6-85fd-6a7c63986103" />




3. Opret en non-root bruger og deaktivere root adgang via SSH:

<img width="653" height="419" alt="Skærmbillede 2026-09-17 161712" src="https://github.com/user-attachments/assets/ed667a3d-4272-4a9e-8a34-c5cdfeb3baa8" />

<img width="656" height="419" alt="Skærmbillede 2026-09-17 144557" src="https://github.com/user-attachments/assets/2b94fa45-36cd-46d7-99b6-9edaadb92239" />

<img width="555" height="353" alt="Skærmbillede 2026-09-17 143046" src="https://github.com/user-attachments/assets/25c31bfc-e9b2-4db2-8030-6d2213543e02" />

<img width="656" height="417" alt="Skærmbillede 2026-09-17 142523" src="https://github.com/user-attachments/assets/8cd99e02-fdab-43a2-9ed0-be91bf67b736" />

<img width="658" height="416" alt="Skærmbillede 2026-09-17 142449" src="https://github.com/user-attachments/assets/f7a47021-932e-474d-b570-f6dd9587ee8f" />


4. Opret SSH adgang via nøgle-baseret authentication:

<img width="650" height="420" alt="Skærmbillede 2026-09-17 145130" src="https://github.com/user-attachments/assets/19c6b653-02a4-4ae0-ab72-b8ba623a0194" />

<img width="543" height="370" alt="Skærmbillede 2026-09-17 155613" src="https://github.com/user-attachments/assets/ed820693-bd6e-4151-9c3f-b48e7ddc5b96" />

<img width="542" height="358" alt="Skærmbillede 2026-09-17 155540" src="https://github.com/user-attachments/assets/e9039315-fc7f-414c-a591-ec931a0ca467" />

<img width="537" height="346" alt="Skærmbillede 2026-09-17 155440" src="https://github.com/user-attachments/assets/9d03267d-f6c3-4b2a-9ab3-1630311f4f7b" />

<img width="653" height="410" alt="Skærmbillede 2026-09-17 155209" src="https://github.com/user-attachments/assets/9c61e4e4-4e1f-4804-b72b-8ae98dac651a" />

<img width="383" height="180" alt="Skærmbillede 2026-09-17 154915" src="https://github.com/user-attachments/assets/1e13848f-22a1-4728-979c-c64923726a4c" />

<img width="382" height="395" alt="Skærmbillede 2026-09-17 154852" src="https://github.com/user-attachments/assets/9b8f896c-d026-4ff5-a50d-4a8a832524d6" />

<img width="466" height="254" alt="Skærmbillede 2026-09-17 154744" src="https://github.com/user-attachments/assets/8baa5d73-7bc3-4387-8ba3-2150458bd44d" />

<img width="656" height="417" alt="Skærmbillede 2026-09-17 153455" src="https://github.com/user-attachments/assets/064758ed-85ee-4494-a428-f6a6e7f222f4" />

<img width="506" height="266" alt="Skærmbillede 2026-09-17 152828" src="https://github.com/user-attachments/assets/4a38635e-1a5b-4e77-8145-0d245aff1499" />

<img width="508" height="244" alt="Skærmbillede 2026-09-17 152758" src="https://github.com/user-attachments/assets/2e9bcc87-b680-4b6d-b9b6-d2addea0b94e" />
<img width="407" height="326" alt="Skærmbillede 2026-09-17 152645" src="https://github.com/user-attachments/assets/e701c502-bf20-46d8-826e-baa8c8506a9b" />

<img width="651" height="412" alt="Skærmbillede 2026-09-17 151424" src="https://github.com/user-attachments/assets/e2ce7dbe-ef6e-49ba-a53b-7c56eedb3d7a" />

<img width="653" height="419" alt="Skærmbillede 2026-09-17 151404" src="https://github.com/user-attachments/assets/a82c9fe3-3a9b-4bb5-867e-9607b1534958" />

<img width="613" height="158" alt="Skærmbillede 2026-09-17 151025" src="https://github.com/user-attachments/assets/f69021f2-c7ba-4fb7-8c59-5205911037de" />

<img width="651" height="413" alt="Skærmbillede 2026-09-17 150511" src="https://github.com/user-attachments/assets/6077a668-d889-481a-bfdc-7c425bd8d58c" />

<img width="652" height="418" alt="Skærmbillede 2026-09-17 150246" src="https://github.com/user-attachments/assets/2762a7a9-0814-4690-867f-479da212f2a2" />

<img width="652" height="421" alt="Skærmbillede 2026-09-17 150159" src="https://github.com/user-attachments/assets/5d60158f-b8c0-4f5b-bf0b-bd546b2d9ff7" />

<img width="647" height="416" alt="Skærmbillede 2026-09-17 150049" src="https://github.com/user-attachments/assets/86576fb7-fd7a-41d1-bd77-b3a9a2d4b99f" />

<img width="652" height="416" alt="Skærmbillede 2026-09-17 145820" src="https://github.com/user-attachments/assets/308a333b-dcbe-434d-ad66-1b0deadb5152" />

<img width="654" height="422" alt="Skærmbillede 2026-09-17 145046" src="https://github.com/user-attachments/assets/4ed33b06-9e42-4fbb-826d-c28c9df94c0f" />

<img width="653" height="414" alt="Skærmbillede 2026-09-17 145355" src="https://github.com/user-attachments/assets/edd4b0bc-e819-4615-af05-87e40dbdb0be" />

<img width="655" height="416" alt="Skærmbillede 2026-09-17 145337" src="https://github.com/user-attachments/assets/65eff0d9-ac38-4ba9-8e12-13a1a8d09f7e" />

<img width="951" height="488" alt="Skærmbillede 2026-09-17 144635" src="https://github.com/user-attachments/assets/18fccfe2-4cf3-473a-97e0-9db9a9a7ff8e" />

<img width="657" height="422" alt="Skærmbillede 2026-09-17 144500" src="https://github.com/user-attachments/assets/d9ef9258-33f9-4d6f-b538-7d5f13bf6044" />

<img width="653" height="426" alt="Skærmbillede 2026-09-17 144411" src="https://github.com/user-attachments/assets/e7822466-1f8b-4a9b-993d-8ad1eef2f612" />

<img width="548" height="341" alt="Skærmbillede 2026-09-17 144140" src="https://github.com/user-attachments/assets/36895da4-83bf-4a38-aa18-c8df7da36e08" />

<img width="657" height="424" alt="Skærmbillede 2026-09-17 143526" src="https://github.com/user-attachments/assets/aa4d753b-de93-4145-a795-4c80ea1a1db2" />

<img width="546" height="344" alt="Skærmbillede 2026-09-17 143108" src="https://github.com/user-attachments/assets/59ab3aa3-3574-461d-8366-af232b187427" />

<img width="546" height="341" alt="Skærmbillede 2026-09-17 142916" src="https://github.com/user-attachments/assets/e7013d8a-7aa2-4c23-b16e-d886251eb751" />

<img width="552" height="347" alt="Skærmbillede 2026-09-17 141934" src="https://github.com/user-attachments/assets/c14216a5-194b-4fa9-99bc-0948701c543a" />

<img width="563" height="345" alt="Skærmbillede 2026-09-17 134332" src="https://github.com/user-attachments/assets/2272ba8a-3d98-4585-a88c-49b40fcd3770" />

5. Diverse bilag:
   
Projektstyring

Trello tasks progression på modul 1:

<img width="956" height="389" alt="Skærmbillede 2026-09-17 154041" src="https://github.com/user-attachments/assets/ed99361d-93c3-43fb-b110-b727ba33d99f" />

<img width="956" height="365" alt="Skærmbillede 2026-09-17 144301" src="https://github.com/user-attachments/assets/c28cba73-11ae-4081-b0c4-ecca6dbacc62" />

<img width="959" height="379" alt="Skærmbillede 2026-09-17 142749" src="https://github.com/user-attachments/assets/d0715ded-7e83-4ff5-b8a2-136db218fb7c" />
