# Banking-Application
                   WE HOPE THERE ARE BUGS,BUT WE HOPE THIS COULD BE HELPFUL TO ME WHO ARE THERE TO MAKE 'MAGIC'.
                 
                   MY PROJECT IS BASED ON THE BANKING APPLICATION.COUPLING THIS SOFTWARE WITH NECESSARY HARDWARE DEVICES,THIS COULD BE CONVERTED TO AN ATM(AUTOMATIC TELLER MACHINE).THIS IS JUST A SIMULATION OF THE NETWORK BANKINGS,.SO CAN BE CALLED AS  A MINI-ATM.
                   
                    SERVER IS DESIGNED TO BE MULTITHREADED.IT CAN TAKE OFF ANY NUMBER OF CLIENTS(WE HAVE TESTED UPTO 7 CLIENTS).FIRST THE SERVER SHOULD BE STARTED BEFORE CLIENTS GETTING ACCESS THE SERVER.SERVER SHOULD BE MADE TO RUN ON A SYSTEM,THEN CLIENTS CAN START FROM ANY OTHER SYSTEM BUT WITHIN THE SAME LOCAL AREA NETWORKS.ALSO THE PROGRAM IS WRITTEN IN SUCH A WAY THAT IT COULD TAKE THE LOOK AND FEEL OF THE SYSTEM ON WHICH IT IS RUNNING.
 

                     THE OPERATIONS AND FEATURES IN THIS ARE THOSE THAT WE CAN SEE IN ANY OTHER BANKINGS.THERE ARE THREE LEVELS OF USERS.

   1)ADMINISTRATOR:            
                    HE HAS THE POWER TO CREATE ACCOUNT,DELETE ACCOUNT,EDIT AND UPDATE ACCOUNT,VIEW ACCOUNT,VIEW ACCOUNT LOGS,CLIENT MONITORING AND PORT TERMINATION.
   
   2)INTERMEDIATE ADMINISTRATOR OR TELLER:
                      HE HAS THE PRIVELAGE TO DEPOSIT MONEY TO ACCOUNTS.
 
   3)CLIENT:
                      HE CAN VIEW HIS ACCOUNT,VIEW LOGS, TRANSFER MONEY,WITHDRAW MONEY,ACCOUNT OPTIONS SUCH AS CHANGE PIN,PASSWORD,ETC..

 
                 




 FOLDERS:

To make some order, files are placed in separate folders!

"BANKCLIENTS"  - CONTAINS CLIENTS STATION FILES.

"BANKSERVER" - CONTAINS SERVER FILES.

 PASSWORDS:

1)SERVER SIDE :
                 User id :    Administrator
                 Password:   Admin
2)CLIENT SIDE :
               -->for Teller:

                          Acct No  : Any Acct No after 1001( to where it ends)
                          Name     : Administrator
                          Password : Admin

                     He can do deposit after getting to this mode.


               -->for Clients
                          
                          Acct No  : Any Acct No after 1001( to where it ends)
                          Name     : (get it from database)
                          Password : (get it from database)

                     HE CAN DO ALL OPERATIONS EXCEPT DEPOSIT.




 IMPORTANT REMARKS:

Because of problematical setup of Java Virtual Machine on some
computers, it may be required to execute this command
before running anything:
                  

    set classpath=.

(no quotation marks!)

  NOTE:

                    As we have used access as the database, before running the server,a datasourcename should be created at the server for the mdb file.This can be done as follows:
 For Windows only,
          * Goto control panel>>ODBC DataSources
          * take the system DSN tab
          *Select the database,give the name as ServerDb
          *(Remember the name of database is ServerDb.mdb in bankserver directory)   
             

RUNNING

To start Server:
                 1. set current directory to "BANKSERVER".
                 2. type "java Server <client_port> ",
                    example: java Server 1234 
                 
To start client station:
                 1. set current directory to "BANKCLIENTS".
                 2. type "java ClientLog <host> <client_port>",
                    example: java ClientLog localhost 1234
                  (Server should be running!).
                    example: java ClientLog 192.168.0.174 1234

                  (Server should be running on machine with above IP specified)  

DETAILS OF FILES INCLUDED IN PACKAGES

      Bankserver Directory
          1)Server.java(Main File)
          2)AccessDbase.java
          3)AccessServer.java
          4)AdminCreateAcc.java
          5)AdminDeleteAcc.java
          6)AdminEditAcc.java
          7)AdminEntryLevel.java
          8)AdminMainMenu.java
          9)AdminUpdateAcc.java
         10)AdminViewAcc.java
         11)AdminViewreport.java
         
         ServerDb.mdb(Database)
 
     BankClients Directory
          1)ClientLog.java(Main File)
          2)ClientAcctOptions.java
          3)ClientDeposit.java
          4)ClientMainMenu.java
          5)ClientPassPin.java
          6)ClientTransMoney.java
          7)ClientValidatePin.java
          8)ClientViewAcc.java
          9)ClientViewLog.java
         10)ClientWithDraw.java

    11 files in Bankserver and 10 files in Bankclients.
                  


  
