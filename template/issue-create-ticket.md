# Issue: Create ticket with validation

## Request

```txt
Serve creare ticket dal supporto.
```

## Fatti (Facts)

- ci troviamo su un applicazione di ticketing in react e java;
- non bisogna scrivere codice, siamo in una fase di pianificazione;
- non possiamo visualizzare la repo di riferimento;

## Assunzioni (Assumptions)

- deve essere implementato un input che se cliccato permette di compilare un ticket

## Domande Aperte (Questions)

- cosa vuol dire ticket "dal supporto"?
- fuori dal supporto è già possibile inviare ticket?

## Decisione (Decision)

Per questo slice, "creare ticket" significa:

```txt
avere un bottone che una volta premuto ti permette di complare ed inviare un messaggio al supporto, per avere chiarimenti o soluzioni ad un problema.
```

## Fuori Scope / Non-Obiettivi (Non-Goals)

- non scriviamo codice
- non installare o aggiungere file nella repo
- non leggere file oltre a quelli contenuti nella cartella template
- un ticket non può essere vuoto

## Criteri Di Accettazione (Acceptance Criteria)

1. un input valido inserito permette di inviare il ticket dal supporto
2. il resto dell'applicazione, al di fuori del ticket dal supporto deve risultare invariato.


## Piano Di Verifica Manuale (Manual Test Plan)

- implementazione valida: alla pressione dell'input sarà possibile compilare ed inviare il ticket
- implementazione non valida: alla pressione dell'input non sarà possibile compilare ed inviare il ticket
