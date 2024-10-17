# **Configurazione prodotti**
In questo documento verranno descritti gli step di setup e predisposizione degli ambienti per i prodotti Dynamics 365 Sales e Customer Insights Journeys

### Creazione degli ambienti
Di seguito elencati gli step seguiti per effettuare la creazione degli ambienti Dynamics; la procedura sotto riportata, è stata eseguita per la creazione di ogni singolo ambiente (sviluppo, test, produzione).

1. Accesso a **Power Platform interfaccia di amministrazione** (con utenza di amministratore Dynamics 365 o Power Platform amministratore)  
2. Selezionare la voce **“Ambienti”**  
3. Cliccare su **“Nuovo”**  
4. All’interno della form di creazione, popolare i seguenti campi:  
    - *Nome:* DEV-CRM (ambiente di sviluppo); UAT-CRM (ambiente di test); PROD-CRM (ambiente di produzione)  
    - *Area Geografica:* Europa  
    - *Type:* Sandbox (per gli ambienti dev e uat) / Production (per l'ambiente di Produzione)  
    - *Aggiungi un'origine dati Dataverse:* si  
    - *Pagamento a consumo con Azure:* no 
   - *Selezionare **Avanti** e proseguire con la valorizzazione*
    - *Lingua:* italiano  
    - *Valuta:* €  
    - *Gruppo di sicuarezza:* Inserimento del Gruppo definito su Azure Active Directory: crm-d-adgroup-admin (ambiente di sviluppo); crm-u-adgroup-admin (ambiente di test); crm-p-adgroup-admin (ambiente di produzione);   
    - *Url (selezionare clicca QUI):* dev-pagopa (ambiente di sviluppo); uat-pagopa (ambiente di test); pagopa (ambiente di produzione)  
    - *Abilita app Dynamics 365:* si (selezionare l’app dynamics sales) å
5. Procedere al **Salvataggio**; a seguito del salvataggio è stata avviata la creazione degli ambienti con annessa installazione del modulo Sales.
### Installazione di Customer Insights - Journeys
Di seguito gli step per l’installazione dell’app *Customer insights \- Journeys:*  
1. Dall'**interfaccia di amministrazione di Power Platform**, cliccare su Power Platform Admin Center  
2. Selezionare l’ambiente: dal menu di sinistra, selezionare **Ambienti** e scegliere l'ambiente in cui installare l'app (la procedura è stata replicata per ogni ambiente)   
3. Installazione dell'app: Cliccare su **Risorse** \--\> App Dynamics 365 \--\> ricercare "app di marketing" nell'elenco delle app disponibili, selezionare (Dynamics 365 solution only) e cliccare su **Installa**.

Il sistema avvia automaticamente l’installazione dell’app.
Per rendere fruibili tutti i servizi di *Customer Insights - Journeys*, è  necessario accedere alla sezione Provisioning e cliccare sul pulsante **“Convert to payment offer"**.
### Assegnazione ruoli a gruppi di sicurezza
1. Nell’interfaccia di amministrazione di Microsoft, selezionare il gruppo di sicurezza  
2. Dalla sezione Ruoli sono stati assegnati i ruoli desiderati al gruppo  
3. Cliccare su Gestisci l’appartenenza al gruppo  
4. Aggiungere o rimuovere gii utenti dal gruppo per gestire chi ha accesso ai ruoli assegnati
### Ambienti
Di seguito riportati gli url degli ambienti creati:
* Ambiente di sviluppo: [https://dev-pagopa.crm4.dynamics.com/](https://dev-pagopa.crm4.dynamics.com/)  
* Ambiente di test: [https://uat-pagopa.crm4.dynamics.com/](https://uat-pagopa.crm4.dynamics.com/)  
* Ambiente di produzione: [https://pagopa.crm4.dynamics.com/](https://pagopa.crm4.dynamics.com/)


----

#### Rif. 
* [1_PagoPA_MM_Sessione_20241004_v1.1](https://docs.google.com/document/d/1GTad8IEvvKHjZOjb_HWC4Cl4mOQG-Dtg/edit?usp=sharing&ouid=109593398864246406190&rtpof=true&sd=true)
