# 5micron-backend-challenge

We are working on a project functioning as an IOT platform. Daily backend tasks involves maintaining web servers and communication with IOT sensors (guarantee performance and security). This is the a challenge that candidate should pass to show his/her capability to work comfortably in our environment. The challenge contains:
1. Create a NodeJS web server listening at port 3000.
2. Create a Postgresql database to store incoming sensor data.
3. Create a REST API endpoint [api/sensors](http://localhost:3000/api/sensors) at the web server to handle incoming sensor data in JSON format:
    1. Allow only POST HTTP request in JSON data format that has properties following this example:  ```{ "serial": "TEM-000001", "swVersion": "01-01", "temperature": "28", "date": "2023-04-17T12:22:43", "gps": "52.52,12.04"}```.
    3. Parse JSON data and store it into database.

Note and hints:
- We recommend using ExpressJS to write the web server because of its simplicity.
- Database should have a table with columns matching the properties "serial", "swVersion", "temperature", "date", "gps".
- Use curl or Postman to send POST HTTP request that body contains JSON data similar to the example ```{ "serial": "TEM-000001", "swVersion": "01-01", "temperature": "28", "date": "2023-04-17T12:22:43", "gps": "52.52,12.04"}``` to test server's behavior and also to store to the database.

We expect to receive:
  - source code (can be github link or zip file).
  - Postgresql database in plain-text format that contains a table with at least 3 rows of data similar to the above example  (use pg_dump command utility to export).

We assume that in order to complete the challenge the candidate has basic understanding of backend development as theory concepts and practical deployments. If there are any concepts that are new to the candidate, we expect that he/she is able to learn by doing research. That's the trait of the candidate we are looking for as we have to constantly improve our systems guaranteeing performance and security.

## Have fun coding! :)
