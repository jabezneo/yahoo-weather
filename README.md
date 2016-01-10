# Yahoo Weather

There are a ton of yahoo weather modules, mine allows access to all of the information or 
just a subset.

# Usage

    var yw = require('weather-yahoo');
    var ans = {};
    yw.getSimpleWeather('denver,co').then(function(res){
        console.log(res);
        ans=res;
    }); // pulls just some of the info from yahoo weather
    
    yw.getFullWeather('denver,co').then(function(res){
        console.log(res);
        ans=res;
    }); // returns full yahoo weather json


