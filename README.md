# DevFinder
A simple app to add, list and search for developers near you. Using: ReactJS, ReactNative, Node.js


Some useful requests to the backend:

#GET - Get a list of all Devs:

Send a GET request to '/devs'


#GET - Search for a devs

Send a GET request to '/search' using query params
Ex.
http://localhost:3333/search?latitude=-20.123456longitude=-30.123456techs=ReactJS,%20Angular


#POST - Create/Save a new Devs

Send a post request to '/devs' with github_username, techs (separated with ', '), latitude and longitude
Ex.
{
	"github_username" : "exampleName",
	"techs" : "ReactJS, React Native, Node.js",
	"latitude": -20.123456,
	"longitude": -30.123456
}
