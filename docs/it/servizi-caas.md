# Servizi Container as a Service (CaaS)

Nella seguente tabella è possibile consultare i servizi afferenti alla categoria Container as a Service (CaaS).

| FAMIGLIA | SOTTO-FAMIGLIA                      | NOMENCLATURA SERVIZI              |
| -------- | ----------------------------------- | --------------------------------- |
| Compute  | Confidential - Kubernetes - Private | Kubernetes Confidential Computing |

## Compute

Di seguito le sotto-famiglie afferenti alla famiglia Compute:

- Confidential - Kubernetes - Private

### Confidential - Kubernetes - Private

Di seguito l'elenco dei servizi afferenti alla sotto-famiglia Confidential - IaaS - Private:

- Kubernetes Confidential Computing

**Descrizione del servizio**

Servizio che permette l'erogazione di una pittaforma per l'orchestrazione di container privati e sicuri, progettati per gestire applicazioni containerizzate in ambienti altamente regolamentati o con requisiti di riservatezza.
Offe un ambiente Kubernetes sicuro e controllato in cui la componente di sicurezza è uno degli aspetti principali della soluzione. Il sistema operativo su cui la soluzione si basa è hardenizzato, al fine di ridurre al minimo la superficie di attacco e di possibili vulnerabilità. 
All'interno delle componenti architetturali della soluzione sono utilizzati meccanismi che permettono di garantire la sicurezza del dato anche nelle fasi di comunicazione (tramite meccanismi di crittografia applicate di default alle comunicazioni tra le componenti di piattaforma) e nei dati memorizzati all'interno della piattaforma stessa.
La piattaforma può essere personalizzata per adattarsi alle esigenze specifiche di ogni Organizzazione, garantendo l'integrazione con sistemi e applicazioni aziendali esistenti.

**Funzionalità e Vantaggi del servizio**

La realizzazione richiede una combinazione di hardware certificato per Confidential Computing, un'infrastruttura Kubernetes privata rinforzata a livello di sicurezza, e un insieme di tool di osservabilità e governance per mantenere il controllo totale sul ciclo di vita dei container.
Funzionalità incluse:

- *Protezione dei dati* → il sistema operativo è configurato per garantire la protezione in tutte le sue fasi: dati in memoria, tramite crittografia completa del disco e rotazione delle chiavi; dati in transito, utilizzando protocolli di comunicazione sicuri e crittografati; dati in uso, adottando pratiche di Confidential Computing e ambienti di esecuzione sicuri.

- *Enclave sicure* → applica isolamento e crittografia, garantendo che solo le parti autorizzate possano accedere ai dati.
- *Ambienti di esecuzione attendibili (TEE)* → aggiunge un ambiente di elaborazione sicuro, proteggendo i dati dalle minacce esterne.

Essendo una soluzione Kubernetes gestita il cliente non dovrà occuparsi della gestione dell'infrastruttura e della sua complessità, in quanto il layer infrastrutturale viene gestito da Leonardo durante tutto il ciclo di vita del servizio.

I vantaggi offerti sono:

- Sicurezza e riservatezza delle applicazioni containerizzate: crittografia end-to-end, confidential computing per i workload, isolamento dei container su nodi dedicati con protezione hardware-based, policy di sicurezza integrate e RBAC avanzato;
- Controllo e governance centralizzati dei cluster
- Scalabilità e flessibilità;
- Integrazione con ambienti multicloud e legacy.