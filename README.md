# Geog 458 Essay: The Radio Garden
## Jackson Shaw
The Radio Garden is an interactive web map that displays the locations of radio stations all around the globe and allows users to tune in to radio stations through their browser, from anywhere in the world, based on their broadcast city.

![Radio garden map of the US](/img/Map_radio.png)

The map was first developed in 2016 by Studio Puckey & Moniker, a company based in the Netherlands, and was commissioned as an exhibition project by the Netherlands Institute for Sound and Vision in the context of the research project Transnational Radio Encounters. Since the exhibition, Johnathon Puckey (the man behind Studio Puckey & Moniker) has since made Radio Garden an independent company and has been "tending to the garden", as he puts it, ever since. The map is intended for anyone to use, but has recently redesigned its entire display and experience to cater to mobile users, as its most popular version is in the form of mobile applications.

The data used in the map to display and link to radio stations is maintained by the developers, and must be fairly responsive, as it has an option to add or change data pertaining to radio stations via a submitted form.

The radio broadcast program works by having a user first select a city, which populates the stations pane with:
1. A list of all radio stations broadcasting from the selected city, ordered alphabetically
2. A list of the most popular stations from the selected city (if the city has more than six stations)
3. A curated list of "Picked Stations" from the area surrounding the selected city
4. A list of the most popular stations from around the country containing the selected city
5. A list of the closest cities to the selected city
6. A list of the cities in the country containing the selected city that have the most radio Stations

From there, the user can select a radio station based in the selected city, and the program will connect the client browser to the selected station.

Additionally, the user can choose to "favorite" stations that they enjoy, which add them to a list in the "Favorites" tab of the stations pane. They can also, as of 2019, search for a city or station directly.

The map uses a number of libraries and technologies to display and manipulate the data it uses, including:

- Cesium's 3D Globe model
- Satellite imagery from a number of sources, including ESRI, the USGS, AeroGRID, GeoEye, and the GIS user community
- Free Geoip's geolocations
- React's user interface
- Rematch's predictable state container

In terms of map components, the map is displayed on a 3D globe model using satellite imagery, but lacks common map features, like scale bars, north arrows, and legends. Each of the cities is displayed with a green dot, the size of which indicates the number of stations based there.

This map is an interesting hybrid of simple and complex design. On the one hand, as it is a free web service that is designed to be usable by anyone, it is very easy to use and understand; but on the other, its use of satellite imagery makes it seem visually cluttered. Clearly, this is intended to make the globe model more genuine; pasting a street map around a globe would not work in this context. But, the satellite imagery can tend to obscure the green points representing cities with fewer radio stations, as they do not visually contrast with some of the terrain displayed as part of the basemap.

On the whole, the application is easy to use, fun to play around with, and provides a useful service. 
