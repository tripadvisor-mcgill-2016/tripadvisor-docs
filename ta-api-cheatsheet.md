# TripAdvisor Partner JSON API

### Sample URL
http://api.tripadvisor.com/api/partner/2.0/location/60745/hotels?key=<your_key>

### URL Structure
   - **Host, Servlet, Namespace, Version**: `http://api.tripadvisor.com/api/partner/2.0/`
   - **Endpoint and Connection**: `location/60745/hotels`
   - **Your Key**: `?key=<your_key>`
   - **Optional URL Parameters**: `&lang=de`

### Response Format Sample Snippet (for a list call)

    {
         "data": [
             {
                 "location_id": "77638",
                 "name": "The Inn at Longwood Medical",
             },
             {
                 "location_id": "3225572",
                 "name": "enVision Hotel Boston",
             },
         ],
    }

### Reference Documentation
API reference: `http://api.tripadvisor.com/api/partner/2.0/doc?key=<your_key>`

Detailed Documentation: `https://developer-tripadvisor.com/partner/json-api/` <br/>
(Contact the hackathon organizers for credentials)

### TripAdvisor Location ID Examples
Property:
   - Accommodation: 114134: The Lenox Hotel in Boston
   - Attraction: 105250: Fenway Park
   - Eatery: 322981: Pizzeria Regina

Geo:
   - 1 : The World
   - 17 : North America
   - 191 : USA
   - 28942 : Massachusetts
   - 60745 : Boston

### Sample Calls
#### /location
Get data for location 89575
`http://api.tripadvisor.com/api/partner/2.0/location/89575?key=<your_key>`

Get reviews for location 89575
`http://api.tripadvisor.com/api/partner/2.0/location/89575/reviews?key=<your_key>`

Get the best Hotels in location 60745 (Boston)
`http://api.tripadvisor.com/api/partner/2.0/location/60745/hotels?key=<your_key>`

Get photos for location 60745
`http://api.tripadvisor.com/api/partner/2.0/location/60745/photos?key=<your_key>`

#### /map
Get locations near a lat long point
`http://api.tripadvisor.com/api/partner/2.0/map/42.33141,-71.099396?key=<your_key>`

Get locations near a lat long point that are attractions
`http://api.tripadvisor.com/api/partner/2.0/map/42.33141,-71.099396/attractions?key=<your_key>`

Get attractions near a lat long point that contain ‘art’ in the name
`http://api.tripadvisor.com/api/partner/2.0/map/42.33141,-71.099396/attractions?key=<your_key>&q=arts`

Get geographic locations (cities) near a lat long point
`http://api.tripadvisor.com/api/partner/2.0/map/42.33141,-71.099396/geos?key=<your_key>`

#### /search
Search for locations with “freedom trail run”
`http://api.tripadvisor.com/api/partner/2.0/search/freedom%20trail%20run?key=<your_key>`

Search for locations with “bellagio” that are hotels
`http://api.tripadvisor.com/api/partner/2.0/search/bellagio?key=<your_key>&category=hotels`

#### Neat Stuff / Ideas
Best hotels in a country
`http://api.tripadvisor.com/api/partner/2.0/location/191/hotels?key=<your_key>`

Walk part of the location hierarchy:
`http://api.tripadvisor.com/api/partner/2.0/location/1/geos?key=<your_key>`

Get locations of some type near lat / long
`http://api.tripadvisor.com/api/partner/2.0/map/42.33141,-71.099396/attractions?key=<your_key>`

### Acknowledgements
Thanks to Barlow Adamson (TripAdvisor)
