# Web-Application-Assignment

Banking Web Application developed for my Web Applications and Services Module, in Jakarta EE.

# Front-End
The front-end is developed using JSF pages and are all connected to CDI backing beans. [Materialize CSS Framework]{https://materializecss.com/} was used for styling the webapp and some custom CSS to achieve the desired look.

# Accounts
Users can sign up with £1000 or the equivalent in the chosen currency. There is one master admin account capable of creating more admin accounts but child admin accounts cannot not create more admin accounts.

Admins can view all users and their balances, all transactions in the system and the master admin can create more admin accounts.

Users can view their transaction history, pending transaction request, make transaction request and view their balance.

# Backend
The backend is based around the DAO and DTO design pattern. Data is sent between the layers using DTOs and are passed to DAOs to persist the new data to the database.
The database and webapp is hosted on a Payara server.

# RESTful currency conversion API
There is a RESTful API used for currency conversion and uses this format baseURL/conversion/{currency1}/{currency2}/{amount_of_currency1}. The values are hardcoded per the requirements set for this work.
