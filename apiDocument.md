// page 1
# List of City
>> https://zom-api.herokuapp.com/location
>> http://localhost:9700/location

# List of Restaurants
>> https://zom-api.herokuapp.com/restaurants
>> http://localhost:9700/restaurants

# List of Restaurants wrt to City
>> https://zom-api.herokuapp.com/restaurants?state_id=1
>> http://localhost:9700/restaurants?state_id=4

# List of MealType
>> https://zom-api.herokuapp.com/quicksearch
>> http://localhost:9700/mealType

//Page2
# List of restaurants on basis of meal
>> https://zom-api.herokuapp.com/restaurants?mealtype_id=
>> http://localhost:9700/restaurants?meal_id=4

# Filter on basis of cuisine
>> https://zom-api.herokuapp.com/filter/4?cuisine=1
>> http://localhost:9700/filters/3?cuisineId=4

# Filter on basis of cost
>> https://zom-api.herokuapp.com/filter/1?hcost=1000&lcost=500
>> http://localhost:9700/filters/1?lcost=300&hcost=900

# Sort (low to High)
http://localhost:9700/filters/1?lcost=300&hcost=900&sort=-1
http://localhost:9700/filters/1?cuisineId=4&sort=-1

//page3
# Details of restaurants
>> http://zom-api.herokuapp.com/details/1
>> http://localhost:9700/details/618776b162a1816f885956bf

Menu on the basis of restaurants
>> http://zom-api.herokuapp.com/menu?restId=8
>>  http://localhost:9700/menu?restId=8

//page4 
> Menu details of item selected
(POST)> localhost:9700/menuItem
(body)> [1,4,6]

> Place Order
(post) > localhost:9700/placeOrder
(body) > 
{
	"name":"parth",
	"email":"parthsheth278@gmail.com",
	"address":"Hno 23,Sector 1",
	"phone":7575073278,
	"cost":399,
	"menuItem":[34,26,17],
	"status":"Pending"
}

//page5
> See all order place
>>> localhost:9700/viewOrder
> Get Order on basis of emailId
>>>>  localhost:9700/viewOrder?email=parthsheth278@gmail.com

//update order
(put) localhost:9700/updateOrder/62514d42f5aec503b2e0f2a9
(body) 
{
	"status":"In Transit",
    "bankName":"Axis Bank"
}

