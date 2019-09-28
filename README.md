# _Carbs: The Bakery_

#### _A Basic "Point of sale" system for a bakery, September 27th, 2019_

#### _By **Jennifer Batara**_

## Description

This application is a C#.Net application run in the console that is able to track transactions for a bakery with certain discount schemes.

The user is able to add a new transaction, see old transactions, and edit old transactions. Currently the transactions are stored locally, and are not saved between run istances of the console application.

## Specifications: Pricing

|Spec | Input | Output|
|:---:|:------|:------|
|Bread is $5 each|Add 2 Bread Items| Total: $10|
|Bread is 3 for $10|Add 3 Bread Items|Total: $10|
|Pastries are $2 per pastry|Add 2 Pastry Items| Total: $4|
|Pastries are 3 for $5|Add 7 pastries| Total: $12|

## Specifications: User Interface
For all of these situations, the sample Transaction list is only 1 transaction long.
|Spec | Input | Output|
|:---:|:------|:------|
|If POSMainMenu command input doesn't exist|"wegwe"| wegwe is not a valid ID input. Going back to the main. Going back to the main menu.  |
|POSNewTransaction creates a new Transaction when fed the code 0| POSNewTransaction(0) | New Transaction Created|
|POSNewTransaction does not create a new Transaction when fed the code 1, instead it will open the latest transaction| POSNewTransaction(1)|Open Transaction Count|
|POSEditTransaction requires an ID selection that exists| POSEditTransaction(1)|Print Transaction with ID 1|
|POSEditTransaction requires an ID selection that exists| POSEditTransaction(100)|An ID of 100 is an invalid Input. Going back to the Main Menu.|



## Setup/Installation Requirements

-   Internet Connection
-   Internet browser
-   Bash Terminal
-   .NET Core

If you do not have the .NET Core installed on your computer, please install it by following the directions for your operating system [here](https://dotnet.microsoft.com/download). The .NET Core version used for this project is 2.1

To view locally please copy the link to [this repo](https://github.com/jbatara/CarbsTheBakery) and type the following command into your Bash terminal:

$git clone repo_url

with repo_url being the url that was just copied. To open the console app, navigate to the local directory which the online repository was cloned to using the command

$cd CarbsTheBakery/

Once in the correct repository, and confirming that you have .NET core installed (version 2.1 at minimum), run the app with the command

$dotnet run

and enjoy!

This project is currently not hosted online.

## Known Bugs

_1. Trying to add a new transaction within the main menu returns an invalid ID for POSEditTransaction. WIP_

## Support and contact details

Please feel free to contact the developer by raising a new [issue](https://github.com/jbatara/CarbsTheBakery/issues/new) on the github repo. You can browse the current issues [here](https://github.com/jbatara/CarbsTheBakery/issues).

## Technologies Used

* C#
* .NET Core 2.1

### License

_MIT_

Copyright (c) 2019 **_Jennifer Batara_**