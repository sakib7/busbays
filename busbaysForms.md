# BusBays Forms Development To-do List

![BusBays Schema](https://user-images.githubusercontent.com/20136237/33782855-830fae2e-dc84-11e7-902d-af5fd7adb073.JPG)
[**click here for busbays.sql**](https://gist.github.com/sakib7/fc44d277ecdbbf3fc22c7bbfa3364a7c)

>Please pay attention to the **foreign key** dependencies among different entities and maintain the required chronological order while developing the modules. Also pull the foreign keys in a **drop down** menu.

## Perform a simple CRUD on the following:
1. District
2. Driver
3. Supervisor
4. Bus
5. Restaurant
6. Booking_Config
7. Passenger
8. Staff
9. Bus_Stop

## Managing Routes

I believe, updating a route means creating a new route. We, therefore, won't do any update operation on routes.

 **Create a new route**

 Since routes can have any number of bus stops, we'll have to create a dynamic form for adding new route. New route form will have the following:
- There will be an *add a bus_stop* button which will dynamically create a drop down for **bus_stop** and two text fields for **distance** and **arriving time**.
- Drop downs for source and destination city, driver, supervisor, bus , restaurant.  

 **Perform read and delete operations on routes**

## Buying tickets

Again no update is required, Just do the delete and insert. Inserting will have two pages : 
### route selection
1. **boarding city**  will update boarding points drop down.
2. **boarding point** will update arrival city and bus stops.
2. **arrival city** will update arrival bus stops.
3. **arrival bus stop** will update boarding time.
4. **Journey date** will be loaded after being verified from booking_config.
5. **Journey Time** :  This selection will lead to an unique route id.
### seat selection
1. Create bus seat model using buttons and select a seat from the ones that haven't been booked yet.
2. Finally add passenger info.
