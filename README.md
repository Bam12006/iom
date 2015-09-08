Internet of Microscopes (IoM) for Biomedical Imaging Source Code
------------------------------------------
For additional information please see IoM Project Description.pdf

uManager
https://www.micro-manager.org/

ImageJ
http://imagej.nih.gov/ij/


September 8, 2015: We want to start with a very simple IoM application. It will take an image using the demo microscope (that uManager provides) , send it the server hub application (on Microsoft Azure (C#)), and a remote user application (Javascript) can see the image. 

1. ClientMicroManager (Bahareh): Java application (that uses ImageJ and uManager API) for image acquisition 

2. ClientRemoteUser: Javascript (JQuery) application for communicating with the hub

3. ServerHub: C# hub application on the server

4. SignalRClinetJava (Luis): Java code for communication between #1 and #3. We need to customize following code to meet our needs:
https://github.com/SignalR/java-client

5. SignalRClientJavascript: Javascript code for communication between #2 and #3 (Eric). 
http://www.asp.net/signalr/overview/guide-to-the-api/hubs-api-guide-javascript-client

6. SignalRHubCSharp (Luis): C# code for communication between #1, #2, and #3. 
http://www.asp.net/signalr/overview/guide-to-the-api/hubs-api-guide-server

* Tutorial: Getting Started with SignalR 2.
http://www.asp.net/signalr/overview/getting-started/tutorial-getting-started-with-signalr

Please note #4-6 will eventually be incorporated into #1-3 and I copied all the information above into REAMDE.MD files. The names shown are the ones working on the parts. Let me know if you want to work on parts not yet assigned to any. 
