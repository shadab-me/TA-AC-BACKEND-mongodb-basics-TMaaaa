writeCode

Write command to

- List collections from a database.
show dbs
- create a new collection in your country database which you created recently.
use country 
db.createCollection('India')
Write code to:-

- crate a database named `weather`
use weather
- create a capped collection named `temperature` with maximum of 3 documents and try inserting more than 3 to see the result.
db.createCollection('temperature');
db.temperature.insert({city: 'Dharamshala', temp: 25});
db.temperature.insert({city: 'Mumbai', temp: 35});
db.temperature.insert({city: 'Jashpur', temp: 22});
db.temperature.insert({city: 'Mumbai', temp: 22});



- create a simple collection named `humidity`
db.createCollection('humidity');
- check whether `temperature` collection is capped or not ?
show collections
- Delete `humidity` collection and then the entire database(weather).
db.humidity.drop();
db.dropDatabase();