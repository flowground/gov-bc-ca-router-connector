# ![LOGO](logo.png) BC Route Planner **flow**ground Connector

## Description

A generated **flow**ground connector for the BC Route Planner API (version 1.3.0).

Generated from: https://api.apis.guru/v2/specs/gov.bc.ca/router/1.3.0/openapi.json<br/>
Generated at: 2019-05-07T17:42:12+03:00

## API Description

Finds shortest/fastest route between a start point and one or more stop points on British Columbia's public road network. The BC Route planner [webpage](https://www2.gov.bc.ca/gov/content?id=9D99E684CCD042CD88FADC51E079B4B5) provides additional information.  Here are some geocoded addresses to play with:<br>18 Douglas St,Victoria -123.36962,48.40892<br>1002 Johnson St, Victoria -123.355745,48.426206<br>543 Johnson St, Victoria, BC -123.36907,48.42770 <br>14 Centennial Sq, Victoria, BC -123.36564,48.42863<br>1105 Royal Ave,New Westminster  -122.92009,49.20063<br>808 Jackson Cres, New Westminster -122.90762,49.22558<br>10810 McDonald Rd, Chilliwack -121.93808,49.19859<br>3950 June Springs Rd, Kelowna -119.40751,49.83960<br>1201 Riondel Rd, Kootenay Bay -116.85402,49.74448<br>1201 Riondel Rd, Kootenay Bay -116.832759,49.730500 (parcelPoint)<br>2499 Walbran Pl, Courtenay -124.97295,49.71518<br>2013 Smoke Bluff Rd, Squamish -123.13946,49.70401<br>235 Kelvin Grove Way, Lions Bay -123.23524,49.45035<br>   Please see our <a href=https://github.com/bcgov/api-specs/blob/master/COLLECTION_NOTICE.md#collection-notice target="_blank">data collection notice</a>. 

Please note that you may experience issues when submitting requests to the delivery or test environment if using this [OpenAPI specification](https://github.com/bcgov/api-specs) in other API console viewers. 

[Developer API keys](https://github.com/bcgov/gwa/wiki/Developer-Guide#developer-api-keys) are unique and provide the ability to make up to 2 requests per second. Production government applications may use organization API keys which are further described in [the Developer guide](https://github.com/bcgov/gwa/wiki/Developer-Guide#developer-api-keys).

**To acquire an API key please visit the [API Key Request](https://kq.apps.gov.bc.ca) application.**

## Authorization

Supported authorization schemes:
- API Key
## Actions

### Get the directions, path, distance and travel time between a series of geographic points

> Represents the turn-by-turn directions, geometry, distance, and time of the shortest path or fastest path between given start and end points

*Tags:* `directions`

#### Input Parameters
* `outputFormat` - _required_ - Format of representation
    Possible values: json, kml, html.
* `points` - _required_ - A list of any number of route points in start to end order. See <a href=https://github.com/bcgov/api-specs/blob/master/router/glossary.md#points target='_blank'>points</a>
* `outputSRS` - _optional_ - The EPSG code of the spatial reference system (SRS) to use for output geometries. See <a href=https://github.com/bcgov/api-specs/blob/master/router/glossary.md#outputSRS target="_blank">outputSRS</a>
    Possible values: 4326, 4269, 3005, 26907, 26908, 26909, 26910, 26911.
* `criteria` - _optional_ - Routing criteria to optimize (e.g., shortest, fastest). Default is shortest.
    Possible values: shortest, fastest.
* `distanceUnit` - _optional_ - distance unit of measure (e.g., km, mi). Default is km.
    Possible values: km, mi.
* `roundTrip` - _optional_ - If true, route ends at start point. Default is false.
* `routeDescription` - _optional_ - Route description (e.g., Shortest route from 1002 Johnson St, Victoria to 1105 Royal Ave,New Westminster)

### Get the directions, path, distance and travel time between a series of geographic points

> Represents the turn-by-turn directions, geometry, distance, and time of the shortest path or fastest path between given start and end points

*Tags:* `directions`

#### Input Parameters
* `outputFormat` - _required_ - Format of representation
    Possible values: json, kml, html.
* `points` - _required_ - A list of any number of route points in start to end order. See <a href=https://github.com/bcgov/api-specs/blob/master/router/glossary.md#points target='_blank'>points</a>
* `outputSRS` - _optional_ - The EPSG code of the spatial reference system (SRS) to use for output geometries. See <a href=https://github.com/bcgov/api-specs/blob/master/router/glossary.md#outputSRS target="_blank">outputSRS</a>
    Possible values: 4326, 4269, 3005, 26907, 26908, 26909, 26910, 26911.
* `criteria` - _optional_ - Routing criteria to optimize (e.g., shortest, fastest). Default is shortest.
    Possible values: shortest, fastest.
* `distanceUnit` - _optional_ - distance unit of measure (e.g., km, mi). Default is km.
    Possible values: km, mi.
* `routeDescription` - _optional_ - Route description (e.g., Shortest route from 1002 Johnson St, Victoria to 1105 Royal Ave,New Westminster)

### Get distance and travel time between two geographic points

> Represents the distance and time of the shortest or fastest path between given start and end points.

*Tags:* `distance`

#### Input Parameters
* `outputFormat` - _required_ - Format of representation
    Possible values: json, kml, html.
* `points` - _required_ - A list of any number of route points in start to end order. See <a href=https://github.com/bcgov/api-specs/blob/master/router/glossary.md#points target='_blank'>points</a>
* `outputSRS` - _optional_ - The EPSG code of the spatial reference system (SRS) to use for output geometries. See <a href=https://github.com/bcgov/api-specs/blob/master/router/glossary.md#outputSRS target="_blank">outputSRS</a>
    Possible values: 4326, 4269, 3005, 26907, 26908, 26909, 26910, 26911.
* `criteria` - _optional_ - Routing criteria to optimize (e.g., shortest, fastest). Default is shortest.
    Possible values: shortest, fastest.
* `distanceUnit` - _optional_ - distance unit of measure (e.g., km, mi). Default is km.
    Possible values: km, mi.
* `routeDescription` - _optional_ - Route description (e.g., Shortest route from 1002 Johnson St, Victoria to 1105 Royal Ave,New Westminster)

### Get distance and travel time between two geographic points

> Represents the distance and time of the shortest or fastest path between given start and end points.

*Tags:* `distance`

#### Input Parameters
* `outputFormat` - _required_ - Format of representation
    Possible values: json, kml, html.
* `points` - _required_ - A list of any number of route points in start to end order. See <a href=https://github.com/bcgov/api-specs/blob/master/router/glossary.md#points target='_blank'>points</a>
* `outputSRS` - _optional_ - The EPSG code of the spatial reference system (SRS) to use for output geometries. See <a href=https://github.com/bcgov/api-specs/blob/master/router/glossary.md#outputSRS target="_blank">outputSRS</a>
    Possible values: 4326, 4269, 3005, 26907, 26908, 26909, 26910, 26911.
* `criteria` - _optional_ - Routing criteria to optimize (e.g., shortest, fastest). Default is shortest.
    Possible values: shortest, fastest.
* `distanceUnit` - _optional_ - distance unit of measure (e.g., km, mi). Default is km.
    Possible values: km, mi.
* `routeDescription` - _optional_ - Route description (e.g., Shortest route from 1002 Johnson St, Victoria to 1105 Royal Ave,New Westminster)

### Get distance and travel time between each pair of geographic points

> Represents the distance and time of the shortest or fastest paths between all pairs of fromPoints and toPoints. The number of fromPoints times the number of toPoints should not exceed 100 or the request will time out.

*Tags:* `distance`

#### Input Parameters
* `outputFormat` - _required_ - Format of representation
    Possible values: json, html.
* `fromPoints` - _required_ - A comma-separated list of origin points.  See <a href=https://github.com/bcgov/api-specs/blob/master/router/glossary.md#fromPoints target='_blank'>fromPoints</a>
* `toPoints` - _required_ - A comma-separated list of destination points. See <a href=https://github.com/bcgov/api-specs/blob/master/router/glossary.md#toPoints target='_blank'>toPoints</a>
* `outputSRS` - _optional_ - The EPSG code of the spatial reference system (SRS) to use for output geometries. See <a href=https://github.com/bcgov/api-specs/blob/master/router/glossary.md#outputSRS target="_blank">outputSRS</a>
    Possible values: 4326, 4269, 3005, 26907, 26908, 26909, 26910, 26911.
* `criteria` - _optional_ - Routing criteria to optimize (e.g., shortest, fastest). Default is shortest.
    Possible values: shortest, fastest.
* `distanceUnit` - _optional_ - distance unit of measure (e.g., km, mi). Default is km.
    Possible values: km, mi.
* `routeDescription` - _optional_ - Route description (e.g., Shortest route from 1002 Johnson St, Victoria to 1105 Royal Ave,New Westminster)
* `maxPairs` - _optional_ - The maximum number of pairs to return for each toPoint.  Pairs are ordered by distance/time from fromPoint. For example, given 1 fromPoint, and 10 toPoints, and maxPairs=1 , return the nearest toPoint to the fromPoint. Given 3 fromPoints and 10 toPoints, maxPairs=3 means return the 3 nearest toPoints to each fromPoint.

### Get distance and travel time between each pair of geographic points

> Represents the distance and time of the shortest or fastest paths between all pairs of fromPoints and toPoints. The number of fromPoints times the number of toPoints should not exceed 100 or the request will time out.

*Tags:* `distance`

#### Input Parameters
* `outputFormat` - _required_ - Format of representation
    Possible values: json, html.
* `fromPoints` - _required_ - A comma-separated list of origin points.  See <a href=https://github.com/bcgov/api-specs/blob/master/router/glossary.md#fromPoints target='_blank'>fromPoints</a>
* `toPoints` - _required_ - A comma-separated list of destination points. See <a href=https://github.com/bcgov/api-specs/blob/master/router/glossary.md#toPoints target='_blank'>toPoints</a>
* `outputSRS` - _optional_ - The EPSG code of the spatial reference system (SRS) to use for output geometries. See <a href=https://github.com/bcgov/api-specs/blob/master/router/glossary.md#outputSRS target="_blank">outputSRS</a>
    Possible values: 4326, 4269, 3005, 26907, 26908, 26909, 26910, 26911.
* `criteria` - _optional_ - Routing criteria to optimize (e.g., shortest, fastest). Default is shortest.
    Possible values: shortest, fastest.
* `distanceUnit` - _optional_ - distance unit of measure (e.g., km, mi). Default is km.
    Possible values: km, mi.
* `routeDescription` - _optional_ - Route description (e.g., Shortest route from 1002 Johnson St, Victoria to 1105 Royal Ave,New Westminster)
* `maxPairs` - _optional_ - The maximum number of pairs to return for each toPoint.  Pairs are ordered by distance/time from fromPoint. For example, given 1 fromPoint, and 10 toPoints, and maxPairs=1 , return the nearest toPoint to the fromPoint. Given 3 fromPoints and 10 toPoints, maxPairs=3 means return the 3 nearest toPoints to each fromPoint.

### Get the directions, optimal path, distance and travel time between a start point and a series of end points which are reordered to minimize total distance or time.

> Represents the turn-by-turn directions, geometry, distance, and time of the shortest path or fastest path between a start point and a series of end points which are reordered to minimize distance/time

*Tags:* `directions`

#### Input Parameters
* `outputFormat` - _required_ - Format of representation
    Possible values: json, kml, html.
* `points` - _required_ - A list of any number of route points in start to end order. See <a href=https://github.com/bcgov/api-specs/blob/master/router/glossary.md#points target='_blank'>points</a>
* `outputSRS` - _optional_ - The EPSG code of the spatial reference system (SRS) to use for output geometries. See <a href=https://github.com/bcgov/api-specs/blob/master/router/glossary.md#outputSRS target="_blank">outputSRS</a>
    Possible values: 4326, 4269, 3005, 26907, 26908, 26909, 26910, 26911.
* `criteria` - _optional_ - Routing criteria to optimize (e.g., shortest, fastest). Default is shortest.
    Possible values: shortest, fastest.
* `distanceUnit` - _optional_ - distance unit of measure (e.g., km, mi). Default is km.
    Possible values: km, mi.
* `roundTrip` - _optional_ - If true, route ends at start point. Default is false.
* `routeDescription` - _optional_ - Route description (e.g., Shortest route from 1002 Johnson St, Victoria to 1105 Royal Ave,New Westminster)

### Get the directions, optimal path, distance and travel time between a start point and one or more end points which are reordered to minimize total distance or time.

> Represents the turn-by-turn directions, geometry, distance, and time of the shortest path or fastest path between a start point and one or more end points which are reordered to minimize distance or time.

*Tags:* `directions`

#### Input Parameters
* `outputFormat` - _required_ - Format of representation
    Possible values: json, kml, html.
* `points` - _required_ - A list of any number of route points in start to end order. See <a href=https://github.com/bcgov/api-specs/blob/master/router/glossary.md#points target='_blank'>points</a>
* `outputSRS` - _optional_ - The EPSG code of the spatial reference system (SRS) to use for output geometries. See <a href=https://github.com/bcgov/api-specs/blob/master/router/glossary.md#outputSRS target="_blank">outputSRS</a>
    Possible values: 4326, 4269, 3005, 26907, 26908, 26909, 26910, 26911.
* `criteria` - _optional_ - Routing criteria to optimize (e.g., shortest, fastest). Default is shortest.
    Possible values: shortest, fastest.
* `distanceUnit` - _optional_ - distance unit of measure (e.g., km, mi). Default is km.
    Possible values: km, mi.
* `roundTrip` - _optional_ - If true, route ends at start point. Default is false.
* `routeDescription` - _optional_ - Route description (e.g., Shortest route from 1002 Johnson St, Victoria to 1105 Royal Ave,New Westminster)

### Get the optimal path, distance and travel time between a start point and a series of end points which are reordered to minimize total distance or time.

> Represents the geometry, distance, and time of the shortest or fastest path between a start point and a series of end points which are reordered to minimize distance or time

*Tags:* `route`

#### Input Parameters
* `outputFormat` - _required_ - Format of representation
    Possible values: json, kml, html.
* `points` - _required_ - A list of any number of route points in start to end order. See <a href=https://github.com/bcgov/api-specs/blob/master/router/glossary.md#points target='_blank'>points</a>
* `outputSRS` - _optional_ - The EPSG code of the spatial reference system (SRS) to use for output geometries. See <a href=https://github.com/bcgov/api-specs/blob/master/router/glossary.md#outputSRS target="_blank">outputSRS</a>
    Possible values: 4326, 4269, 3005, 26907, 26908, 26909, 26910, 26911.
* `criteria` - _optional_ - Routing criteria to optimize (e.g., shortest, fastest). Default is shortest.
    Possible values: shortest, fastest.
* `distanceUnit` - _optional_ - distance unit of measure (e.g., km, mi). Default is km.
    Possible values: km, mi.
* `roundTrip` - _optional_ - If true, route ends at start point. Default is false.
* `routeDescription` - _optional_ - Route description (e.g., Shortest route from 1002 Johnson St, Victoria to 1105 Royal Ave,New Westminster)

### Get the path, distance and travel time between a start point and a series of end points which are reordered to minimize total distance or time.

> Represents the geometry, distance, and time of the shortest or fastest path between a start point and a series of end points which are reordered to minimize total distance or time.

*Tags:* `route`

#### Input Parameters
* `outputFormat` - _required_ - Format of representation
    Possible values: json, kml, html.
* `points` - _required_ - A list of any number of route points in start to end order. See <a href=https://github.com/bcgov/api-specs/blob/master/router/glossary.md#points target='_blank'>points</a>
* `outputSRS` - _optional_ - The EPSG code of the spatial reference system (SRS) to use for output geometries. See <a href=https://github.com/bcgov/api-specs/blob/master/router/glossary.md#outputSRS target="_blank">outputSRS</a>
    Possible values: 4326, 4269, 3005, 26907, 26908, 26909, 26910, 26911.
* `criteria` - _optional_ - Routing criteria to optimize (e.g., shortest, fastest). Default is shortest.
    Possible values: shortest, fastest.
* `distanceUnit` - _optional_ - distance unit of measure (e.g., km, mi). Default is km.
    Possible values: km, mi.
* `roundTrip` - _optional_ - If true, route ends at start point. Default is false.
* `routeDescription` - _optional_ - Route description (e.g., Shortest route from 1002 Johnson St, Victoria to 1105 Royal Ave,New Westminster)

### Get the path, distance and travel time between a series of geographic points

> Represents the geometry, distance, and time of the shortest or fastest path between given start and end points.

*Tags:* `route`

#### Input Parameters
* `outputFormat` - _required_ - Format of representation
    Possible values: json, kml, html.
* `points` - _required_ - A list of any number of route points in start to end order. See <a href=https://github.com/bcgov/api-specs/blob/master/router/glossary.md#points target='_blank'>points</a>
* `outputSRS` - _optional_ - The EPSG code of the spatial reference system (SRS) to use for output geometries. See <a href=https://github.com/bcgov/api-specs/blob/master/router/glossary.md#outputSRS target="_blank">outputSRS</a>
    Possible values: 4326, 4269, 3005, 26907, 26908, 26909, 26910, 26911.
* `criteria` - _optional_ - Routing criteria to optimize (e.g., shortest, fastest). Default is shortest.
    Possible values: shortest, fastest.
* `distanceUnit` - _optional_ - distance unit of measure (e.g., km, mi). Default is km.
    Possible values: km, mi.
* `roundTrip` - _optional_ - If true, route ends at start point. Default is false.
* `routeDescription` - _optional_ - Route description (e.g., Shortest route from 1002 Johnson St, Victoria to 1105 Royal Ave,New Westminster)

### Get the path, distance and travel time between a series of geographic points

> Represents the geometry, distance, and time of the shortest or fastest path between given start and end points.

*Tags:* `route`

#### Input Parameters
* `outputFormat` - _required_ - Format of representation
    Possible values: json, kml, html.
* `points` - _required_ - A list of any number of route points in start to end order. See <a href=https://github.com/bcgov/api-specs/blob/master/router/glossary.md#points target='_blank'>points</a>
* `outputSRS` - _optional_ - The EPSG code of the spatial reference system (SRS) to use for output geometries. See <a href=https://github.com/bcgov/api-specs/blob/master/router/glossary.md#outputSRS target="_blank">outputSRS</a>
    Possible values: 4326, 4269, 3005, 26907, 26908, 26909, 26910, 26911.
* `criteria` - _optional_ - Routing criteria to optimize (e.g., shortest, fastest). Default is shortest.
    Possible values: shortest, fastest.
* `distanceUnit` - _optional_ - distance unit of measure (e.g., km, mi). Default is km.
    Possible values: km, mi.
* `roundTrip` - _optional_ - If true, route ends at start point. Default is false.
* `routeDescription` - _optional_ - Route description (e.g., Shortest route from 1002 Johnson St, Victoria to 1105 Royal Ave,New Westminster)

## License

**flow**ground :- Telekom iPaaS / gov-bc-ca-router-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
