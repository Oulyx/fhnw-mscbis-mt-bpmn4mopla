# fhnw-mscbis-mt-bpmn4mopla

With my Supervisor Dr. Emanuele Laurenzi and Prof. Dr. Alta Van der Merwe the following Paper resulted out of the Thesis: https://www.researchgate.net/publication/359152597_BPMN4MoPla_Mobility_Planning_Based_on_Business_Decision-Making

A downloadable ZIP of the Tool can be found here: https://kdrive.infomaniak.com/app/share/474717/25c96d64-4e84-4e73-9fa7-5aa7185bdcb5/files/12

Readme BPMN4MoPla

The DSML-Library BPMN4MoPla
Register and install the ADOxx Modelling Toolkit and the ADOxx Development Toolkit found here: https://www.adoxx.org/live/download-guided
For the Development Toolkit Startup please consult: https://www.adoxx.org/live/getting-started
 -Open the Development Toolkit
 -Click on the Library Icon (2nd from left)
 -Click on the Management Icon (Library Icon with 2 yellow arrows)
 -Import .abl file
 -The question: Create a default model group and an attribute profile group appears
 -Click Yes
 -Close the management window
 -Switch to the User management (First Icon top left)
 -Open the User list (Icon with 3 user - Pink, Grey, Pink)
 -Add
 -Enter credentials and chose the correct Application Library "BPMN4MoPla"
 -Click on User group...
 -Make sure the ADOxx is marked with a green tick
Open the Modelling Toolkit
 -Login with the newly created user
 -Click on the Puzzle (top left)
 -ADL import
 -Check "Import objects from other library"

Pre-Execution notes
To execute this process a connection to the mBot is needed. Also the task that execute the movements needs to be adapted to the IP of the bot you are using
and must be congruent with the Swagger API it is adressing.

Bee-Up execution
For the execution in Bee-Up the tool must be downloaded here: https://austria.omilab.org/psm/content/bee-up/download?view=download
 -Click on the Puzzle (top left)
 -ADL import
 -import .adl file

Camunda execution
The Camunda Modeler can be downloaded here: https://camunda.com/download/modeler/
The whole Platform including the current Tomcat server are found here:https://camunda.com/download/
Please be aware that different versions might affect how models are displayed or executed. And are dependent on the current Java Environment installed.
Otherwise the Camunda Folder used on my MacBook Pro is uploaded in the BPMN4MoPla folder here:  https://drive.switch.ch/index.php/s/zE49YcH8D3Y3xbl

Open the Camunda Folder
 -Use the start-camunda.sh/.bat depending on your Operating System
 -If neither the JAVA_HOME nor the JRE_HOME environment vairable is defined, consult: https://forum.camunda.org/t/getting-started/1526
 -Camunda starts in a browser, if not open it manually: http://localhost:8080/camunda-welcome/index.html

Open the Camunda Modeler
 -Open the travelBotOverviewProcess.bpmn
 -Click Deploy Current Diagram (the black arrow pointing upwards in the action list, located top side in the Modeler)
   - More information about the deployment can be found here: https://docs.camunda.org/get-started/quick-start/deploy/

Switch to the Browser and Press F5 in order to refresh the page.
 -Open http://localhost:8080/camunda/app/tasklist/default/#/
 -Login with the user demo and password demo
 -Start Process (top right)
 -Select the All Tasks list and select the newest Task "Define purpose and Luggage"
 -On the top right side click onto the small x next to Demo Demo
 -Select "Claim"
 -Select "Work 
