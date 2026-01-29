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
