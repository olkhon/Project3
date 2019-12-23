Weather-Journal App Project
Overview
This project requires you to create an asynchronous web app that uses Web API and user data to dynamically update the UI.

Instructions
This will require modifying the server.js file and the website/app.js file. You can see index.html for element references, and once you are finished with the project steps, you can use style.css to style your application to customized perfection.

Extras
If you are interested in testing your code as you go, you can use tests.js as a template for writing and running some basic tests for your code.


 to do

 Start by setting up your project environment.1. (Make sure Node is installed from the terminal)-> done.
 2. Install the packages Exprnpess, Body-Parser, and Cors from the terminal and them include them your server.js file. -> done
 3. Create a server running on the port of your choosing -> done
 4. Add a console.log() to the server callback function, and test that your server is running using Node in the terminal to run the file server.js-> done


 to do routes

 1. Add a GET route that returns the projectData object in your server code Then, add a POST route that adds incoming data to projectData. -> done
 2. The POST route should anticipate receiving three pieces of data from the request body->done
temperature
 date
 user response
 3 Make sure your POST route is setup to add each of these values with a key to projectData.
 -> JavaScript Array entries() Method

Api OpenWeatherAPp
 1 Acquire API credentials from OpenWeatherMap website. -> done
 2 Use your credentials and the base url to create global variables at the top of your app.js code. -> done
 3 Write an async function in app.js that uses fetch() to make a GET request to the OpenWeatherMap API. ->done
 4 Create an event listener for the element with the id: generate, with a callback function to execute when it is clicked.->done
 5 Inside that callback function call your async GET request with the parameters: ->done
 base url
 user entered zip code (see input in html with id zip)
 personal API key


 After your successful retrieval of the weather data, you will need to chain another Promise that makes a POST request to add the API data, as well as data entered by the user, to your # app.

 You will need to write another async function to make this POST request.
 
 1 The function should receive a path and a data object.->done
 2 The data object should include->done
 3
 temperature
 date
 user response
 Remember, you can access the value of DOM elements by selecting them in your JS code.


 Finally, chain another Promise that updates the UI dynamically Write another async function that is called after the completed POST request. This function should retrieve data from our # app, select the necessary elements on the DOM (index.html), and then update their necessary values to reflect the dynamic values for:->done

 Temperature
 Date
 User input