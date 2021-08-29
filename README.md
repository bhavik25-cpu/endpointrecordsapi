run code
1 npm i
2 npm start

# 
You have been given a Json data file, create a endpoint “/records” which will return json data.

Create a API "api/managed-records.js", that requests data from the “/records” endpoint, transforms the result into the format outlined below

1.	Get data from the /records endpoint using the Fetch API. Process pages of 10 items at a time. Note that the /records endpoint may return more than 10 items per request.

2.	Upon a successful API response, transform the fetched payload into an object containing the following keys:

Ids: An array containing the ids of all items returned from the request.

Open: An array containing all of the items returned from the request that have a disposition value of "open".

ClosedCount: The total number of items returned from the request that have a disposition value of "closed" and contain a primary color.

PreviousPage: The page number for the previous page of results, or null if this is the first page.

NextPage: The page number for the next page of results, or null if this is the last page.
