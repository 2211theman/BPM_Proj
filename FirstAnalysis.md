# Passagi da seguire con anche la modifica del ritardo

1. **Ricezione dell'Ordine**
    - Il processo inizia con la ricezione di un ordine di trasporto contenente la data, il luogo e il contatto di origine e destinazione.

2. **Verifica della Capacità di Trasporto**
    - Il vettore verifica se è in grado di effettuare il trasporto. 
    - Se il vettore non è in grado di gestire il trasporto, il processo termina.

3. **Inserimento dell'Ordine nel Piano delle Consegne**
    - Se il vettore è in grado di gestire il trasporto, l'ordine viene inserito nel piano delle consegne.

4. **Prelievo**
    - Il vettore effettua il prelievo della merce presso l'origine indicata.

5. **Trasporto**
    - La merce viene trasportata dal luogo di origine al luogo di destinazione secondo i tempi indicati.

6. **Consegna**
    - La merce viene consegnata al luogo di destinazione indicato.

7. **Controllo della Presenza del Mittente e del Destinatario**
    - Al momento del prelievo e della consegna, il vettore verifica la presenza del mittente e del destinatario.
    - Se il mittente o il destinatario non sono presenti, il vettore procede al passaggio successivo.

8. **Contatto per Negoziare Nuove Date**
    - Il vettore contatta il mittente e/o il destinatario per negoziare una nuova data di prelievo e/o consegna.

9. **Proposta e Accettazione di Nuove Date**
    - Durante le negoziazioni, vengono proposte a turno nuove date di prelievo e/o consegna.
    - L'ultima data proposta viene accettata dal mittente o dal destinatario.

10. **Firma dei Documenti di Trasporto**
    - Al momento del prelievo e della consegna, vengono fatti firmare i documenti di trasporto al mittente e al destinatario, rispettivamente.

11. **Restituzione del Modulo Firmato**
    - Il processo termina quando il destinatario restituisce il modulo firmato al vettore.

**In caso di ritardo imprevisto:**

- **Contatto Preventivo per Ritardo**
    - Se si verifica un ritardo imprevisto, il vettore contatta preventivamente il destinatario per informarlo e negoziare una nuova data di consegna.
  
- **Prelievo**
    - Dopo aver negoziato una nuova data, il vettore effettua il prelievo della merce per procedere con la consegna.

# Descrizione del flusso 

1. **Ricezione dell'Ordine** -> **Verifica Capacità di Trasporto** -> **Inserimento Ordine nel Piano delle Consegne** -> **Prelievo** -> **Trasporto** -> **Consegna**

2. **Consegna/Prelievo** -> **Controllo Presenza Mittente e Destinatario** 
    - **Se il mittente o il destinatario non sono presenti**: 
        - **Contatto per Negoziare Nuove Date** -> **Accettazione Nuove Date**
    - **Se si verifica un ritardo imprevisto**: 
        - **Contatto per Negoziare Nuove Date** -> **Prelievo (per ritardo imprevisto)**

3. **Firma Documenti di Trasporto** -> **Ricezione Modulo Firmato** -> **Processo Termina**

# First bpmn try

https://modeler.cloud.camunda.io/share/39674854-dcb5-48ea-b165-db59c010a7d5