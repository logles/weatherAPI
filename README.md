# weatherAPI

Build a weather dashboard application that calls the OpenWeather API and renders data in the browser.

## Weather Dashboard

The application’s front end has already been created. It's your job to build the back end, connect the two, and then deploy the entire application to Render.

Under Create Key, give your API key a name that's unique to your project, then click the Generate button. This will take you to a page that lists any keys that you've created. They should look like a random string of 32 characters. Copy the new key that you've created, and save it in the JavaScript file where you'll be making API calls.

Key: b5731a5bf64664fdb1a09f71619f661b
Name: weatherAPI

## Getting Started

On the back end, the application should include a searchHistory.json file that will be used to store and retrieve cities using the fs module.

The following HTML route should be created:

GET \* should return the index.html file.
The following API routes should be created:

GET /api/weather/history should read the searchHistory.json file and return all saved cities as JSON.

POST /api/weather should receive a city name to save on the request body, add it to the searchHistory.json file, and then return associated weather data to the client. You'll need to find a way to give each city name a unique id when it's saved (look into npm packages that could do this for you).

Refer to the Full-Stack Blog on deploying to RenderLinks to an external site. and the Render documentation on setting environment variablesLinks to an external site..

## Hints

Using the 5-day weather forecast API, you'll notice that you'll need to pass in coordinates instead of just a city name. Using the OpenWeatherMap APIs, how could we retrieve geographical coordinates given a city name?

How could we make the OpenWeather API calls server-side, parse the data, and then send the parsed data client-side?
