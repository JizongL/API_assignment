
### YouTube API documentation
List 1 required parameter and 2 optional parameters for this endpoint. For each parameter listed, state the data type and give an example of the allowed values.

*required* 
Param:`part`
data type:`string`
allowed value:`contentDetails: 2`

*Optional*
`maxResults`
data type: `unsigned integer`
allowed value: 1 to 50, inclusive

`maxHeight`
data type: `unsigned integer`
allowed value: 72 to 8192, inclusive

### Google Maps Geocoding API documentation
Construct the full URL for requesting the geographic coordinates of The Statue of Liberty in JSON format. Do the same for your own address.

`https://maps.googleapis.com/maps/api/geocode/json?address=Statue+of+Liberty+National+Monument,+New+York,NY&key=YOUR_API_KEY`

`https://maps.googleapis.com/maps/api/geocode/json?address=901+vandon+loop,+Berlin+NJ&key=YOUR_API_KEY`



### Meetup API


Visit the meetup.com API docs found here: https://www.meetup.com/meetup_api/. Answer the following questions:


* Does this API require authentication?

Most requests must be authenticated. Unless otherwise specified

* Does this API support CORS?

Yes, it does. 

* Find the events search endpoint documentation. 
Describe in detail the response format of the 
events search endpoint.

A successful request will return a 201 response with a body containing the new event information.

* What are the limitations placed on the number of 
requests that can be made?

By default it limits users to 200 requests per hour, and 200 max results for each request. If exceeded this number, the platform will return a 400 error response with limit as the code element in the error response body.


* List the errors that you can expect when making 
calls to this API.

400 Bad request when there was a problem with the request
401 Unauthorized when you don't provide a valid key
429 Too Many Requests when you've gone over your request rate limit
500 Internal Server Error if we messed up -- please let us know!