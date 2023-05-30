# Voorbeeld 2

Deze keer gaan we terug de gegevens bij houden van personen.    
Nu dien je echter wel eerst zelf op SQL Server een nieuwe database aan te maken :   
  * Naam database = **ScalaAdovb2**  
  * Je maakt in deze database 1 tabel aan.  Naam = **Personen**  
  * Aan deze tabel voeg je volgende kolommen toe :   
    *  Id, nvarchar(50), primaire sleutel  
    *  Naam, nvarchar(50), vereist  
    *  Voornaam, nvarchar(50), vereist  
    *  Adres, nvarchar(50)  
    *  Gemeente, nvarchar(50)  
    *  Geboortedatum, datetime, vereist  
    *  Soort, nvarchar(50), vereist
  
In de starterscode zit enkel een WPF project (Xamll code + event handlers)  
Je maakt dus zelf een class-library aan : **Scala.Adovb2.Core**  
Je voegt 2 mapjes toe aan deze class-library : **Entities** en **Services**   
Kopieer uit de cursus of het vorige project (in het mapje **Services**) de klassen **Helper** en **DBServices** : pas in **Helper** de sql connectiestring aan.   
Installeer via Nuget Packages **System.Data.SqlClient**  
Voorzie in het mapje **Entities** 1 entiteitsklasse **Persoon** die een weerspiegeling is van de tabel die je zonet maakte.  
Voorzie in het mapje **Services** nog een klasse **PersoonService** die : 
  * De beschikbare personen aanlevert, al dan niet gefilterd op soort.  
  * Een persoon toevoegt  
  * Een persoon wijzigt  
  * Een persoon verwijdert  

Het WPF project ligt voor de hand : personen afbeelden, toevoegen, wijzigen en verwijderen.  
Bijkomend : personen moeten kunnen gefilterd worden op soort.  We voorzien hiervoor een combobox (**cmbFilter**) waarin we tijdens het opstarten 3 waarden steken : 
  * Familie
  * Vrienden
  * Andere
 
De code wordt uiteraard uitvoerig tijdens de les besproken.   
