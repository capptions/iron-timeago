sc-geolocator
============

Polymer 1.0 element that offers geolocation, based on https://github.com/onury/geolocator

`sc-geolocator` is an invisible element that offers a couple of methods to detect the location of the user.

It uses both HTML5-geolocation (GPS / Wifi) if allowed by the user and supports fallback to IP-geo lookup.

- HTML5 geolocation (by user permission)
- Location by IP (Supported source services: FreeGeoIP, GeoPlugin, WikiMedia)
- Reverse Geocoding (address lookup)
- Full address information (street, town, neighborhood, region, country, country code, postal code, etc...)
- Fallback mechanism (from HTML5-geolocation to IP-geo lookup)

The element has the following public properties:

- `locating`: a boolean indicating if the element is currently busy retrieving the location
- `location`: an object that contains the retrieved location
- `fallbackToIP`: fallback to IP-geo lookup if HTML5-geolocation fails (`true`)
- `timeout`: allowed time for HTML5-geolocation to happen (`6000`)
- `maximumAge`: maximum age of the geolocation returned (`0`)
- `enableHighAccuracy`: use high accuracy geolocation (`true`)

The element has one method called `locate` which needs to be fired without any arguments to start a new location lookup.

It fires either a `success` or `error` event when the lookup has completed.

Example value of the `location` property once a lookup was successful:

```js
{
  address: {
    city: "New York",
    country: "United States",
    countryCode: "US",
    neighborhood: "Williamsburg",
    postalCode: "11211",
    region: "New York",
    street: "Bedford Avenue",
    streetNumber: "285",
    town: "Brooklyn"
  },
  coords: {
    accuracy: 65,
    altitude: null,
    altitudeAccuracy: null,
    heading: null,
    latitude: 40.714224,
    longitude: -73.961452,
    speed: null
  },
  formattedAddress: "285 Bedford Avenue, Brooklyn, NY 11211, USA",
  ipGeoSource: null,
  timestamp: 1360582737790
}
```

Contributions welcome, please create issues!