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
1. If a person chose value meal, no top-up should be offered.  

Based on the requirements above, the working sequence is designed in the following way:  

