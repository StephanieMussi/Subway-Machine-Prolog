# Subway_Machine_Prolog
The Prolog Subway Sandwich Machine offers users different options of meals and display the menu based on user's choice. The machine is also capable of recording the order and displaying the receipt.  

## Introduction  
The machine offers the following options:  
* __meal__ options
* __bread__ options
* __meat__ options
* __vegetable__ options
* __sauce__ options
* __top-up__ options
* __sides__ options  
  
Moreover, the machine can intelligently display the options selectively person’s previous choices:  
1. If the person chose a _veggie meal_, meat options should not be offered.  
1. If a person chose a _healthy meal_, fatty sauces should not be offered.  
1. If a person chose a _vegan meal_, cheese top-up should not be offered.  
1. If a person chose a _value meal_, no top-up should be offered.  

Based on the requirements above, the working sequence is designed in the following way:  

The full menu is as followed:   
```prolog
meal([standard, value, veggie, vegan, healthy]).
bread([italian_wheat, hearty_italian, honey_oat, parmesan_oregano, multigrain, flatbread]).
meat([chicken_breast, ham, bacon, meat_ball, roast_beef, steak, tuna]).
veggies([cucumbers, bell_peppers, lettuce, onions, tomatoes, olives, corn, pickles]).
fatty_sauce([chipotle_southwest, ranch, bbq, mayonnaise, mustard]).
non_fatty_sauce([chilli_sauce, tomato_sauce]).
cheese_topup([processed_cheddar, monterey_cheddar]).
non_cheese_topup([egg_mayo, guacamole]).
sides([chips, cookies, hash_browns, yogurt, drinks]).
```

