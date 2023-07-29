1- There's a file named "ExcelUtility" that has the export file inside of it called "ExcelUtilty". Export the zip file.

2- Import the project file into your desired IDE (It is preferred if you use Eclipse).

3- In eclipse, right click on the project and click properties. Then go to Java Build Path.

4- Click on JavaFX17 then click edit. Then click User Libraries. Then click new.

5- Name it "JavaFX17". After adding, click on it again then click Add External JARs.

6- From the submission file you've downloaded, you can see a file called javafx-sdk-17.0.1. Go inside it and go to a file named "lib" then choose all jar files within it.

7- Click Apply and Close. Then check and uncheck the box in front of JavaFX17 library then click finish.

8- Now, check the library and see if all jar files has been added to JavaFX17 in the module path. If it didn't, click edit, check and uncheck JavaFX17 once more, then click finish.

9- The project is created in maven so there should be maven dependencies. Make sure there are jar files inside of that are related to poi library. If there isn't, add the dependency. you 
can do so within a file named "pom.xml".

10- Click on the project file and click Run Configurations.

11- In main tap, make sure that the project is the one that contains the ExcelUtility export. Do that by clicking browse then choosing the right project.

12- Go to arguments tap then copy paste the following into the VM Arguments box:
 --module-path "PASTE_YOUR_PATH_HERE_THAT_CONTAINS_THE_JARS_FILES_RELATED_TO_JAVAFX/javafx-sdk-17.0.1/lib" --add-modules javafx.controls,javafx.fxml,javafx.web,javafx.graphics,javafx.media
-Dcom.sun.webkit.useHTTP2Loader=false

   Important note: if you're copy pasting your path, make sure that the slashes are forward. like "/" not "\".

13- Run the program and it should work! Ignore everything that appears in the console. It just shows info that has been imported from the excel file.

14- There's an excel file that is dealt with internally from within the project file. If you would like to use yours, put it on the file named "data" within the ExcelUtility file.
    Make sure that you rename your file to "Competitions Participations". Same thing goes for the email template file, make sure you rename it to "EmailBodyTemplate".

15- Have fun!

