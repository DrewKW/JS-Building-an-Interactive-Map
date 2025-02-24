# Mapping with Leaflet

Tailored Travel is in the process of building their new app to improve the traveler experience. You've been hired on as an independent contractor to handle the mapping and localization functionality for the app. One of the main features needed is for the user to be able to quickly locate local businesses. At the very least, the application must do the following:

Obtain the user's current location.
Map the location on a Leaflet map.
Allow the user to select a business type from a list and map the five nearest locations on the map using the Foursquare API.

data from Foursquare based on the selected business and placing markers for those locations on your map. The markers should have pop-ups containing at least the business title.

1. Connect to Foursquare
The Foursquare Places API is free, but you must create an account to use it. You'll need to obtain your client ID and client secret to access the API. Also, spend some time reading the Getting Started page which will show you how to create your account, get your API key, and see how you can use the Place Search generator to get started.

Once on the Place Search page, to the top right of the console, you'll see a 3 dot menu where you can set the language as JavaScript. Under Authentication - Header, place your API key. Then to the left, try entering a few of the paramaters. You'll need a query (place type), ll (latitude, longitue), and limit (5).

PS: When accessing the data locally, you'll most likely run into a CORS (Cross-Origin Resource Sharing) access error. What this means is that the API is blocked from accessing the data locally. To fix this, you can preface your fetch url with the following: https://cors-anywhere.herokuapp.com. This is a proxy that will make FourSquare accessable locally. In order for the proxy to work, visit: https://cors-anywhere.herokuapp.com/corsdemo. Click the link "Request temporary access to the demo server" in order for the proxy to work. You'll take a deep dive into CORS in the next course.