# webapps
This is a standalone application developed with minimal dependencies. Only Java JDK installation is required. 

Steps to deploy the application

download the zip file and extract the files in CashManATM.
Click on the CashManATM.bat file to run the application
Application will get launched through command prompt.
Command prompt is the user interface.

Application displays the Amount it has and the count of denominations of each 20's and 50's 
each transactions details are maintained in CashManATM.csv file which is in CashManATM\src folder.

All transactions are logged in the csv file. Application does not log details if CSV is in use by any other person.

This application provides below Feature Set

 The device will have a supply of cash (physical bank notes) available.
It must know how many of each type of bank note it has. It should be able to report back how much of each note it has. 
It should be possible to tell it that it has so many of each type of note during initialization. After initialization, it is only possible to add or remove notes. 
It must support $20 and $50 Australian denominations. 
It should be able to dispense legal combinations of notes. For example, a request for $100 can be satisfied by either five $20 notes or 2 $50 notes. It is not required to present a list of options. 
 If a request can not be satisfied due to failure to find a suitable combination of notes, it should report an error condition in some fashion. For example, in an ATM with only $20 and $50 notes, it is not possible to dispense $30. 
Dispensing money should reduce the amount of available cash in the machine. 
Failure to dispense money due to an error should not reduce the amount of available cash in the machine. 

For an ATM-style of machine (with $20 and $50 notes), the following dispensed amounts are of particular interest
·         $20 
·         $40
·         $50
·         $70
·         $80
·         $100
·         $150
·         $60 
·         $110
·         $200, when there is only 3x$50 notes and 8x$20 notes available.

Optional Feature Set

The controller should dispense combinations of cash that leave options open. For example, if it could serve up either 5 $20 notes or 2 $50 notes to satisfy a request for $100, but it only has 5 $20 notes left, it should serve the 2 $50 notes. 
The controller needs to be able to inform other interested objects of activity. Threshold notification in particular is desirable, so that the ATM can be re-supplied before it runs out of cash. (partially completed)
Persistence of the controller is optional at this time. It can be kept in memory. However, it should go through a distinct initialisation period where it is told the current available amounts prior to being used.(partially completed) CSV has the transaction log details

Application displays the Threshold notification and all combinations of cash outcome at each stage but for initialization of amounts need to manually enter the amount and denominations in CSV file at this stage.

