## Library Locator Application

**Description** 
This application was created to help all Prince George's County residents, (which includes parents, teens, college students, and others) combat the problem of lacking access to computers or reliable internet connection at home by providing an app that will display the nearest libraries to them on a map. We created an interactive map that pinpoints different libraries in the county based on the location of the user and the location of possible destinations. We also included services that each library offers to help residents figure out which library suits their needs. The address and contact information of each library has also been provided to help people contact and locate libraries of choice.

  **Link to Heroku Application** [
  https://enigmatic-scrubland-86362.herokuapp.com](https://enigmatic-scrubland-86362.herokuapp.com)
  
**Description of target browsers** 
This application is capable of running on all modern browsers, which includes Chrome, Firefox, Safari, Internet Explorer, and etc.

** [Link to User Manual](https://drive.google.com/file/d/1FIsxx6KMBxeoa6-E8yyWSsHD_ljL1Xdt/view?usp=sharing) **
** [Link to Developer Manual](https://docs.google.com/document/d/14rsH_CzjXin884hOHW-kBhxmEbJ3mn3oWwoHLqa1IRk/edit?usp=sharing)**

## Developer Manual

**Installing Application and all Dependencies**
There are no external dependencies required to be installed for this application to run. All the necessary code to run the application can be found in the LibraryLocator repository.

The JSON, CSS, and index.html files are found in the LibraryLocator repository. The Javascript code can be found within the index.html file.

**How to Run Application on a Server**
-   Preliminaries:
	- Download CLI | [https://devcenter.heroku.com/articles/heroku-cli](https://devcenter.heroku.com/articles/heroku-cli)
    - Download Git | [https://git-scm.com/book/en/v2/Getting-Started-Installing-Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
    - Download NPM | https://nodejs.org/en/download/
    
-   Running Application on Server
    -  Open your command-line tool
    - Navigate to the repository in which you have the code held in
    - Run *Heroku login* on your terminal and type in your credentials
    - To ensure that the app is correctly downloaded, you will want to run it locally by typing *Heroku local web*
	    - To check, open up your preferred browser and type in the search bar *localhost:5000*. A local version of the app should appear.
-   If changes must be made to the code, enter the following:
	- *git add .*
	- *git commit -m “More”*
	- *git push https://git.heroku.com/enigmatic-scrubland-86362.git master*

**All the endpoints and what they do**
When calling each endpoint, the user will receive a string that provides information about the website. Each of the endpoints, GET, POST, and PATCH, are easily accessible for the users to gain more information about our site. When these are used, the API will request information and then print out a response for the user.

**Future Application Development**
 - Have services of each library appear in a table below or beside the
   map so the map itself is not overcrowded.
 - Include a filter component on our application that will allow users to choose which libraries appear on the map based on the location and services of each library.
 - Expand the map to include libraries in different counties or states, rather than only including a small list of public libraries within Prince George’s County.
 - Provide a more detailed description of the resources and services found at each library location to inform users about what the library has to offer. For example, the application might display the calendar of recent events for a library, once the user selects a location.
 - Implement a GPS feature to our application that would provide users with the fastest route from their current location to the library of their choice. Additionally, provide the users the option to change the mile radius on the app. Right now, there is a two-mile radius from any user’s location.
 - Currently, the map displays the markers based on the information from the PG County Library API. In the future, implement an error-handling mechanism that displays a message if the Library API does not at work at any given time the application is open.
