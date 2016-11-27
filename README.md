#I hate breakfast
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
**carbs/$** | 17.1 | 12.5
**protien/$** | 6.5 | 8.2

So far, it seems like lunch has more protien and mass(g) per dollar, while giving you less calories and carbs (bread and butter, literally). More to follow

###Methodology
- I didnt allow duplicate items in multiple categories
- I tried to standardize items between lunch and breakfast, eg. I included only medium french fries instead of sm/md/lg because there is no hash brown size to match it to.
- I only included lunch and breakfast items, no deserts or mccafe stuff

###Possible Errors:
- I haven't checked if there are an equal number of 'value' items on both the lunch and breakfast sections

###Sources:
I got pricing from [Fast Food Menu Prices](http://www.fastfoodmenuprices.com/mcdonalds-prices/), which seems accurate based on what I've seen at my local store.
I got nutrition info from [pffy's awesome repo](https://github.com/pffy/data-mcdonalds-nutritionfacts).

