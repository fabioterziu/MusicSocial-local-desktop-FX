# 🎵 SOCIAL_MUSICALE_LOCALE_DESKTOP_JAVAFX

## DESCRIZIONE:
Applicazione desktop realizzata in Java in collaborazione di un collega per l'esame universitario "Ingegneria del Software".
L'applicazione permette la gestione collaborativa di materiale musicale (testi/audio/video/youtube).
- Soltanto gli utenti autorizzati da un profilo admin potranno accedere.
- Gli utenti possono avere la possibilità di caricare/scaricare materiale musicale, commentare e annotare brani.

Per un'illustrazione più dettagliata fare riferimento a "Relazione.pdf"

## TECNOLOGIE UTILIZZATE
- linguaggio: JAVA
- framework GUI: JAVAFX
- markup UI: FXML
- stile UI: CSS
- database: SQLITE

## PATTERN
- Architetturale: MVC
- Design: DAO, SINGLETON, SINGLETON (lazy)
  
## DOCUMENTAZIONE E TESTING
Nel file "Relazione.pdf" è presente la documentazione del progetto, che comprende:
- Use Case principali e relative schede di specifica
- Sequence diagram di dettaglio per i principali Use Case
- Activity Diagram relativo alle modalità di interazione/operatività del software
- Class Diagram e Sequence diagram del software progettato
- Test degli sviluppatori
- Unit test
- Integration test
- Test degli utenti generici

Tutti i diagrammi (oltre ai principali in Relazione.pdf) sono presenti in "Diagrammi.pdf"//////////////////////////// ** FINIRE DI SCRIVERE ***

## NOTE
- **stato del progetto:**
  Il progetto è concluso e funzionante.
  È prevista però una fase di refactoring volta a migliorare ulteriormente la separazione delle resposabilità.
  Nello specifico si procederà alla suddivisione della logica di business dai controller in apposite classi di servizio, come è stato già fatto per 'TrackController' e 'TrackService'

- Credenziali admin:
  username: admin
  password: admin

- Gestione chiave YOUTUBE API:
  per questioni di sicurezza, la chiave è gestita esteranmente.
  Prima di avviare l'applicazione è neccessario impostare la variabile "YOUTUBE_API_KEY" da terminale:
  per linux/macos: export YOUTUBE_API_KEY="CHIAVE"
  altrimenti:
  l'applicazione viene eseguita comuque, ma senza la possibilità di visionare video youtube all'interno dell'app stessa
