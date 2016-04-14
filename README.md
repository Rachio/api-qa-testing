# api-qa-testing

Use the following Rachio open [API] (https://rachio.readme.io/) for testing.

A OAuth2 token will be provided.

Use a testing framework like [Spock] (http://spockframework.github.io/spock/docs/1.0/index.html) or a similiar DSL framework for RESTful endpoint testing.

1. Retrieve the information for a person using these endpoints (https://rachio.readme.io/docs/publicpersoninfo) (https://rachio.readme.io/docs/publicpersonid) and assert the user has one device.

2. Start a zone for 5 minutes (https://rachio.readme.io/docs/zonestart), verify the zone is indeed running (https://rachio.readme.io/docs/publicdeviceidcurrent_schedule), stop the zone (https://rachio.readme.io/docs/devicestop_water) and verify the device is not currently watering.
