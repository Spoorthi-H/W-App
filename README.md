<! —Project Title →
# Weather App
<! — Introduction — the project’s aim →
## the Project’s Aim
Aim of this project to build a App that displays the current weather of the specified city
<! —Tools and technologies →
## Tools & Technologies stack
HTML5
Css3
ReactJs
ExpressJs
NodeJs
Git

### Packages installed
express
body-parser
cors
nodemon

### How to run the project
First, run the backend(i.e server) using the command: nodemon server
The server runs on http://localhost:5000
Then run frontend(i.e client side) using the command: 
npm start 
The client run at http://localhost:3000

### Apply cors policy:
app.use((req, res, next) => {
    res.setHeader('Access-Control-Allow-Origin', 'http://localhost:3000');
    res.setHeader('Access-Control-Allow-Methods', 'GET, POST, PUT, DELETE');
    res.setHeader('Access-Control-Allow-Headers', 'Content-Type');
next();
  });
  
### Project Description
The project is built to implement the Weather App.
When the project is run, the user enters the city name in the search bar.
The city name is sent to the server using axios post request.
The server makes request to the external server that is to the openweathermap api with city name and api key. The request is made using https.get.
The response from the openweathermap api is returned to the frontend that is to the user which gives city’s current weather.
The interface of the App displays city, it’s temperature in degree celcius on the button click.

### openweathermap api
'https://api.openweathermap.org/data/2.5/weather?q='+city+'&appid='+apikey+'&units=metric'
City:’cityname’ eg: London
Apikey: user’s unique openweather key



