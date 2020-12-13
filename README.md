# Project Work Videoteca

   1. Tecnologie utilizzate

	
    • Database MySql vers. 8.
    • WebServer Tomcat 9.
    • Java JDK 8.
    • Servlet/Jsp
    • Web Service RestFul

   2. Struttura del Progetto

    L’applicazione verrà realizzata secondo il Pattern MVC
   3. Descrizione entità
	     
          Le entità saranno le seguenti:
    1. Utente
    2. Film
    3. Genere
	
3.1. Utente
    
    • Id
    • username
    • password
    • email
    • ruolo
    • data di nascita

	Gli utenti saranno distinti per Ruolo fra Admin e User

3.2. Film
   
    • Id
    • titolo
    • regista
    • genere
    • anno
    • vm18
    • immagine(Opzionale)

	il campo genere sarà associato alla chiave primaria della tabella Genere 
3.3. Genere
    
    • Id
    • genere


   4. Presentazione Videoteca
  
    In questa sezione verrà descritta la componente di View relativa alla videoteca.

4.1. Pagine Pubbliche
	
    • Landing Page/Login
    • Registrazione
    • Logout
	
4.1.1 Landing Page/Login

    La Landing Page presenterà una form di Login ed un link alla pagina di Registrazione

	  Una volta loggati con successo l’utente verrà reindirizzato alla Home
4.1.2 Registrazione

	La Pagina di registrazione permetterà di agli utenti di registrarsi.
	
	Una volta completata con successo la registrazione l’utente verrà reindirizzato alla Landing Page/Login 

4.1.3 Logout

	La pagina di logout verrà visualizzata dopo aver effettuato il logout dal portale
	
4.2. Pagine Private
    
    • Home 
    • Catalogo Film
    • Aggiungi Film
    • Modifica film
    • Aggiungi Genere
    • Gestione Utenti
    • Aggiungi Utente

4.1.1 Home

	Nella Home Page verranno presentati i primi 5 film Popolari recuperati da una specifica API

	https://imdb-api.com/api#MostPopularMovies-header

	Saranno presenti inoltre i link alle seguenti pagine:

	Utente:
	
	
    • Catalogo Film

	Admin:

    • Catalogo Film
    • Gestione Utenti
4.1.2 Catalogo Film

	Nella Pagine catalogo Film verrà visualizzata una tabella con tutte le info relative ai film registrati nel sistema

	Gli utenti con età inferirore ai 18 anni non dovranno visualizzare i film vm18.

	(Opzionale) La tabella di visualizzazione dei film potrà essere ordinabile per:
	
    • Titolo
    • Anno
    • Genere
	
	L’admin oltre a visualizzare le informazioni legate al film, potrà modificare o cancellare ogni singolo record tramite apposite CTA all’interno della tabella.


	L’admin visualizzerà in Pagina i Pulsanti:

    • Aggiungi Film
    • Aggiungi Genere
4.1.3 Aggiungi Film
	
	Form aggiunta Film
4.1.4 Modifica Film
	
	Form Modifica Film
4.1.5 Aggiungi Genere

	Form aggiunta Genere
4.1.6 Gestione Utenti

	La Pagina Gestione Utenti presenterà una tabella con la lista degli Utenti.
	
	Sarà inoltre presente la CTA Aggiungi Utente
4.1.7 Aggiungi Utente
	    
    Form Aggiunta Utente
4.1.8 Logout

	In tutte le pagine private dovrà essere presente un pulsante di Logout, dopo aver effettuato la logout l’utente verrà reindirizzato sulla omonima pagina.
