# weatherforecast
This project process data from Weather Forecast API and generate the graph based on Time Vs Temperature in Fahrenheit. 

This project process data from Weather Forecast API and generate the graph based on Time Vs Temperature in Fahrenheit. The graph is updating every five second based on the data received from Weather Forecast API. It has Node Framework based backend application(SERVER-WEATHER-FORECAST) as well as React Framework based frontend application (APP-WEATHER-FORECAST). Semantics UI is used for CSS. 

######################################################################################################################################################################################

#SERVER-WEATHER-FORECAST
This server is based on the Node framework. It is used to interact with Weather API (https://api.weatherapi.com/v1/forecast.json?key=3738897fde7047f0a1822737203011&q=20171&days=1) and process the data as per the requirements.

Server.js: This is the initial point of the server. Middleware API like Express, Cors, Fetch API has been used to process the request.
http://localhost/forecastdata:  This is the url to display the processed json data as per the requirement.

Command to start Server:  node server.js


######################################################################################################################################################################################
#APP-WEATHER-FORECAST
This frontend application is based on the React framework. It is used display the graph between the Temperature in Fahereint and Time of the current day. It interacts with the SERVER-WEATHER-FORECAST and retreive the Temperature-Time data as per the requirement. The data is pulled every 5 seconds of time difference.

ForecastChart.js: This is the initial point of the application. Here, Semantics UI CSS is used for formating the application as per the requirements. react-google-charts Module has been used for generating the Line graphs. Fetch API has been used to interact with SERVER-WEATHER-FORECAST and process the data accordingly. The concept of polling has been coded in utils.js. It calls the fetch method every 5 seconds.     

Command to start Application:  npm start
 
