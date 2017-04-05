# openSearch-Postman-client

[openSearch](http://www.dbc.dk/produkter-services/webservices/open-search), udstiller et API bestående af en række services, som er beskrevet i https://opensource.dbc.dk/services/open-search-web-service.

API'et kan også tilgås fra en web klient i browseren. Se de mulige service endpoints under overskriften "Versions" under https://opensource.dbc.dk/services/open-search-web-service/.

Hensigten med dette Github repository er at:
* Give biblioteksmedarbejdere mulighed for at se de data openSearch API'et via Postman klienten.
* Dele en Postman collection bestående af et antal foruddefinerede forespørgsler til openSearch.
* Beskrive hvordan man installerer postman.
* Beskrive hvordan man importerer FBS Postman collectionen.
* Beskrive hvordan man benytter environment variables til at autentificere FBS, bestemte brugere mv.

Målgruppen er webmastere der ønsker at se de data FBS udleverer til f. eks. DDB CMS.

FBS Postman collection giver mulighed for at hente følgende oplysninger fra FBS:

* Search
* getObject
* info

Se https://opensource.dbc.dk/services/open-search-web-service/ for nærmere beskrivelse af de tre kald.

## Installér Postman klienten

Postman er gratis værktøj med en grafisk brugergrænseflade, der kan installeres på Windows, Mac og Linux computere, og den egner sig derfor godt til brugere, som undertegnede, der ikke færdes hjemmevant i en kommandoprompt og ikke kan programmere op imod et API.

Postman kan downloades fra https://www.getpostman.com/ og installeres som ethvert andet program, og det forudsætter derfor også administratorrettigheder at installere.

## Importér openSearch.postman_collection

"openSearch postman collection" er en samling af kald som er defineret ud fra https://opensource.dbc.dk/services/open-search-web-service/.

Tryk på linket https://raw.githubusercontent.com/rolfmadsen/openSearch-Postman-client/master/DBC%20openSearch.postman_collection.json
Tryk CTRL+S for at downloade filen, og gem den på dit skrivebord.
Åben Postman
Tryk på "Import" knappen i den øverste grå menu linje og tryk på "Choose Files" knappen i det Import vindue der dukker op midt på skærmen.
Dobbelt-klik på "openSearch postman collection" filen på dit skrivebord for at importere den.

## Benytte Environment variables

Postman giver mulighed for at benytte Environment variables, der er variabler gør det let at skifte imellem forskellige FBS miljøer, Lånere mv.

Det er hensigtsmæssigt at oprette flere Environments og jeg har lagt seks forskellige i dette repository.

1. Tryk på linket for henholdsvis:
  * https://raw.githubusercontent.com/rolfmadsen/openSearch-Postman-client/master/DBC%20openSearch%20(Br%C3%B8nd%203.0%20-%20opensearch.addi.dk-4.0.1).postman_environment.json
  * https://raw.githubusercontent.com/rolfmadsen/openSearch-Postman-client/master/DBC%20openSearch%20(Br%C3%B8nd%203.0%20-%20opensearch.addi.dk-b3.0_4.3).postman_environment.json
  * https://raw.githubusercontent.com/rolfmadsen/openSearch-Postman-client/master/DBC%20openSearch%20(Br%C3%B8nd%203.5%20-%20opensearch.addi.dk-b3.5_4.3).postman_environment.json
  * https://raw.githubusercontent.com/rolfmadsen/openSearch-Postman-client/master/DBC%20openSearch%20(TESTBR%C3%98ND%203.5%20-%20oss-services.dbc.dk-opensearch-4.2).postman_environment.json
  * https://raw.githubusercontent.com/rolfmadsen/openSearch-Postman-client/master/DBC%20openSearch%20(TESTBR%C3%98ND%203.5%20-%20oss-services.dbc.dk-opensearch-4.3).postman_environment.json
  * https://raw.githubusercontent.com/rolfmadsen/openSearch-Postman-client/master/DBC%20openSearch%20(TESTBR%C3%98ND%203.5%20-%20oss-services.dbc.dk-opensearch-4.5).postman_environment.json
2. Tryk CTRL+S for at downloade filen, og gem filen på dit skrivebord
3. Åben Postman
4. Tryk på tandhjulet i øverste højre hjørne
5. Tryk på "Manage environments"
6. Tryk på "Import" knap nederst i "Manage environment" vinduet.
7. Tryk på Vælg filer knappen "Manage environment vindue der dukker op midt på skærmen.
4. Dobbelt-klik på en af de environment filer du har downloadet til dit skrivebord for at importere den.

Herefter kan man vælge de kald man ønsker at udføre og trykke på den blå "Send" knap.

Hvis man har oprettet flere Environment variables, f. eks. hvis man har forskellige versioner af openSearch man gerne vil teste kan man skifte imellem environments i den drop down menu der ligger øverst til højre ved siden af "øjet" og "tandhjulet".
