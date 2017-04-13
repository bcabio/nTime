# nTime
UGA Hacks Fall 2016: Best Hack Overall

###Inspiration

With some of us on the team being commuters, we were tired of being late or sitting in the library waiting for class to start because traffic wasn't different on the route

###What It Does
If the user sends their origin, destination, and time it takes for them to get ready, nTime will take these variables and calculate the time the user Should wake up based on real-time traffic data. As a little aside, it also shows the user the temperature and weather of the destination. 

### How We Built It
We used an Arduino, a Raspberry Pi, a Node Web Server, a Python Script, and a text file. On the Node website, the user will input their origin (home), their destination (work), and a rough average time of how long it takes them to get ready in the morning. This site posts that into our text file, acting as our pseudo database. The python reads from this "database" and uses the info provided to calculate what time the user should wake up using Google's Real-Time Traffic API and Open Weather Map API. The python script runs constantly on the Raspberry Pi to update the database
