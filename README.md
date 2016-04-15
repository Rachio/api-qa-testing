# api-qa-testing

##Concepts
The following are a few of the main concepts in our public API:

###Persons
`Person`s are the core of the public Rachio API. A `Person` has information about the user as well as the `Device`'s that belong to the user

###Devices
A `Device` represents the physical sprinkler controller. A `Device` has information about itself and has collections of `Zone`'s, `Schedule`'s, `Webhook`'s. 

###Zones
A `Zone` represents an area in the `Person`'s yard where sprinklers can be run. It contains information about the `Zone`.

###Schedules
A `Schedule` represents a rule that the `Person` has setup in the Rachio app to run a set of `Zone`'s. There are two types of schedules, Schedules Rules and Flex Schedule Rules. Both represent when the given zones will be turned on and off. Flex Schedule Rules cannot be controlled.

###Webhooks
A `Webhook` is a way to get HTTP callbacks when things happen to a `Device`. There are different event types that are returned in the callback and represent what happened to the device.

##Your Task
Given these cocepts, write a small test suite that exercises and verifies that the afformentioned concepts are functioning. We use [Spock](http://spockframework.github.io/spock/docs/1.0/index.html) for our testing, but feel free to use whatever you feel is the best tool for testing RESTful APIs.

You can access all of the documentation for our public API [here](https://rachio.readme.io/). We will provide you with a valid oAuth token to use for your test suite. 

Good luck!

####PS/Extra credit
Use your own HTTP server with webhooks to verify functionality. You may want to use a tool like [ngrok](https://ngrok.m/).
