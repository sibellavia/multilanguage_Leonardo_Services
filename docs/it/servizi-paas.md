# Servizi Platform as a Service (PaaS)

Nella seguente tabella è possibile consultare i servizi afferenti alla categoria Platform as a Service (PaaS).


| FAMIGLIA             | SOTTO-FAMIGLIA             | NOMENCLATURA SERVIZI                                        |
| -------------------- | -------------------------- | ----------------------------------------------------------- |
| Compute              | FAAS                       | Functions as a Service                                      |
| Security             | IAM                        | Servizio di Identity & Access Management                    |
| Security             | Key Management             | Key Vault as a Service                                      |
| Middleware           | API Platform               | PaaS API Management                                         |
| Middleware           | APP Runtime                | Jboss as a Service                                          |
| Middleware           | APP Runtime                | Spring boot as a Service                                    |
| Middleware           | BPM                        | PaaS Business Process as a service                          |
| Middleware           | CMS                        | PaaS CMS as a Service                                       |
| Middleware           | ETL                        | PaaS ETL - Batch / Real Time Processing - 1 worker          |
| Infra & Ops Platform | Multicloud Management      | Multicloud Management Platform-Leonardo SCMP                |
| Infra & Ops Platform | Multicloud Management      | Multicloud Management Platform-Morpheus                     |
| Infra & Ops Platform | Observability-Infra        | Control Room as Service                                     |
| Infra & Ops Platform | Observability-Infra        | IT infrastructure Service Operations (Logging & Monitoring) |
| Infra & Ops Platform | TTM                        | PaaS Servizio di ticket management                          |
| Infra & Ops Platform | TTM                        | PaaS Servizio di ticket management (ITSM)                   |
| Infra & Ops Platform | TTM                        | PaaS Servizio di ticket management (ADD-ON ITOM)            |
| DevSecOps            | CI                         | Configuration Manager                                       |
| DevSecOps            | CI                         | Test Automation                                             |
| DevSecOps            | CI                         | Quality Code Analysis                                       |
| DevSecOps            | CI/CD                      | DevSecOps As A Service By PSN                               |
| DevSecOps            | CI/CD                      | Qualizer DevSecOps                                          |
| Big Data             | Data Lake                  | Data Lake - 1TB                                             |
| Big Data             | Data Lakehouse             | Data Lakehouse                                              |
| Big Data             | Business Intelligence      | Business Intelligence                                       |
| Big Data             | ETL                        | Batch/Real time Processing - 1 Worker                       |
| Big Data             | Event Platform             | Event Message                                               |
| Big Data             | Data Governance            | Data Governance                                             |
| AI                   | AI - Audio & Conversazioni | Speech to Text                                              |
| AI                   | AI - Image                 | OCR                                                         |
| AI                   | AI - Text                  | AI Search - AI Search - RAG - 10 GB - 1 worker              |
| AI                   | AI - Text                  | Text Analytics                                              |
| AI                   | AI - Text                  | Translation                                                 |
| AI                   | AI - Generativa            | AI SLM/LLM                                                  |
| AI                   | AI - Tools                 | AI workflow                                                 |
| AI                   | AI - Tools                 | Vector DB                                                   |
| AI                   | AI - Tools                 | AI Platforrm                                                |
| VDI                  | Virtual Desktop            | VDI                                                         |
| VDI                  | Virtual Desktop            | VDI con Supporto GPU                                        |
| Collaboration        | Communication              | Instant Messaging                                           |

## Compute

Di seguito le sotto-famiglie afferenti alla famiglia Compute:

- FAAS       

### FAAS

Di seguito l'elenco dei servizi afferenti alla sotto-famiglia FAAS:

- Functions as a Service

**Descrizione del servizio**

FaaS (Function as a Service) è un modello di progettazione di sistema, basato su eventi eseguito su container stateless, in cui gli sviluppatori creano, distribuiscono ed eseguono piccole funzioni indipendenti per eseguire attività specifiche senza preoccuparsi dell'infrastruttura sottostante.
L'adozione di un FaaS consente di standardizzare lo sviluppo e l'esecuzione delle applicazioni, centralizzando funzionalità trasversali quali orchestrazione, provisioning automatico, monitoring, gestione dei servizi integrati e controllo dei flussi event-driven.
Offre strumenti per: 

- gestire in modo centralizzato funzioni serverless;
- automatizzare il lifecycle management dei componenti;
- abilitare portabilità multi-cloud e hybrid cloud;
- supportare l'innovazione con runtime GPU e strumenti dedicati all'AI.

La piattaforma FaaS fornisce e scala le risorse sottostanti, in base alla domanda. È ideale per scenari ad alto dinamismo, con carichi di lavoro variabili, e si integra perfettamente con architetture a microservizi ed eventi.

**Funzionalità e Vantaggi del servizio**

Il servizio non si limita solo a fornire un motore di esecuzione, ma mette a disposizione un ecosistema completo, composto da: 

- *Esecuzione serverless* → funzioni stateless e workflow event-driven, scalabili e disponibili in diversi linguaggi di programmazione.
- *Portabilità e indipendenza* → eseguibile su qualsiasi cluster Kubernetes, multiambiente, senza vincoli di lock-in.
- *Sicurezza e conformità* → protezione dei dati e gestione centralizzata degli accessi.

La soluzione consente alle organizzazioni di adottare un modello moderno e flessibile, riducendo la complessità operativa e beneficiando di un servizio standardizzato e facilmente accessibile.

Il servizio è erogato tramite Apache OpenServerless, una piattaforma serverless open source, cloud-agnostic, basata su Apache OpenWhisk come Function-as-a-Service (FaaS) engine.

I vantaggi offerti sono:

- *Riduzione dei costi operativi* → si paga solo per l'effettivo utilizzo delle funzioni;
- *Flessibilità e scalabilità* →  le risorse si adattano alla domanda;
- *Efficienza operativa* →  eliminazione della gestione diretta di server, patch e aggiornamenti;
- *Elevata disponibilità* →  ridondanza e tolleranza agli errori integrate, garantendo un'elevata disponibilità delle funzioni anche in caso di guasti hardware o altre interruzioni;
- *Time-to-market accelerato* → rilascio rapido di nuove funzionalità senza preoccuparsi dell'infrastruttura;
- *Agilità nello sviluppo* → focus sul codice e sulla logica di business, non sulla gestione dei server;
- *Innovazione continua* → sperimentazione veloce di nuovi servizi a basso costo;
- *Vantaggio competitivo* di costo e velocità rispetto a modelli tradizionali di hosting.