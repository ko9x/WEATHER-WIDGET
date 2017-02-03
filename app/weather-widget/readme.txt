Here are the dependancies for this weather widget component
{
  "license": "UNLICENSED",
  "repository": {
    "type": "git",
    "url": "https://github.com/ko9x/WEATHER-WIDGET.git"
  },
  "dependencies": {
    "@angular/common": "2.1.2",
    "@angular/compiler": "2.1.2",
    "@angular/core": "2.1.2",
    "@angular/forms": "2.1.2",
    "@angular/http": "2.1.2",
    "@angular/platform-browser": "2.1.2",
    "@angular/platform-browser-dynamic": "2.1.2",
    "@angular/router": "3.1.2",
    "angular-in-memory-web-api": "0.1.13",
    "bootstrap": "4.0.0-alpha.5",
    "core-js": "2.4.1",
    "font-awesome": "^4.7.0",
    "reflect-metadata": "0.1.8",
    "rxjs": "5.0.0-beta.12",
    "systemjs": "0.19.40",
    "zone.js": "0.6.26"
  }
}



Add this script tag to the index html to get the Skycons working

<script src="app/weather-widget/js/skycons.js"></script> //  THIS PATH COULD BE DIFFERENT BUT THE NEEDED FILE IS IN THE JS FOLDER



You will also need to import the following to your app module


import { JsonpModule, HttpModule } from '@angular/http'; //  IF NOT ALREADY IMPORTED

import { WeatherComponent } from './weather-widget/component/weather.component'

import { SpeedUnitPipe } from './weather-widget/pipe/speed-unit.pipe';
import { TempUnitPipe } from './weather-widget/pipe/temp-unit.pipe';



The WeatherComponent selector is weather-widget


