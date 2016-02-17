## API keys for the MCHacks hackathon (these will be revoked following the weekend)

### API Key Rules
* Please do not start burning through API data before the hackathon starts!

* Please be careful not to accidentally call the api hundreds of times from 
a loop. *Once the daily call limit on a key is reached, we cannot reset it.*

### Partner API docs

TA partner API docs: https://developer-tripadvisor.com/partner/json-api/documentation

Main auto-gen docs: http://api.tripadvisor.com/api/partner/2.0/doc?key=KEY

### Call Samples
```
curl "https://api.tripadvisor.com/api/partner/2.0/search/coffee?key=KEY&geo=155004&category=restaurants"
```

### Useful TripAdvisor region IDs (geos)
* Ottawa 155004
* Toronto 155019
* Montreal 155032
* Ontario 154979
* Canada 153339
