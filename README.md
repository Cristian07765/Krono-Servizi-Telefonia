# Centralino online gratuito – Studio Multiservizi

## Avvio / pubblicazione
Questa è una web app statica. Per provarla in locale usa un server HTTPS o localhost; il microfono richiede un contesto sicuro.
Puoi pubblicare `public/index.html` su un hosting statico gratuito che fornisca HTTPS (ad esempio GitHub Pages).

## Come provarla
1. Pubblica la pagina in HTTPS.
2. Il professionista apre la scheda "Sono un professionista", sceglie il servizio, inserisce un codice condiviso di almeno 6 caratteri e preme "Attiva disponibilità".
3. Il cliente apre la stessa pagina, seleziona il servizio, inserisce il codice comunicato per quel servizio e avvia la chiamata.
4. Entrambi consentono l'uso del microfono.

## Limiti da conoscere
- È una chiamata audio via browser/WebRTC, NON una chiamata telefonica verso numeri fissi o cellulari.
- Usa il servizio pubblico di segnalazione PeerJS; disponibilità e condizioni possono cambiare e non è un servizio garantito.
- La connessione diretta può fallire per NAT/firewall/reti mobili. Un server TURN migliora l'affidabilità ma può non essere gratuito.
- La pagina deve essere servita via HTTPS (localhost è un'eccezione per i test).
- I codici sono condivisi manualmente; non c'è ancora autenticazione robusta, gestione privacy o storico chiamate. Non pubblicare codici sensibili.
- Per un uso commerciale stabile occorre una revisione di sicurezza, privacy/GDPR, test su dispositivi e un servizio di segnalazione/TURN affidabile.
- Non usare per emergenze. In caso di pericolo chiamare 112.
