# lazy_fashions_mule_sfdc

1. Adding the data to Salesforce
POST
path : /lazyadd
    Query parameter: 
      Name: (Name of the customer)
      email: (Email of the customer)
      zip: (zipcode of the user)
      
2. Fetching data from salesforce
path: /lazyflow
GET

3. Updating data

POST
path : /lazyupdate
    Query parameter: 
      Name: (Name of the customer)
      email: (Email of the customer)
      zip: (zipcode of the user)
      
Along with these there are two flows with schedulers that runs after 5 mins and 3 seconds respectively

One flow deletes data every three second from mysql database (Online)
Second flow inserts data from SFDC to MySql db after every 5 minutes.
Time parameter can be adjusted as per user convenience.
      
