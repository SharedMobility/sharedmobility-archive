# Shared Mobility

Our Code for Atlanta slack channel: [#mobilize](https://codeforatlanta.slack.com/messages/C9J705RRB). &nbsp; 
Our workflow: [Trello](https://trello.com/b/qAGKrRAP/mobilize)

# 1. Fresh Produce Locations

Automate pulling Fresh Produce locations for Georgia to use with Aglanta.

[USDA Files](https://drive.google.com/drive/folders/1ZLh0eATgikkfWz1GFlCPtES8gKo8Mctf?usp=sharing) - Manually pulled from [USDA Website](https://www.ams.usda.gov/services/local-regional/food-directories-listings). Experiment with SheetSee.js.  

[Working SheetSee sample](https://codeforatlanta.github.io/mobilize/map/) in our Code For Atlanta Repo.  
[Page to point at a USDA sheet](https://codeforatlanta.github.io/mobilize/map/fresh.html) - Point at a new sheet that pulls from raw sheets. Raw sheets will be updated monthly.

# 2. Atlanta Shared Mobility APIs

Prepare request to City of Atlanta to require APIs for Shared Mobility access modeled after Los Angeles.

http://policies.sharedusemobilitycenter.org/#/policies/1044

Atlanta omitted an API requirement in the [September 2018 ordinance](https://github.com/AtlantaRides/atlantarides.github.io/blob/master/resources/ordinance/Ordinance-18-O-1322-as-Substituted-by-PSLA-on-09-25-2018.pdf), but we still have time to input a request from Code For Atlanta. You might find some more leads in this [Google search](https://www.google.com/search?q=cities+that+require+APIs+from+shared+mobility+providers&oq=cities+that+require+APIs+from+shared+mobility+providers&aqs=chrome..69i57.13920j0j7&sourceid=chrome&ie=UTF-8)

# Shared Mobility Map

Where's my next ride? Shared mobility vehicle locations (Coord.co API)

- [Atlanta Map](atlanta/) ([AtlantaRides](https://github.com/AtlantaRides/atlantarides.github.io), [KeyTopics for new dockless ordinance](https://sharedmobility.github.io/atlanta/ordinance/2018/Dockless_KeyTopics_20180731.pdf)) - 
[JSON](https://api.coord.co/v1/bike/location?access_key=p9H_wRiQaoEoIKQBaJnA1oR77yCBY-6Z-AEku8bgJNk&latitude=33.7490&longitude=-84.3880&radius_km=10)
- [Chattanooga Map](chattanooga/) ([Shared Mobility Hackathon Aug 11, 2018](https://www.eventbrite.com/e/national-day-of-civic-hacking-tickets-48338457628)) - [Writeup from the event](https://connect.chattanooga.gov/ndoch_2018/)
- [Washington, DC Map](dc/) ([Cood.co Bike-Share API](https://coord.co/quickstart/bike-share))

# Starter Kits

We've forked three starter kits for creating Coord.co API apps.
Choose one and fork it to your city's GitHub account.

- [React for Fresh Produce](https://github.com/codeforatlanta/mobilize/)
- [Vue Quasar](https://github.com/DataPortal/coord-vue-quasar) ([Detached Version](https://github.com/DataPortal/coord-quasar)) - [Bike List](https://smartparks.github.io/)
- [Angular 6 NGX](https://github.com/DataPortal/coord-angular) - MANT Stack (MongoDB Angular NestJS TypeScript) - [Bike List](https://dataportal.github.io/coord-angular/dashboard/gridmap/grid-list)


[RideMap Bike Predict](https://github.com/SharedMobility/RideMap) - Address auto-lookup and weather conditions

<b>You'll need a branch called gh-pages to publish</b>  
Otherwise the forked Master branch will appear instead of your custom site.  
In GitHub Desktop choose "Branch > New Branch" and add one called gh-pages.

<b>How to update your local branch (once you've forked an upstream master listed above):</b>  
In Github Desktop, choose menu Branch > Merge Into Current Branch > "upstream/master".  
Then click "push origin" to move update into your fork on GitHub.  
Add new pages to avoid merge conflicts with master.  
We will move the master readme files so you can maintain a unique readme file.  

# Upcoming Projects

* Get routing working in Quasar VueJS [bike list sample](https://smartparks.github.io/).

* Add direct link to Angular [bike list](https://dataportal.github.io/coord-angular/dashboard/gridmap/grid-list) (under Get Started > Mobility > Available Vehicles)

* Add Google Location auto-lookup to Coord.co shared mobility map.  
See [RideMap](https://github.com/SharedMobility/RideMap) sample. Add to [Atlanta Map](atlanta/)

* Add unique Relay Bikes icon to [Atlanta Map](https://sharedmobility.github.io/atlanta/) legend.

* Add Bird scooter and other vehicle APIs to map.

* Center the map on user's current location. Add an icon for recentering. Sample: [data.georgia.org](https://data.georgia.org)

* Combine mobile-friendly lists with map.

* Add other APIs (Air quality, wind speed, etc.) from [RideMap Bike Predict](https://bikepredict.herokuapp.com/) sample. Lazy load via modular file.

# Previous Projects

* Pull Bird scooters from the [Bird API](https://github.com/ubahnverleih/WoBike/blob/master/Bird.md). Display list with React or VueJS. Document any problems to provide to the City of Atlanta. Our findings: Bird API is not available! Needs to allow for a mile radius, okay to limit requests.

<a href="https://github.com/SharedMobility/sharedmobility.github.io">GitHub</a>
