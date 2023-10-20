# Ex-04_RESTful_Web_Services
## Aim:

To create, deploy and execute RESTful Web service programs using Server, Client and Client-Side remote invocation
## Procedure:

### Server side:
Step 1: Create a new Java Web Project. Follow Steps 1-5 as in SOAP Based Web Service.

Step 2: Right-click on the project name and select New->RESTful Web Services from Patterns.

![image](https://github.com/kannan0071/Ex-04_RESTful_Web_Services/assets/119641638/99f32ea8-f53c-46db-888f-afca546a023c)

Step 3: A new window will appear. Select “Simple Root Resource” and click Next.
 
 ![image](https://github.com/kannan0071/Ex-04_RESTful_Web_Services/assets/119641638/15d066b5-9bac-42d7-b595-767cbb08774f)

Step 4: In the next window, give a Resource Package name and choose MIME Type as “text/html”. Click Finish.

![image](https://github.com/kannan0071/Ex-04_RESTful_Web_Services/assets/119641638/23d20718-7a45-401a-ad26-5577d10f1b9a)

Step 5: Two editing tabs will appear. Close “ApplicationConfig.java”. You need to write all your required functionalities in GenericResource.java.

Step 6: Alter getHtml() method as shown below.

Step 7: Save your project, clean and build it. Deploy your project.
 
![image](https://github.com/kannan0071/Ex-04_RESTful_Web_Services/assets/119641638/c0cb1d9e-886f-4896-aa88-a4bcf261877e)

Step 8: To test your web service, open a new browser window/tab and type the URL as http://localhost:8080/project_name/webresources/generic?params=45&params=35 and hit enter. (This is the easiest way of testing the web service when it makes use of List).


Client-Side:

Step 1: Create a new Java Web Project. Follow steps 1-5 as in section 1.1.

Step 2: Right-click on the project and select New->RESTful Java Client.

![image](https://github.com/kannan0071/Ex-04_RESTful_Web_Services/assets/119641638/8d8ae95b-f2bc-4264-96ee-5ee0b8144245)

Step 3: A new window will appear. In that, give a name to your client, a package name and select “From Project” under the “Select the REST resource:” tab and click Browse. Step 4: Carefully select your RESTful resource (web service) and click OK.

Step 4: Carefully select your RESTful resource (web service) and click OK.

![image](https://github.com/kannan0071/Ex-04_RESTful_Web_Services/assets/119641638/d48995d7-03f2-442b-bc4e-63d8c45a87b6)

Step 5: Once everything is filled, the New RESTful Java Client window should look like this. Click Finish.

![image](https://github.com/kannan0071/Ex-04_RESTful_Web_Services/assets/119641638/0581ba28-4e4a-46e7-bd60-071100029a58)

Step 6: An editing tab will open. Alter getHtml() method with the following.

![image](https://github.com/kannan0071/Ex-04_RESTful_Web_Services/assets/119641638/1e73e1f9-056d-4408-bde8-992333bf2840)

Step 7: Right-click on the Libraries folder under your project and select “Add JAR/Folder”.

![image](https://github.com/kannan0071/Ex-04_RESTful_Web_Services/assets/119641638/a3de49e1-0dff-42ce-9b86-c93359d15339)

Step 8: A new window will appear. Navigate to the folder where you have placed the “javax.ws.rs-api2.0.1.jar” file and select Open.

![image](https://github.com/kannan0071/Ex-04_RESTful_Web_Services/assets/119641638/d87518fe-47f9-43d7-b4df-2da66e1d0f0a)

Step 9: Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.

Step 10: A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.

![image](https://github.com/kannan0071/Ex-04_RESTful_Web_Services/assets/119641638/f908fbce-ce46-423e-9b45-31977bdbf61b)

Step 11: Save the project and build it.

Step 12: Run the JSP file and you should see the output in a new browser window.
 
![image](https://github.com/kannan0071/Ex-04_RESTful_Web_Services/assets/119641638/bb6c2396-729d-4d4f-9a0c-a654711514cf)

Client-Side Remote Invocation:


Step 1: Follow steps 1-5 as in Section 2.2

Step 2: In the generated NewJerseyClient.java file, Replace BASE_URI from private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources"; TO private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";

Step 3: Follow steps 6-12 as in Section 2.2

## Result:
 Thus, the RESTful web service program has been successfully created and executed.
