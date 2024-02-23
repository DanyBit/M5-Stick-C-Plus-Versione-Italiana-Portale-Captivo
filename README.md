M5Stick-NEMO
Firmware per scherzi ad alta tecnologia su dispositivi M5Stack ESP32
Traduzione in Italiano / Customizzazione / Bugfix / Tester IG _danybit_


Caratteristiche
TV B-Gone porta (grazie a HAKRWATCH di MrArm) per spegnere molte TV, proiettori e altri dispositivi controllati da infrarossi
AppleJuice spam di accoppiamento Bluetooth del dispositivo iOS
Spam di notifiche del dispositivo Bluetooth per SwiftPair (Windows) e Android
Spam WiFi - SSID divertenti, WiFi Rickrolling e una modalità casuale che crea centinaia di SSID con nomi casuali al minuto
WiFi NEMO Portal - Un captive portal che cerca di ingannare le credenziali email - salva nomi utente e password sulla SD Card (se inserita in un lettore supportato)
WiFi SSID Scanner - Visualizza gli SSID a 2.4 GHz nelle vicinanze, ottieni informazioni su di essi e clona gli SSID in NEMO Portal
Orologio digitale regolabile dall'utente di 24 ore supportato dal M5 Stick RTC, quindi mantiene un tempo relativamente stabile anche in modalità sleep profondo e a bassa batteria
Impostazioni supportate da EEPROM per rotazione, luminosità, oscuramento automatico e NEMO Portal SSID
Livello della batteria e crediti nel menu delle impostazioni
Interfaccia Utente
Ci sono tre comandi principali:

Home - Interrompe il processo corrente e ti riporta al menu da quasi ovunque in NEMO

Next - Sposta il cursore alla successiva opzione di menu. In modalità funzione, questo interrompe solitamente il processo e ti riporta al menu precedente.

Select - Attiva l'opzione di menu attualmente selezionata e risveglia lo schermo spento in modalità funzione

StickC e StickC-Plus

Power: Premi a lungo il pulsante di accensione per 6 secondi per spegnere l'unità
Home: Tocca il pulsante di accensione (il più vicino alla porta USB)
Next: Tocca il pulsante laterale
Select: Tocca il pulsante M5 sul lato anteriore dell'unità
Cardputer

Home: Tocca il tasto Esc/~/` o il tasto Freccia sinistra/,
Next/Prev: Tocca il tasto Giù/. e i tasti Su/; per navigare
Select: Tocca il tasto OK/Enter o il tasto Destra/?
NEMO Portal
In modalità NEMO Portal, NEMO attiva un hotspot WiFi aperto chiamato "Nemo Free WiFi" (configurabile in portal.h) con server DNS, DHCP e Web attivati.

NEMO Portal serve una pagina di login falsa che afferma di fornire l'accesso a Internet se effettui il login.
Questo è un attacco di social engineering e registrerà i nomi utente e le password inseriti sulla pagina.
Dai dettagli della scansione WiFi, puoi clonare un SSID esistente dalla lista di scansione. Uscire da NEMO Portal cancellerà l'Evil Twin SSID
Puoi visualizzare le credenziali acquisite collegandoti al portale dal tuo dispositivo e navigando su http://172.0.0.1/creds
Puoi impostare un SSID personalizzato collegandoti al portale dal tuo dispositivo e navigando su http://172.0.0.1/ssid
Se il tuo dispositivo supporta l'EEPROM per le impostazioni, l'SSID personalizzato che inserisci verrà salvato come predefinito, anche se spento.
Se il tuo dispositivo ha un lettore di schede SD con una scheda formattata con filesystem FAT inserita, i nomi utente e le password verranno registrati in nemo-portal-creds.txt sulla scheda SD per permetterti di esaminarli successivamente.
Il supporto alla scheda SD è abilitato solo di default sulla piattaforma M5Stack Cardputer. Può essere abilitato su dispositivi M5Stick, ma è necessario costruire e collegare un lettore di schede SD all'intestazione dei pin pannello frontale.
NEMO Portal è destinato solo per utilizzi professionali con un valido campo di lavoro, scopi educativi o dimostrativi. La conservazione, vendita o utilizzo di informazioni personali senza consenso è contro la legge. 🤓
Installazione da M5Burner
Questo è il modo assoluto più semplice per ottenere NEMO

M5Stick C Plus Quick Start contiene collegamenti all'app M5Burner per Linux, MacOS e Windows. Questo è lo strumento ufficiale per installare UIFlow e altri firmware ufficiali. Fornisco binari aggiornati per NEMO lì.




