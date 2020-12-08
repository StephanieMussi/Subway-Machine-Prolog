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
<img src = "https://github.com/StephanieMussi/Subway_Machine_Prolog/blob/main/Figures/FlowChart.png" width = 1000 height = 200>  

The full menu is as followed:   
* meal   
  * standard, value, veggie, vegan, healthy   
* bread   
  * italian_wheat, hearty_italian, honey_oat, parmesan_oregano, multigrain, flatbread   
* meat  
  * chicken_breast, ham, bacon, meat_ball, roast_beef, steak, tuna  
* veggies  
  * cucumbers, bell_peppers, lettuce, onions, tomatoes, olives, corn, pickles  
* sauce  
  * fatty_sauce  
    * chipotle_southwest, ranch, bbq, mayonnaise, mustard  
  * non_fatty_sauce
    * chilli_sauce, tomato_sauce  
* top-up  
  * cheese_topup  
    * processed_cheddar, monterey_cheddar  
  * non_cheese_topup  
    * egg_mayo, guacamole]  
* sides  
  * chips, cookies, hash_browns, yogurt, drinks  


## Demo
After implementing the machine, the following test cases are used to demonstrate the fulfillment of all requirements.   

The first thing before the testing is to declare the list of user's choices as "dynamic". This allows __SWI-Prolog__ to modify the lists on the fly.  
``` prolog
Dynamicall(0):- dynamic(chosen_meal/1),
                dynamic(chosen_bread/1),
                dynamic(chosen_meat/1),
                dynamic(chosen_veggies/1),
                dynamic(chosen_sauce/1),
                dynamic(chosen_topup/1),
                dynamic(chosen_sides/1).
```  


### Test case 1: Standard Meal
### Test case 2: Value Meal
### Test case 3: Veggie Meal
### Test case 4: Vegan Meal
### Test case 5: Healthy Meal



