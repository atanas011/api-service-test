### API Service Test

To run collection locally, from command line, Node.js should be installed (and added to System variables), as well as newman (npm i -g newman), and newman-reporter-htmlextra (npm i -g newman-reporter-htmlextra).  
Collection can also be run from Postman.

- To run it from command line, clone repo to local dir, and open cmd.exe in it
- To get results, run: newman run RestfulBooker.postman_collection.json -e Test.postman_environment.json
- To get an HTML report, run: newman run RestfulBooker.postman_collection.json -e Test.postman_environment.json -r htmlextra
- Report is created in: newman/


User story:

- Test collections are run against Restful-Booker, a 3rd party API.
- It is a CRUD Web API with authentication feature and loaded with bugs.
- It is pre-loaded with 10 records to work with and resets itself every 10 minutes back to default state.