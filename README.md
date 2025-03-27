# Gestione Ordini Ristorante
Crea un piccolo sistema PHP che simuli la gestione degli ordini di un ristorante. Il sistema dovrà:
✅ Utilizzare superglobali ($_POST, $_GET) per gestire il passaggio dei dati
✅ Utilizzare array (sia indicizzati che associativi)
✅ Implementare funzioni per la gestione dei dati
✅ Gestire JSON per salvare e recuperare gli ordini
✅ Applicare la programmazione ad oggetti (OOP)

🛠 Requisiti
1- Pagina di Ordine (index.php)
- Creare un form HTML con i seguenti campi:
    - Nome del cliente (name);
    - Selezione del piatto (dish) → (es. Pizza, Pasta, Insalata);
    - Quantità (quantity)
- Il form deve inviare i dati con POST a process.php.

2- Gestione dell’ordine (process.php)
- Recuperare i dati inviati con $_POST.
- Controllare che tutti i campi siano stati compilati.
- Creare un array associativo per rappresentare l'ordine (nome cliente, piatto, quantità, prezzo totale).
- Salvare l’ordine in un file JSON (orders.json).

3- Visualizzazione Ordini (orders.php)
- Leggere i dati dal file JSON.
- Mostrare tutti gli ordini in una tabella HTML.

4- Implementare una Classe Ordine
- Proprietà: $nomeCliente, $piatto, $quantità, $prezzo.
- Metodo calcolaPrezzo() che imposta il prezzo in base al piatto scelto.
- Metodo salvaSuJSON() per salvare l’ordine nel file JSON.

📌 Struttura dei File
/progetto_ristorante
│── index.php      → Pagina del form d'ordine
│── process.php    → Logica di gestione e salvataggio
│── orders.php     → Visualizzazione ordini
│── orders.json    → File JSON per salvare gli ordini
│── Ordine.php     → Classe per la gestione degli ordini

🎯 Obiettivi e Concetti Utilizzati
✅ Super Variabili Globali ($_POST) per gestire l'input dell'utente
✅ Condizioni e Controlli per verificare che tutti i dati siano validi
✅ Array Associativi per rappresentare gli ordini
✅ JSON per salvare e recuperare gli ordini in modo persistente
✅ Programmazione ad Oggetti (OOP) per organizzare il codice con una classe Ordine
✅ Metodi e Proprietà per calcolare il prezzo e salvare i dati
✅ File Handling (file_get_contents, file_put_contents) per leggere e scrivere su un file

💪 Sfida Extra
1- Aggiungi un'opzione per eliminare un ordine;
2- Aggiungi una sessione ($_SESSION) per mostrare un messaggio di conferma dopo aver inviato un ordine;
3- Migliora il codice con il concetto di ereditarietà (ad esempio, una classe Pasto e una classe Ordine che la estende).

(Consegna presente nella chat Intervista PHP Tecnica)