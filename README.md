# VONA-alert-light
Un dispositivo elettronico capace di mostrare il livello di allerta dell’emissione della cenere vulcanica dell’Etna (indicato nel più recente comunicato VONA) attraverso un LED..


![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdfQsHug61evHYBKZ-YGyH91-3xZjieyA-C2-sKjOfzpad5EejSaPCt1hrZDcvhGv3HFQXglxm8h8V2u12b5AiUlOn7-nXVA82Tes9Ik_6Lu1MjzJ7ANN2Jp0pPIrDib7QmGy_LjQ?key=buQ2jXQKaaDo5jNF0tqy7w)

# TPS³ – progetto TPSIT **verticale** per il **triennio** 

VONA Alert Light

## 🧩🧠🎓

## **🔧💡📐**

## **🌍🧭📦**

## 🧩 

## Cosa voglio realizzare?

| **Un dispositivo elettronico capace di mostrare il livello di allerta dell’emissione della cenere vulcanica dell’Etna (indicato nel più recente comunicato VONA) attraverso un LED.** |
 | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | 

L’Etna è uno dei vulcani più attivi al mondo e le sue frequenti eruzioni esplosive generano alte colonne di cenere che possono interferire con il traffico aereo, in particolare presso il vicino aeroporto di Catania.

Per monitorare questi eventi e ridurre i rischi per l’aviazione l’Istituto Nazionale di Geofisica e Vulcanologia (INGV) ha introdotto nel 2014 i comunicati VONA (Volcano Observatory Notice for Aviation). Si tratta di notifiche ufficiali inviate ogni volta che si verifica un’eruzione significativa e servono ad allertare in tempo reale le autorità aeronautiche.

Alla caduta della cenere sono interessati anche i cittadini che vivono alle pendici dell’Etna dovendo far fronte ai disagi che la cenere provoca sulle loro case, sui giardini e sulle automobili.

Nasce quindi l’esigenza (didattica) di monitorare lo stato di allerta.

## 🧠 

## Cosa devo conoscere per realizzarlo?

Per realizzare il progetto è necessario avere una conoscenza, anche di base, dei seguenti argomenti:

| **microcontrollore ESP32** | **linguaggio Python** | **HTML e DOM** |
 | -------------------------- | --------------------- | -------------- | 
| **protocollo HTTP** | **linguaggio PHP** | **RDBMS MySQL** |
| **CAD 2D e 3D (facoltativo)** | **Laser cutter (facoltativo)** |  |

Nel coinvolgere colleghi e studenti in modo da riuscire a realizzare il progetto in un solo anno scolastico, si suggerisce l’uso di strumenti di collaborazione e project management (propri della materia GPOI) come Trello, Gantt e il repository Git.

## 🎓 

## Quali anni sono coinvolti e in che modo?

Il progetto si suddivide in tre fasi:

1.  monitoraggio ed estrazione del comunicato VONA dal sito dell'INGV
    
2.  servizio di cache con salvataggio su DB locale dei dati estratti
    
3.  servizio RESTful API per l’interrogazione dell’ultimo bollettino restituito in JSON
    
4.  visualizzazione dello stato corrente dell’alert recuperando i dati tramite API RESTful attraverso un microcontrollore e un LED
    

Le attività da svolgere per realizzare il progetto sono state suddivise nel triennio della materia TPSIT secondo lo schema seguente:

| **3° anno – microcontrollori e SoC** |
 | ------------------------------------ | 

*   capire cos’è un microcontrollore e come si programma
    
*   utilizzare ESP32 per controllare componenti semplici (es. LED RGB)
    
*   sviluppare programmi con interfacce testuali (Arduino IDE) e visuali (STEAMakersBlocks)
    

| **4° anno – web scraping e DB** |
 | ------------------------------- | 

*   python per il web scraping
    
*   utilizzo del DOM
    
*   estrazione dati da PDF
    
*   salvataggio nel DB
    

| **5° anno – RESTful API e DB** |
 | ------------------------------ | 

*   uso di RDBMS per lo storage dei dati
    
*   framework per l’implementazione di API RESTful in PHP
    
*   il formato JSON per la restituzione dei dati
    

E’ inoltre prevista un’attività trasversale da eseguire opzionalmente nel corso del triennio:

| **trasversale – realizzazione del package** |
 | ------------------------------------------- | 

*   progettazione del package per la stampa in 3D
    
*   progettazione del package per il taglio e l’incisione laser
    

### **🔧** 

### Come lo realizzo?

Breve panoramica della **sequenza operativa** o delle fasi del progetto.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXc9Lf_O4jBl4n2b6HlaH7tfyG-ucG-SP_q23k_Ave_XJyVaTr3xORgV47P3RoakW6LMp9gDiCy5-uAeULhsls2WvQEmuc2PmgEHgod7O2cQnNOYr-sSS3H2gR78CRQtkAWBR9zWtA?key=buQ2jXQKaaDo5jNF0tqy7w)

Il progetto si suddivide in tre fasi:

5.  monitoraggio ed estrazione del comunicato VONA dal sito dell'INGV
    
6.  servizio di cache con salvataggio su DB locale dei dati estratti
    
7.  servizio RESTful API per l’interrogazione dell’ultimo bollettino restituito in JSON
    

### visualizzazione dello stato corrente dell’alert recuperando i dati tramite API RESTful attraverso un microcontrollore e un LED

### **💡** 

### Quali strumenti, software, materiali o tecnologie servono?

*![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcIhPZ9FOXKClk3KPUXjefKJsFwfQd2fESrhfVv52h-u3PYoeySIBuz4zE3cagd7YYAeYsGruQDBM4_SY5WcxVRoHGfZO2zX9vRIe4bmh_PbJdwV-B7C2_0qd-ajnmfrF_dGs1ZYQ?key=buQ2jXQKaaDo5jNF0tqy7w)*

E’ necessario avere a disposizione un SoC **ESP32**, **ESP8266** o il più recente **Arduino R4** che integrando il modulo WiFi dispongono di un accesso a internet. Valutare l’eventualità di utilizzare una scheda con presa RJ45 per una connessione via cavo.

Il sistema luminoso di avviso è realizzato da un LED RGB adatto per le tensioni di uscita a 3,3V.

*![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfMEDr1N7qCX7pRBRRtQIlIRsojGSvrljDK9XTDnEiiP9gf0TIzqLoEnoSpOMcHim3XktBBq4nEIEfzWdHufYpBxw7RFLeRxIKpcgt_X36rypBE-QTyq9cVI7cQZny7OTUQESrs?key=buQ2jXQKaaDo5jNF0tqy7w)*

Con python vengono usate le librerie:

*   **requests** per l’accesso alla pagina web dell’INGV
    
*   **htmldom** per il parsing del DOM 
    
*   **PdfFileReader** per estrarre il testo dal comunicato INGV in PDF
    

*![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdY70ljYVUyihvG08RhtHu11qoDsF8lxFZ65MBH_fmINl8OcHUbK6Kco1Yi8CVRoXbD-70MauLPtYtQ3k0uVzUAE0QKH1j4nuGi5tZ_NaeI-YxHJZPToO_8P0RsC9xEnwPOYlLU?key=buQ2jXQKaaDo5jNF0tqy7w)*

In PHP si fa uso del framework **Micron** per realizzare il server delle API RESTful che verrà interrogato dal microcontrollore.

*![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcVW-H4x8HXnZC7I8jFY1FnvlNkLzKHRA33WG6TOWIbiAoVmSzY9IzKrjL9Lt4_aEVeh_EPTBXYQLa-TIcTH6Cy7ViKVyGaVxvnOEbXeIn3v1y9Js1QRogA2f4Sh-c059G0zLjn?key=buQ2jXQKaaDo5jNF0tqy7w)*

Il database **MySQL** (o MariaDB) viene usato per conservare le informazioni aggiornate recuperate dal comunicato VONA. Qui viene effettuato un accesso in scrittura da python (che recupera e scrive i dati) e in lettura da PHP (che restituisce i dati al microcontrollore).

*![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdkKWz4CpKATuxvXfpe4q6Dm0GC0pcQGHLEaP2bUmOaQa2dXsgMnZZRf_Qg6a4qYq-S60g1YMGQyGAnaSizWzDJnB-Tz8IyAw5CExsOQyp0aPxxEt6_wuImPkh7CaHKKxlM9CVHzg?key=buQ2jXQKaaDo5jNF0tqy7w)* *![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXc8jAi-8x-JevL7I_lmnUD9BU4IoY5EVIx--6GQYmoff4mfH2ZA_yJaEabNb7zqb0GAV6ou8gmgZ57A5o_quWyAepudbAYNTMTcaxFBPUfiXZk3bNN55g54PKRDN0NqmTOMTdBN?key=buQ2jXQKaaDo5jNF0tqy7w)*

CAD 2D e 3D vanno scelti tra quelli open source conosciuti dai colleghi e che possano gestire i formati supportati dal software specifico della laser cutter in possesso. 

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXe0kItjFSEVtAUQuQSF9br7PQdfzFY44-6s1Qj5Ev3F-DGr_3rwyvagHcwW4G4V1KHn_cK2vx5Drbb-ssWV_1VTLtmsdBv3LNKGs8__DvU6S8ujUQlJycVc0QLBECm6nTHJvjS3rA?key=buQ2jXQKaaDo5jNF0tqy7w)    ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXczV8luiUOEB2ujIesLdVj1U8QDr8NtJx-kesoJB9Lx1vVZcDRT2tXKaFXL3AgO2hSkIa9oN6p6wXKvmEQ-72wOvba0MZtKGZMmJ3qT3kUPwlzwgc5s9Wf-zUtp7dygoPc54_4quw?key=buQ2jXQKaaDo5jNF0tqy7w)

Tool per il project management, la condivisione dei sorgenti e la collaborazione tra docenti e studenti delle classi verticali.

### **📐**

## Come valuto il lavoro?

Non è necessario effettuare la valutazione una tradizionale valutazione. L’esperienza maturata nel realizzare questo progetto sarà evidente con il rilascio del prototipo e della sua installazione all’interno dell’istituto scolastico.

Tuttavia sono identificabili alcuni criteri generali per misurare il livello raggiunto:

*   competenze tecniche
    
*   collaborazione
    
*   spirito di iniziativa
    
*   presentazione/documentazione
    

### **🌍** 

## Perché ha senso farlo?

Realizzare questo progetto mette alla prova la capacità organizzativa dei docenti nello svolgere un’attività verticale interessando le classi del triennio: dare notizia al dipartimento risulta fondamentale per trovare partner disposti a mettersi in gioco.

Dal punto di vista degli studenti, il progetto realizza una connessione con il mondo reale mettendo in pratica quanto appreso durante la didattica ed ha anche un impatto territoriale coinvolgendo il vulcano e i rischi che questo può generare.

Non si trascura inoltre:

*   il lavoro di gruppo e la collaborazione interclasse
    
*   la condivisione dei ruoli tra classi del triennio
    
*   la comunicazione efficace tra team con competenze differenti
    
*   la pianificazione e la gestione del progetto
    
*   l’organizzazione in fasi operative
    
*   il rispetto delle scadenze
    
*   creazione di documentazione tecnica
    
*   presentazione del progetto per il sito dell’istituto
    
*   problem solving e debugging
    

### **🧭**

## Cosa posso documentare durante il percorso?

Diario di bordo, video, foto dei prototipi, repository di codice, relazioni, ecc.

### **📦** 

## Cosa potrebbe diventare in futuro?

Spazio aperto a miglioramenti, evoluzioni, versioni successive, repliche con altri gruppi, ecc.