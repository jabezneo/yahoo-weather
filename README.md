# Yahoo Weather

[![npm](https://img.shields.io/npm/v/weather-yahoo.svg)](https://github.com/walchko/weather-yahoo)
[![npm](https://img.shields.io/npm/l/weather-yahoo.svg)](https://github.com/walchko/weather-yahoo)
[![Travis](https://img.shields.io/travis/walchko/weather-yahoo.svg)](https://travis-ci.org/walchko/weather-yahoo)

[![NPM](https://nodei.co/npm/weather-yahoo.png)](https://nodei.co/npm/weather-yahoo/)

There are a ton of yahoo weather modules, mine allows access to all of the information or 
just a subset.

## Usage

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

## Change Log 

| Version | Date     | Comments |
|---------|----------|----------|
| 1.0.1   | 11 Jan 16| clean up and doc updates |
| 1.0.0   | 10 Jan 16| Finally published it to npm | 
