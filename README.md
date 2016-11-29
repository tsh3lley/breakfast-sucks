#I Hate Breakfast
I've hated breakfast for a long time now. I can't count how many times I've tried to get food, and stores were either closed or only serving breakfast. While I'd like to have Chipotle at 8AM, I understand their need to run a business. There probably aren't enough people like me who would show up at 8AM to justify opening the store, or they would do it.

The thing that I will never understand, however, is why so many people like the menu items that fast food chains serve for breakfast. I will eat mcnuggets or a hamburger at any time of day, so why am I confined to buttery, bread-heavy bs until 10:30AM? Maybe people don't like breakfast at all... maybe the evil congolmerates have tricked us into thinking that only a madman would eat a burger in the morning... I wanted to find out.

###Hypothesis
Fast food companies are owned and managed by lizard people who trick us into liking breakfast. Breakfast items, on the whole, give us less 'bang for our buck': they contain more crap like bread and less good stuff like meat and veggies per dollar spent. 

###Results
All I really did was combine pricing and nutrition info (sources below), and cleaned the data up a bit. Check out the data at [mcdonalds.csv](./mcdonalds.csv). This is a work in progress, but here are the results so far:

  | Breakfast | Lunch
--- | --- | ---
**g/$** | 61.6 | 64.7
**cal/$** | 183.6 | 148.6
**sfat/$** | 4.0 | 2.1
**tfat/$** | .05 | .11
**chol/$** | 53.5 | 23.5
**salt/$** | 393.4 | 310.7
**carbs/$** | 17.1 | 12.5
**protein/$** | 6.5 | 8.2

So far, it seems like lunch has more protein, trans fat, and mass(g) per dollar, while giving you less calories, saturated fat, cholesterol, salt, and carbs (stuff that kills you).

To get a qualitiative sense of what these stats mean, lets look at the best and worst items for each of the nutritional features. Note that in some cases, I'm using best/worse pretty loosely. More calories per dollar is not necessarily a bad thing, especially if you want to live on the cheap. 

Best | Breakfast | Lunch
--- | --- | ---
**cal/$** | Egg White Delight | Grilled Bacon Ranch Salad
**sfat/$** | Oatmeal | Artisan Grilled Chicken
**tfat/$** | Multi-Item Tie | Multi-Item Tie
**chol/$** | Hash Browns | Multi-Item Tie
**salt/$** | Oatmeal | Med Fries
**carbs/$** | Sausage McMuffin w/ Egg Whites| Grilled Bacon Ranch Salad
**protein/$** | Sausage McMuffin | All $1 Burgers

Worst | Breakfast | Lunch
--- | --- | ---
**cal/$** | Sausage Biscuit | BBQ Ranch Burger
**sfat/$** | Sausage Biscuit | Double Cheeseburger
**tfat/$** | Steak, Egg, & Cheese | McDouble
**chol/$** | Big Breakfast | McDouble
**salt/$** | Sausage Biscuit | Cheeseburger
**carbs/$** | Cinnamon Melts | BBQ Ranch Burger
**protein/$** | Hash Browns | Med Fries

It's somewhat intuitive that a Grilled Bacon Ranch Salad is better for you than a BBQ Ranch Burger, but these tables also give you a sense of what you're getting with breakfast vs lunch. Moral of the story: don't buy a Sausage Biscuit. More to come...

###Methodology
- I didnt allow duplicate items in multiple categories
- I tried to standardize items between lunch and breakfast, eg. I included only medium french fries instead of sm/md/lg because there is no hash brown size to match it to.
- I only included lunch and breakfast items, no deserts or mccafe stuff

###Possible Errors:
- I haven't checked if there are an equal number of 'value' items on both the lunch and breakfast sections

###Sources:
I got pricing from [Fast Food Menu Prices](http://www.fastfoodmenuprices.com/mcdonalds-prices/), which seems accurate based on what I've seen at my local store.

I got nutrition info from [pffy's awesome repo](https://github.com/pffy/data-mcdonalds-nutritionfacts).

