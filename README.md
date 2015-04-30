Mobile Applications Development Project

Jason Thorne
g00317349

Calorie counting app


Constructed using:

Microsoft Azure, Ubuntu server, Cordova, Ionic, VI editor, Putty and GitHub. Written in: Javascript, HTML and CSS.

Aims of app:

This is an app designed to allow the user to keep track of their calorie intake by selecting from a number of foods from a list of their given food group.

How this is implimented: 

The app consists of five different states using ion-nav-view. Four states representing a different food group, and one state representing a homepage of the app which the user is initially directed to when opening the app. 


State 1. Calorie Counter. 

This is the initial home page of the app and as such contains the title of the app "Calorie Counter". This is shown at the top of the app using the ion-nav-bar, as is every other state's title on it's specific state. This state contains links to each food group state. Given in button form. 

States 2-5.

Each of these consists of the 4 most common food types of each of their groups. The groups are as follows: 

*Fruits
*Grains
*Vegetables
*Meats

Each of these groups displays the four most common food types in the form of a list of checkboxes. These allow the user to select any food which they have eaten for recording.

There is also an innerHTML property called "calTotal" shown as the total number of calories. This is initially shown to the user as 0, before they made any selections. 

When an item is selected, a javascript function called "addCals" is invoked, and a value equal to the amount of calories, the item represents is passsed in as an aguement.

This value is then then parsed into an int and stored in the variable "calNum". The variable "calSum" representing the total calorie sum is then declared. This is asigned a value equal to that of the inner HTML property of "calTotal", plus the value of calNum, declared above. The property of "calTotal" is then asigned the value of calSum, giving it the total ammount of calories selected by the user.  
 
There is also a button on these states allowing the user the option to clear their calorie total, if they wish. This is done by invoking the function "reset", once the button is selected. This function asigns a value of 0 to "calTotal".

Finally, there is a button at the bottom of each state allowing the user to travel back to the home page, inorder to pick food items from other food groups.

The different food types from each group, and their asociated calorie totals are as follows: 

State 2 - Fruits. One per serving.

*Apple - 72
*Orange - 62
*Pear - 96
*Banana - 89

State 3 - Grains. Per average 50g serving.

*Oats - 194
*Pasta - 186
*Rice - 56
*bread - 144

State 4 - Vegetables. Per average 25g serving.

*Lettuce - 4
*Potatoes - 19
*Carrots - 10
*Peas - 25

State 5 - Meats. Per average 100g serving.

*Beef - 313
*Lamb - 246
*Pork - 541
*Chicken - 219 
