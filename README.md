# Master Provette — segnalatore di versione

Questo repository serve solo a far sapere all'app **Master Provette** (chiavetta/eseguibile,
codice privato in `nalettonicolo/Francesca`) se esiste una versione più recente.

Contiene un solo file, [`version.json`](version.json), letto pubblicamente
dall'app (nessuna autenticazione richiesta). Non contiene codice né dati
dell'app: solo il numero dell'ultima versione preparata.

## Come si aggiorna

Quando prepari una nuova chiavetta:

1. Aggiorna `CURRENT_VERSION` in `web/index.html` (repo privato) con il nuovo numero.
2. Modifica `version` in questo `version.json` allo stesso numero e fai commit/push.

L'app, la prossima volta che viene avviata con una connessione internet, vedrà
che è disponibile una versione più recente e mostrerà un avviso (nessun
aggiornamento automatico dei file: solo la segnalazione).
