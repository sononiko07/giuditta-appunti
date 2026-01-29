# LEZIONE 1

### 1. ICT (Information and Communication Technology)
*   **Definizione:** Studio dei metodi per memorizzare ed elaborare le informazioni in modo automatico e le loro applicazioni quotidiane.
*   **Ambiti applicativi:** Produttività d'ufficio, navigazione Web, comunicazione (e-mail, messaggistica), e-commerce, home-banking, e-government e intrattenimento.

### 2. Dati e Informazione
*   **Informazione:** È la risposta a una domanda che riduce l'incertezza di chi la riceve.
*   **Dati:** Rappresentano l'informazione codificata per poter essere scambiata ed elaborata.
*   **Il Bit (Binary Digit):** Unità di misura dell'informazione. Un bit è la quantità di informazione sufficiente a **dimezzare l'incertezza** (annullandola se le scelte sono solo due). I valori convenzionali sono 0 e 1.
*   **Capacità e Multipli:**
    *   Con **$n$ bit** si possono rappresentare **$2^n$** possibilità.
    *   **1 Byte = 8 bit** ($2^8 = 256$ combinazioni), ideale per rappresentare numeri 0-255 o singoli caratteri alfanumerici.
    *   Esempi di grandezze: Fotografia ($\approx$ 1 MB), Film ($\approx$ 1 GB).

### 3. Il Computer e la Risoluzione di Problemi
*   **Ruolo del Computer:** Aiuta a risolvere problemi di carenza di informazione. Il computer **non crea** informazione inesistente, ma elabora i dati forniti (**Input**) per produrre informazioni utili (**Output**).
*   **Definizione di Problema:** Partire da informazioni note (Input) per ricavare informazioni ignote (Output).
*   **Funzione Caratteristica ($f_p$):** Relazione matematica che associa l'insieme dei possibili input ($I_P$) a quello dei possibili output ($O_P$). Risolvere un problema significa calcolare $f_p(i)$.

### 4. Modelli di Calcolo: Macchina di Turing (MdT)
*   **Definizione:** Modello astratto delle capacità di calcolo di un computer, composto da un nastro infinito e una testina di lettura/scrittura.
*   **Elementi:** Alfabeto di simboli, insieme di stati (iniziale e finali) e funzione di transizione $\delta$.
*   **Tesi di Church-Turing:** Ogni funzione calcolabile meccanicamente può essere calcolata da una MdT. Un problema è risolvibile se esiste una MdT che ne calcola la funzione caratteristica.

### 5. Algoritmi ed Esecutori
*   **Esecutore (Macchina Astratta):** Poiché la MdT è laboriosa, si preferiscono "esecutori" capaci di operazioni complesse.
*   **Algoritmo:** Sequenza di istruzioni finita, non ambigua ed eseguibile dall'esecutore che giunge alla soluzione partendo dai dati.
    *   **Esempio (MCD di Euclide):** Richiede all'esecutore di saper gestire confronti, operazioni aritmetiche, assegnamenti e salti (condizionati e incondizionati).
*   **Equivalenza:** Due algoritmi sono equivalenti se producono lo stesso output per ogni input (stessa funzione), pur potendo differire per efficienza.

### 6. Complessità Computazionale
*   **Definizione:** Misura le risorse necessarie in funzione della dimensione dell'input.
    *   **Complessità Temporale:** Numero di passi di calcolo.
    *   **Complessità Spaziale:** Quantità di memoria (celle) utilizzata.
*   **Criterio di Accettabilità:** Un algoritmo è considerato accettabile se la sua complessità è **polinomiale**. Esistono problemi risolvibili la cui complessità è talmente alta da rendere impossibile la soluzione in tempi utili.

### 7. Algoritmi e Programmi
*   **Semantica:** Le regole di un linguaggio di programmazione definiscono un esecutore.
*   **Programma:** È la traduzione di un algoritmo in un linguaggio di programmazione specifico per essere eseguito.
*   Gli algoritmi sono solitamente progettati per esecutori astratti facilmente traducibili nei linguaggi di programmazione imperativi più comuni.


# LEZIONE 2

### 1. Fondamenti di Informatica e ICT
*   **ICT (Information and Communication Technology):** Studio dei metodi per memorizzare ed elaborare automaticamente le informazioni.
    *   *Applicazioni:* Produttività (Office), Web, Comunicazione (mail), E-commerce, Home-banking, E-government, Intrattenimento.
*   **Informazione e Dati:**
    *   L'**informazione** riduce l'incertezza del ricevente (risposta a una domanda).
    *   I **dati** sono informazione codificata per essere elaborata.
*   **Unità di misura (Bit):** Il **bit** (binary digit) è la quantità di informazione sufficiente a dimezzare l'incertezza.
    *   $n$ bit rappresentano $2^n$ valori.
    *   **1 Byte = 8 bit** ($2^8 = 256$ possibilità, sufficiente per un carattere alfanumerico o numeri 0-255).
    *   Esempi di grandezze: Foto $\approx$ 1 MB; Film $\approx$ 1 GB.

### 2. Risoluzione di Problemi e Algoritmi
*   **Problema:** Passare da informazioni note (**Input**) a ignote (**Output**) calcolando la **Funzione Caratteristica** ($f_p$). Il computer non crea informazione, ma elabora quella fornita.
*   **Macchina di Turing (MdT):** Modello astratto composto da un nastro infinito e una testina. È caratterizzata da un alfabeto $A$, stati $S$ e una funzione di transizione $\delta$.
    *   **Tesi di Church-Turing:** Ogni funzione calcolabile meccanicamente è calcolabile da una MdT.
*   **Algoritmo:** Sequenza finita di istruzioni non ambigue ed eseguibili che porta alla soluzione.
    *   *Esempio:* Algoritmo di Euclide per l'MCD (confronti, sottrazioni, salti e assegnamenti).
    *   **Equivalenza:** Due algoritmi sono equivalenti se producono lo stesso output per ogni input (stessa funzione), ma possono differire per **Efficienza** (passi di calcolo e memoria usata).
*   **Complessità Computazionale:** Numero di passi (**Temporale**) o celle di memoria (**Spaziale**) necessari in funzione dell'input. Si considera accettabile se è **polinomiale**.
*   **Programma:** Algoritmo espresso in un linguaggio di programmazione (definito da una semantica).

### 3. Rappresentazione dell'Informazione e Cambiamenti di Base
*   **Sistemi Posizionali:** Il valore di una cifra dipende dalla sua posizione (Base 10, Base 2, Base 8, Base 16 con A-F).
*   **Conversioni:**
    *   **Da Base N a 10:** Somma di ogni cifra per la potenza della base corrispondente alla posizione ($c_i \cdot N^i$).
    *   **Da Base 10 a N:** Divisioni intere successive per $N$; il risultato è dato dai **resti** letti dall'ultimo al primo.
*   **Logica Binaria:** I computer usano il binario (0 e 1) perché i dispositivi digitali hanno solo due stati elettrici: **0 (SPENTO/0V)** e **1 (ACCESO/5V)**.

### 4. Rappresentazione dei Numeri (Interi e Razionali)
*   **Interi non negativi (Unsigned):** Con $n$ bit si rappresentano valori da $0$ a $2^n-1$ (es. 1 Byte: 0-255).
*   **Numeri con Segno:** Il bit più a sinistra (MSB) indica il segno ($0 = +$, $1 = -$).
    *   **Complemento a 2:** Metodo standard per i negativi. Si invertono i bit del positivo e si somma $1_2$. Permette di avere una sola rappresentazione dello zero.
    *   Range con 1 Byte: da **-128 a +127**.
*   **Numeri Razionali (Virgola):**
    *   **Conversione decimale:** Si moltiplica la parte frazionaria per 2, prendendo la parte intera risultante come cifra binaria.
    *   **Virgola Fissa:** Numero di bit prestabilito per parte intera e decimale. Semplice ma poco precisa e con intervallo limitato.
    *   **Virgola Mobile (Floating Point):** Notazione scientifica $N = \pm m \cdot b^e$. Composta da: **Segno** (1 bit), **Mantissa** (precisione) ed **Esponente** (ampiezza intervallo).
        *   *Float:* 32 bit (1 segno, 23 mantissa, 8 esponente).
        *   *Double:* 64 bit (1 segno, 52 mantissa, 11 esponente).

### 5. Rappresentazione Alfanumerica
*   **Codice ASCII:** Convenzione universale che associa sequenze di bit a caratteri (es. 'A' = 65 in decimale = `01000001`). In genere 1 Byte = 1 Carattere.


# LEZIONE 2.A

### 7. Codifica delle Immagini
Le immagini sono un continuo e per essere rappresentate digitalmente richiedono due passaggi:
1.  **Discretizzazione (o Campionamento):** Divisione dell'immagine in un insieme di parti discrete chiamate **pixel** (*picture element*). L'immagine viene trattata come una matrice.
2.  **Quantizzazione:** Associazione di un numero (codice binario) a ogni pixel per descriverne il colore o l'intensità.

*   **Risoluzione:** Definita dal numero di pixel che compongono l'immagine. Una risoluzione alta (più pixel) corrisponde a un'immagine più definita.
*   **Profondità di bit per pixel (bpp):**
    *   **1 bit:** 2 informazioni (es. Bianco/Nero).
    *   **8 bit (1 Byte):** 256 colori o livelli di grigio.
    *   **24 bit (3 Byte):** Circa 16 milioni di colori (True Color).

### 8. Formato Bitmap (o Raster)
Il formato bitmap utilizza una mappa di colori associando a ogni pixel un colore specifico.
*   **Toni di grigio:** Si usa 1 byte (8 bit) per pixel (0=bianco, 255=nero).
*   **Colori RGB (Red, Green, Blue):** Si usano **3 byte per pixel**. Ogni byte definisce l'intensità (0-255) di uno dei tre colori base.
*   **Problemi del Bitmap:**
    1.  **Occupazione di memoria:** Occupa molto spazio poiché ogni pixel deve essere memorizzato, anche se l'immagine è semplice o di un solo colore.
    2.  **Perdita di qualità:** Se l'immagine viene ridimensionata (ingrandita), sgranando perde definizione.
*   **Calcolo Occupazione di Memoria:** 
    $$\text{Risoluzione (pixel orizzontali} \times \text{verticali)} \times \text{numero di bit per pixel.}$$
    *Esempio:* Un'immagine 1800x1200 a 16 bit occupa circa 34,56 MB.

### 9. Algoritmi di Compressione
Servono a ridurre il numero di bit necessari per rappresentare i dati.
*   **Compressione Lossless (Senza perdita):**
    *   Permette di ricostruire esattamente i dati originali.
    *   Sfrutta codifiche opportune (es. assegnare meno bit agli elementi che compaiono più spesso, come nel caso di A=0 se A è il 90% dei dati).
*   **Compressione Lossy (Con perdita):**
    *   Scarta informazioni considerate "poco importanti" o impercettibili (es. piccoli cambiamenti di colore che l'occhio umano non nota).
    *   Permette livelli di compressione molto elevati, ma **non consente** di ricostruire i dati originali in modo identico.
    *   Esempi comuni: **JPEG, GIF**. È possibile bilanciare il rapporto tra qualità e livello di compressione tramite parametri.


# LEZIONE 3

### 1. Funzionalità e Architettura del Computer
*   **Compiti del Computer:** Per essere utile, deve ricevere dati (**Input**), elaborarli tramite una composizione di operazioni elementari (**Programma**) e fornire una risposta (**Output**).
*   **Architettura di Von Neumann (1948):** Modello dominante che prevede:
    *   **CPU (Central Processing Unit):** Composta da Control Unit (CU) e Arithmetic/Logic Unit (ALU).
    *   **Memory Unit:** Dove programmi e dati sono memorizzati insieme.
    *   **Dispositivi di Input/Output.**
    *   **Bus:** La linea logica di comunicazione tra i componenti (Bus indirizzi, Bus dati, Bus controllo).

### 2. La Memoria Centrale
*   **Logica:** Sequenza di celle a capacità fissata (es. 8 bit), identificate da un **indirizzo** univoco.
*   **Tipologie:**
    *   **ROM (Read Only Memory):** Non volatile, solitamente sola lettura, contiene i programmi di sistema.
    *   **RAM (Random Access Memory):** Volatile, lettura e scrittura, ospita i dati e i programmi in esecuzione.
*   **Unità di Misura:**
    *   1 byte = 8 bit.
    *   Kilo (KB) = $2^{10}$, Mega (MB) = $2^{20}$, Giga (GB) = $2^{30}$, Tera (TB) = $10^{12}$... fino all'ExaByte (EB) = $10^{18}$.

### 3. La CPU (Central Processing Unit)
*   **Funzionamento:** Esegue calcoli, interpreta ed esegue programmi alla frequenza del segnale di **clock** (misurata in Hz). Contiene celle di memoria velocissime dette **registri**.
*   **Linguaggio Macchina:** Linguaggio binario composto da un **codice operazione** e **campi di indirizzo** (operandi).
*   **Ciclo CPU:**
    1.  **Fetch:** L'istruzione in RAM viene copiata nel registro IR (Instruction Register).
    2.  **Decode:** L'istruzione viene selezionata.
    3.  **Execute:** L'istruzione viene eseguita.
*   **Famiglie:** **CISC** (istruzioni complesse, es. x86) e **RISC** (istruzioni ridotte, es. ARM).
*   **Assembly:** Linguaggio che ha una corrispondenza biunivoca con il linguaggio macchina, ma è leggibile dall'uomo tramite mnemonici.

### 4. Memorizzazione di Massa e I/O
*   **Accesso:** Può essere **sequenziale** (nastri magnetici) o **diretto** (dischi magnetici, ottici e SSD).
*   **Tecnologie:** Hard Disk (meccanici), SSD (stato solido, più veloci), CD/DVD (ottici).
*   **Parametri:** Tempo di accesso (ms) e Transfer rate (MB/s).
*   **Legge di Moore:** La complessità dei microcircuiti (numero di transistor) raddoppia ogni 18 mesi (tendenza in calo negli ultimi anni).

### 5. Il Software e il Sistema Operativo (SO)
*   **Software di Sistema (SO):** Rende le risorse hardware fruibili. Viene caricato al **boot** e rimane sempre in esecuzione.
*   **Software Applicativo:** Programmi che svolgono compiti utili per l'utente.
*   **Funzionalità del SO:**
    *   **Gestione dei processi:** Un processo è un programma in esecuzione. Il SO gestisce il passaggio tra gli stati (*new, ready, running, waiting, terminated*) tramite il *timesharing*.
    *   **Memoria Virtuale:** Astrazione che permette ai processi di usare più memoria di quella fisica disponibile, mappandola tra RAM e disco.
    *   **File System:** Un'interfaccia uniforme che organizza i dati in unità logiche (**File**) dotate di nome e locazione (cartelle).
    *   **Driver:** Programmi specifici che permettono al SO di comunicare con l'hardware tramite interfacce uniformi.

### 6. Macchina Astratta e Famiglie di SO
*   **Macchina Astratta:** Complesso hardware/software che fornisce funzionalità all'utente (interfaccia) o al programmatore (linguaggio di programmazione, es. C).
*   **Sistemi UNIX e derivati:** Nati negli anni '70, multi-utente e multi-programmato. Include Linux, Android, MacOSX (kernel FreeBSD).
*   **Sistemi DOS/Windows:** Inizialmente mono-utente/mono-programmato (MS-DOS). Evoluto con Windows NT e unificato con Windows XP.


# LEZIONE 4

### 1. Definizione di File e File System
*   **File:** Una sequenza di dati omogenei a cui è associato un nome. Spetta alle applicazioni associare un'informazione specifica ai dati (es. programmi, documenti, immagini, film).
*   **File System:** È l'interfaccia che rende la memorizzazione dei dati trasparente all'utente. Anche se i dati sono scritti fisicamente in modo diverso a seconda del supporto, il File System presenta una struttura uniforme.
    *   *Esempi:* FAT, NTFS, ext, HFS+.

### 2. Nomi ed Estensioni
*   **Case Sensitivity:** 
    *   In **UNIX/Linux** i nomi sono *case sensitive* ("Pippo.txt" è diverso da "pippo.txt").
    *   In **Windows** i nomi *non* sono case sensitive.
*   **Estensione:** È la parte del nome che segue l'ultimo punto (.). Indica convenzionalmente il tipo di file (es. `.txt` per testo).
*   **Eseguibili:** In Windows hanno solitamente estensione `.exe`, mentre in Linux non hanno estensione.

### 3. Cartelle e Struttura ad Albero
*   **Cartella (Folder/Directory):** Contenitore di file o altre cartelle, utilizzato per organizzare i milioni di file presenti in un computer. Tecnicamente, è un file speciale contrassegnato dal sistema operativo.
*   **Struttura Gerarchica:** Il file system è organizzato come un **albero**:
    *   **Nodo:** Ogni singolo file o cartella.
    *   **Padre:** La cartella che contiene un determinato nodo.
    *   **Root (/, Radice):** Il nodo principale che non ha padre.
    *   **Foglia:** Un nodo senza figli; i file sono necessariamente foglie.

### 4. Differenze tra Ambienti (Unix vs Windows)
*   **Unix/Linux:** Utilizza un'unica radice (`/`) per tutto il sistema.
*   **Windows:** Ogni unità di memorizzazione è identificata da una lettera (es. `C:`, `F:`).
*   **Separatore dei Path:** Windows usa la barra rovesciata `\` (es. `C:\Documenti`), mentre Unix usa la barra dritta `/`.

### 5. Operazioni e Cloud
*   **Operazioni comuni:** Gestite tramite il **File Manager** (es. Esplora File), permettono la creazione, copia, spostamento ed eliminazione di file e cartelle. L'eliminazione di una cartella include tutto il suo contenuto.
*   **Cloud File System:** Servizi che offrono spazio di archiviazione non locale in modo trasparente (es. **Google Drive**). Permettono di operare sui file (caricamento, download, copia, eliminazione) tramite account remoto.


# LEZIONE 5

### 1. Concetti Base e Struttura
*   **Definizione:** Il foglio elettronico è una **matrice** (griglia) composta da un numero elevato di **celle**. Serve per eseguire calcoli ripetuti in modo automatico e visualizzare risultati immediati (budget, preventivi, grafici).
*   **Coordinate:** La tabella è suddivisa in **righe** (numerate 1, 2, 3...) e **colonne** (etichettate con lettere A, B, C...). Ogni cella è identificata da una lettera e un numero (es. **A1**).
*   **Tipi di dati:** Una cella può contenere dati **testuali**, **numerici** o **date e orari**.
*   **Notazione di selezione:**
    *   `A1:B3` (due punti): indica un intervallo di celle **contigue** (da A1 fino a B3).
    *   `A1;B3` (punto e virgola): indica la selezione di celle **non contigue**.

### 2. Formule e Riferimenti
*   **Formula:** Ogni calcolo deve iniziare con il simbolo **uguale (=)**. Nella cella viene visualizzato il risultato, mentre la formula è visibile nella **barra della formula**.
*   **Tipi di Riferimento:** Fondamentali quando si copia una formula in altre celle:
    1.  **Relativo (es. A2):** Durante la copia, le coordinate cambiano mantenendo la distanza relativa tra le celle.
    2.  **Assoluto (es. $A$2):** Il simbolo **$** blocca la riga o la colonna; il riferimento non cambia mai durante la copia.
    3.  **Misto (es. $A2 o A$2):** Blocca solo la colonna ($A2) o solo la riga (A$2).

### 3. Funzioni e Logica
*   **Sintassi:** `=NOMEFUNZIONE(argomento1; argomento2; ...)`.
*   **Funzioni comuni:**
    *   `SOMMA`, `MEDIA`, `MAX`, `MIN`, `CONTA.NUMERI`.
    *   `SE`: esegue un test logico e restituisce un valore se VERO e un altro se FALSO. È possibile "annidare" più funzioni SE.
*   **Operatori Logici:** Utilizzati per test complessi:
    *   **E (AND):** Vero se tutte le condizioni sono vere.
    *   **O (OR):** Vero se almeno una condizione è vera.
    *   **NON (NOT):** Nega la condizione (inverte Vero/Falso).

### 4. Gestione Dati e Analisi
*   **Ordinamento e Filtri:** I dati possono essere ordinati secondo vari criteri o filtrati per visualizzare solo ciò che serve.
*   **Grafici:** Permettono di riassumere l'andamento dei dati in modo visivo.
*   **Tabelle Pivot:** Strumenti avanzati che offrono diverse viste dei dati, riepilogandoli (somma, media, ecc.) in modo dinamico.

### 5. Messaggi di Errore
*   `#DIV/0!`: Tentativo di divisione per zero.
*   `#RIF!`: Riferimento a una cella non più esistente o non raggiungibile (errore comune nella copia di formule).
*   `#NOME?`: Il nome della funzione utilizzata è inesistente o scritto male.
*   `#VALORE!`: Tipo di dato errato per l'operazione richiesta (es. sommare un numero a una lettera).

### Consigli pratici
*   Inserire sempre un'intestazione per ogni tabella.
*   Assegnare un singolo valore a ogni cella.
*   Evitare di lasciare righe o colonne bianche all'interno dei dati.


# LEZIONE 6
