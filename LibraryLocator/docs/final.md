## Library Locator Application

**Team Members** 
Amber Dietrich, Osi Sunday, Michael Fenn, Zain Mannan, Jose Martinez

**Link to application** 
[https://enigmatic-scrubland-86362.herokuapp.com/](https://enigmatic-scrubland-86362.herokuapp.com/)

**Information Problem**
The information problem that our team decided to investigate was the accessibility of libraries and their services in Prince George’s County. We wanted to ease the process of understanding where libraries are in the county and what each of these libraries has to offer. Prior to our project development, individuals had to search through multiple pages on the Prince George’s County Memorial Library System Website, which takes time and effort. To solve this information problem we thought to create a web application that not only acts as a visual representation of where all of the libraries are in comparison to the user, but also what specific services each library has to offer. Our project will help any Prince George’s County residents who may not have a reliable computer or internet access at home. Having access to computers can be helpful for people who may need to do certain things such as, doing research or writing documents that they may be unable to do on their smartphones or smaller devices. The stakeholders in this situation are the general public of PG County, which includes, parents, teens, college students, and individuals. Our map will assist any resident who may not know where the closest libraries are, but also which specific services can be found at each one. Services like internet connection and printing are all common at the libraries within the Prince George’s County Memorial Library System, but some branches offer other services that could be useful like passport services, small study rooms, and Senior SmarTrip. Existing applications like GoogleMaps provide information about library locations, but not which services are available there, so that is an additional reason why we decided to create this application.

Libraries not only function as places to find books and study but also as community centers. They offer many different kinds of events such as camps for children, English classes, citizenship classes, and academic tutoring. Knowing where a library is and which services it offers, will benefit the residents of Prince George’s County.

**Stakeholders and Target Browsers**
The stakeholders will be anyone that uses our application, so the residents of Prince George’s County who want to know where the nearest library is and which services are at each library. We have catered our application to what we expect these users to need and what resources they may be looking for. We also have a survey that users can complete, which will help us update the application in the future based on any new needs that users have.

**Data Worked With**
[https://data.princegeorgescountymd.gov/Education/Libraries/7k64-tdwr](https://data.princegeorgescountymd.gov/Education/Libraries/7k64-tdwr)

We used the Libraries dataset from the Prince George’s County Open API website for our data. This dataset lists all of the libraries in Prince George’s county. The dataset has five columns which include branch name, address, zip code, telephone, and branch type. We used the address data, specifically the longitude and latitude, to plot on the map where each library was.
[https://www.pgcmls.info/website/library-services-4567](https://www.pgcmls.info/website/library-services-4567)
We then went to Prince George’s County Memorial Library System website to get information about the different services offered at each branch. We manually inputted this data into a JSON dictionary.

**Chosen Strategies and Solutions for the Problem**
To solve our information problem we created an interactive map that displays where the user is and where each library in the county. To see the map the user must enable location services, so it can plot their location and show the nearest libraries within a two-mile radius. This allows for users to find libraries that they can walk to, which is helpful for individuals who may not own a car. All of the libraries in the API are plotted using their longitude and latitude. Each library provides helpful information for the user including the name, address, phone, and services of each library. Users can, therefore, use the map to not only see which libraries are closest to them but also see if the library offers the services that they are looking for. We ended up just focusing on the libraries in the Prince George’s County Memorial Library System because these are all public and free libraries that offer a variety of services that would be useful. We narrowed it down to these libraries after evaluating more specifically who are users would be. We thought that these libraries would be more of what residents would be visiting on a daily basis. If other libraries, like university ones, are found to be highly requested through user feedback, we can always adjust our application to include them.

**Technical System Decision Rationale**
To create the skeleton of our service and the website, our group decided to use HTML and CSS instead of using React or Bootstrap. We chose to do this because we were most familiar with those languages and were confident in our ability to build a website using them. We also used some JavaScript (specifically the library fullpage.js) to make the website function in a professional and aesthetic manner.

For our visualization, we used leaflet.js to build an interactive map that pinpoints the user’s location as well as the location of the libraries around them. We decided to use leaflet.js because it is user-friendly and simplistic. For our visualization, we did not require an intricate map to display the information necessary. A simple, clean display was enough to convey the information since we are not including directions from the user’s current location to the library.

To keep our website organized, we used a flexbox to create a grid where we laid out our information. This allowed for our website to be visually pleasing and consistent.

**How/If Our Final System Helps to Address the Problem**
Our final system helps to address the problem because it provides a visualization of the nearest libraries and information about each library that other mapping services do not provide. Users will be able to look at each specific location and decide based on the services listed, which library they will go to. We even included a two-mile radius, so users can know which libraries are walkable. We also put a list of helpful and unique services to each library, so users can better know which library they should go to when looking for a specific service.

**Challenges Faced and Impact on Final Design**
When working on our project there were areas that we had trouble with, but we made sure that we worked together as a team in order to deal with them. One of the issues we faced early on was working with the map. None of us had experience with leaflet.js, so we had to read up about it in order to better understand how it worked. We were able to get it to work successfully after this. Another difficult thing regarding our project was the actual API. It only provided very limited information, so we had to manually get a lot of the more specific information, such as library services and URLs from the actual library website. This did not really impact our final design, just that it was a bit more time-consuming in getting all of the information that we wanted to display. To get the map to display the user’s location, their location services need to be activated so it can be plotted on the map. We found it hard to get this information without having the user allow their location to be shared, so, for now, the only way our map displays the user’s location is if the user gives permission for their location to be used. We also wanted to change the color of the tick mark for the user, but we found it too tricky and were not able to figure out how to do it. To allow the user to know which mark is theirs, we put a text pop-up that says “You are here.”

**Possible Future Work Directions with this Problem**
Some future work that we could do with this project would be to improve the overall design of the website. Right now each library has a block of text that pops up and lists information, but this can be quite blocky looking as more services are added. In the future, we could find a better way to display this. Another idea is to allow for the filtering of which libraries can pop up. For example, users could filter by which libraries offer Senior SmarTrip cards or the map could be expanded to include libraries in different counties or states, allowing for more people to find the app useful, rather than just those looking for a library in Prince George’s County.

Another idea is to provide even more detailed descriptions of what can be found at each library. This will allow users to know exactly what is at each location. Right now, we only have a handful of the services listed, but if we were to continue improving this application, we would make sure we did not miss any services. Something related to this idea would be to somehow display the calendar of recent events for each library too. Our project currently just has a link to where that information is on the website, so at least users do not have to search for that. But, we would like to find a way to display it on our application.

A final idea for the future would be to allow users to find the fastest route from their location to the library of their choice. They could see how long it would take to get there and we would basically have a GPS feature in our app, so users would not have to rely on other applications to get directions.

We have included a survey on our website, so users can provide feedback. This will allow us to know if our app is not only successful but also what else users would like to see on it.