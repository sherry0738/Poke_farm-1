# Pokemon Farm

## Demo link
[Heroku demo](https://pokemon-farm.herokuapp.com/)

## About
Pokemon farm is a online pokemon fan game.
### Pokemon farm
1. Pokemon farm is where a user can see all the pokemons that they own
2. Pokemon in the farm will grow up as time passes by
3. If a pokemon reaches the level of evolution, player can click the 'evolve' button to let the pokemon evolve

### Pokemon team
1. The team page is to manage player's teams of pokemon.
2. Players can add new teams and add pokemons that they have into a team
3. Player can send out their pokemon team to catch new pokemon

### Pokemon catch
1. This page is for catching new pokemon.
2. Player can select a destination from 9 habitats to start
3. Each habitat will have different pokemons
4. Player can choose one of the pokemon teams to start the trip after choosing a habitat
5. After player send out a team, wait for a while, the team will come back with a possibility of catching a new pokemon from that habitat

### Pokemon shop
1. Player can trade pokemon to the shop or buy poke ball from shop.

## Technologies used
1. HTML, CSS, JAVASCRIPT
2. Bootstrap
3. jQuery
4. AJAX
5. Ruby on Rails
6. PostgreSQL

## The general approach we took
### Pokemon farm
I create a table called my_pokemons to store all the pokemons which had been catched by user. When user catch new pokemon in the Pokemon catch page, he can see his new pokemon in the farm page, because the data is already been stored in my_pokemons table. Pokemons can get exp when they stay in the farm, because there is a calculate of the gap between pokemon update time and current time, exp calculation is base on this gap.

### Pokemon shop
#### for BUY section
- show all items index on the pages from shop database 
- add a input of total value for items to show updating money mount, the things I did for that, which were:
 1. get value and do calculation when user click add or minus button for particular items, and do multipel calculation if user click buttons for more than one items.
 2. then do calculation for total value of user clicks for buy and all money in money bag when user click buy button
 3. get value and do calculation when user click add or minus button for selling items, and do multipel calculation if user click buttons for more than one items.
 4. then do calculation for total value of user clicks for sale and all money in money bag when user click buy button 


#### Epic - In the shop page:

As a logged in user,
when I visit poke farm shop page,
then I should be able to see:
-total mount of user's money
-all items including details of the items for buy in the poke farm shop
-all items including details of the items for sale
-buy pokemons or other items 
-sell pokemons 
-updating of total value for items I want to buy when I click any button in Buy section
-updating of total value for pokemons I want to sell
And I shouldn’t see
-Login
-sign up

As a logged in user,
then I should be able to:
-buy pokemons or other items in BUY section by clicking the add or minus button to choose how many items I want to buy
-purchase for items by clicking BUY button
-sell pokemons or other items in For Sale section by checking or unchecking checkboxes to choose the items whether I want to sell from all My Pokemons list 
-sell for items by clicking SELL button

### Pokedex
when the user put a name of pokemons into input box it returns all the information of
pokemons which are same species using Ajax.
To display its habitat I added method in Species model which returns the habitat of that pokemon.


## User story
The user of this game are pokemon fan who works in the company. They are fan of pokemon, but they are too busy to spend a lot of time to play games. Our game can give them an opportunity to recall childhood without go through a long story line.



## Unsolved problems

1. *Alert:* you can only run db:seed one time after you installed rails server 

2. the poke ball system is not complete
