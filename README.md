# Windy API v3.1

![](assets/intro.gif)

## Getting started
Windy API enables you to create your own Windy Apps with minimum effort. You do not need any server, and you can have your Windy App up & running in less than 5 minutes. 

Once you are logged in API console at [https://api.windy.com](https://api.windy.com), you can create one or more Windy Apps by adding JS, CSS or HTML code to client codes of Windy. 

Your published Windy App will be accessible on `https://mywindy.com/your-username/name-of-your-app`.

If you want to run your Windy App on your own domain, set up your own server somewhere, and embed your Windy App inside and `iframe`.

Windy API console let you edit **Javascript, CSS, Head** or **HTML** of Windy. HTML and Head content is inserted as the last element of document's `body`, or `head` section. Your javascript is wrapped inside `(function() { ... })()` so you donot need to wrap it.

Windy javascript libraries use global object `W`. 

Your Javascript code, that you will write inside the editor in API console, will be launched when document is loaded, Leaflet map is initialized, and all is up and running. Instance of Leaflet map is then available as `W.maps`.

## Examples

[1. Hello world](https://api.windy.com/myapps/59ca6222383fc346dd51a373)

[2. Leaflet, markers and pupups](https://api.windy.com/myapps/59cb613b383fc346dd51a37e)

[3. Playing with User Interface](https://api.windy.com/myapps/59cb5559383fc346dd51a376)

[4. Recieving broadcasts](https://api.windy.com/myapps/59f2d86b8944d95935cfff66)

[5. Changing overlays, levels](https://api.windy.com/myapps/59f2e0e08944d95935cfff68)

[6. Display geoJSON](https://api.windy.com/myapps/5996e7ff41c2a866967c40ed)

[7. Boat tracker](https://api.windy.com/myapps/5a0062e22c38025ff375529c)

[8. Flight tracker](https://api.windy.com/myapps/59c3714a534c3d3051e047c4)

[9. Working with weather picker](https://api.windy.com/myapps/5a03f7ec9c963a620b273cc5)

[10. Hosting your JS and CSS on your own server](https://api.windy.com/myapps/5a032a029c963a620b273cbb)

## Using ES6
Our examples use ES6 syntax, but there is no traspilation of Javascript code. Whatever you write, will go directlly to client's browser so use ES5 if you want to cover older browser. 

## Conditions to use
Windy API is free for time being, but Windy logo must remain visible and clickable in your App. Using Windy API inside native iOS or Android apps is prohibited and requires our permission. Detailed conditions are [described here](CONDITIONS.md)

## How to use Leaflet, jQuery or other libraries
leaflet library is already loaded. We use version 0.77 and we do not plan to upgrade right now. Leaflet documentation [is described here](http://leafletjs.com/)

If you want use external library (for instance `jQuery`) or some Leaflet plugin just include few lines into **head** section of your Windy App, like this.

```html
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.2.1/jquery.slim.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/lodash.js/4.17.4/lodash.min.js"></script>
```

The same philosophy can be used to host your custom JS, CSS codes on your own server. 

## Old Windy API v2.3
We are very sorry but, old API v2.3 is depreciated. We keep it running on server but we will not issue new API keys for it. We have not plan to shut it from servers down.

# CHANGELOG
### [3.1] - 11/2017
- Change of app delivery mechanism (now whole `app.html` is rendered server side with all codes included)
- CLient codes upgraded to `v12.34`

### [3.0] - 10/2017
- First version of Windy API launched, based on client codes `12.30`


