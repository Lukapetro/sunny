### Utenti:

> Questa tabella memorizza le informazioni sugli utenti del sistema.

- ID Utente
- Nome
- Cognome
- Email
- Password (hash)
- Altri dettagli personali (es. telefono)

### Stabilimenti

> Informazioni sugli stabilimenti balneari.

- ID Stabilimento
- Nome
- Indirizzo
- Descrizione
- Contatti (telefono, email)

### Ombrelloni e Lettini

> Dettagli sugli ombrelloni e lettini disponibili in ogni stabilimento.

- ID Ombrellone
- ID Stabilimento (chiave esterna)
- Numero
- Tipo (es. ombrellone, lettino)
- Stato (disponibile, prenotato, ecc.)

### Prenotazioni

> Gestione delle prenotazioni degli utenti.

- ID Prenotazione
- ID Utente (chiave esterna)
- ID Ombrellone (chiave esterna)
- Data Inizio
- Data Fine
- Stato Prenotazione (confermata, annullata, offerta in mercato secondario)

### Mercato Secondario

> Gestione delle offerte nel mercato secondario.

- ID Offerta
- ID Prenotazione (chiave esterna)
- ID Utente Venditore (chiave esterna)
- Prezzo Offerta
- Stato Offerta (disponibile, venduta, ritirata)

### Pagamenti

> Informazioni sui pagamenti effettuati.

- ID Pagamento
- ID Prenotazione (chiave esterna)
- Importo
- Metodo di Pagamento
- Data e Ora del Pagamento
- Stato del Pagamento (es. completato, fallito)

### Recensioni

> Recensioni degli utenti sugli stabilimenti.

- ID Recensione
- ID Utente (chiave esterna)
- ID Stabilimento (chiave esterna)
- Voto
- Testo Recensione
- Data Recensione
