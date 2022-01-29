# T3A2 Part A - Documentation

This repository contains documentation for a web application project which is to be completed as a group as part of a course in web development  The brief for this project was to create a web application for a real business client, which solved a challenge their facing the business.  The 'real' requirement has been dropped, however, due to the difficulties presented by the COVID-19 pandemic.  Our project will create a restaurant menu and ordering web application for an imaginary restaurant.

This repository contains documentation only; the source code for the [back end is here](https://github.com/korayleigh/t3a2-b-backend), and the [front end is here](https://github.com/korayleigh/t3a2-b-frontend)
## Purpose

Our web application is designed to replace manual pen and paper processes for browsing the restaurant menu, and placing an order.  It was conceived for use by customers when seated in the restaurant, however it can also provide for take-away orders.

Customers will be able to browse the restaurant menu on their own smart device while seated at their table, view the details of dishes, add them to their cart and finalise the order.  This allows the restaurant to run more efficiently, with lower reliance on human wait staff, and less chance of human errors such as communication, or mislaid orders.

The web application will also replace other processes in the restaurant relating to orders, such as as notifying the kitchen of pending dishes, and the customer service and other functions performed by the manager.  The web application will provide interfaces for different types of users to enable them to see the order information most relevant to them, and interact with it according to their role.

## Functionality / Features

The below features are grouped according to the anticipated roles of users of the web application, and constitute the agreed minimum viable product (MVP) of the web application.

### Customers

Customers will be able to view general information about the restaurant from the landing page including the a description of the restaurant, the physical address, contact information, and view general images of the restaurant, such as street position, dining rooms,  and the team.

The main feature for customers is the restaurant menu.  Customers may browse the full menu, or search and filter it for a more specific view.  Customers with specific dietary requirements will be able to filter the menu to only display dishes compatible with their needs. 

To best communicate each dish to the customer images will accompany each menu item, and each item can be clicked for more detailed description and specific details, such as ingredients, spiciness, and allergy information etc.

Once a suitable dish is found, customers can then add it to their order, building up a full order for their group.  Customers may be either dining in the restaurant, or making an order for pick-up, and the order process will gather this information. Once finalised, the customer will view a summary of the items on their order, and be asked to confirm their order, after which it begins processing.

At this stage, payment for the order will still be handled manually, as per current process.  For dine-in orders this is at the end of the meal, and for take-away orders at time of pick-up.  However, in future versions of the application online payment is planned, as part of the finalisation of the order.

After finalising the order, the customer can view an order summary and can monitor the status of the order as it is being prepared.

### Kitchen

From the landing page, kitchen users will be able follow a link to a login page, so they may access the interface for the kitchen role.

From this interface, they will be able to see pending dishes from finalised orders that are waiting to be cooked by the kitchen.  

As those dishes are cooked the chef can update the status of the dish, which can be viewed by the customer or others.

### Wait staff

Wait staff are the initial customer service contact for customers in the restaurant.  After logging in, they will be able to view details of all orders, and can escalate any issues to a manager for remediation.

### Manager

The manager of a restaurant is usually tasked with ensuring a smooth operation and dealing with any customer service issues that may arise.  To enable this, the manager is given greater privileges to modify orders and their contents.

After logging in, the manager can view all orders and change any detail of an order, even if it is already cooked or delivered to the customers table.  They could change the price charged for a dish, or delete it entirely from the order. This enables them to provide appropriate remediation for any customer service issues such as quality or errors on behalf of the restaurant.

The manager is also able to make changes to the menu, such as adding, removing or editing menu items.  They may also hide an item from customer view if it is no longer available. 

Managers will also have the ability to view the same interface as wait staff and kitchen users, enabling to monitor these aspects of the restaurant operation.

### App Administrator

In the day-to-day operation of the restaurant, the different roles list above have different privileges and responsibilities, according to the rules of the business.

The application administrator is a special role that has the ability to create new users, and view, edit or delete existing users.  The administrator may customise which components of functionality and the user interface are available to which roles, and can assign role to users, which enables them to perform their associated business functions as detailed above.

### Future Features

While not included in the MVP, the following are some additional features that may be added in future versions of the application.

- The ability for customers make bookings for tables at the restaurant.
- A payment gateway at the end of the order process, removing the need for manual payment
- User accounts for customers, so that regular customers can save user preferences, interact with customer functions faster, and benefit from loyalty promotions.
- Enable customers to provide ratings and comments for items on the menu.
- Email communications, for promotions, booking confirmations etc.
- Live messaging, for customer service and other purposes, for customers in the restaurant or for queries relating to take-away orders or bookings.
- Promotions, targeted discounts for loyal customers, and integration of promotion codes etc. into the order process.
- Business monitoring and decision-making tools, including sales summaries over various periods, and statistics such as the relative popularity of dishes.

## Target Audience

The target audience for this web application is both customers and employees of the restaurant.

Customers may be prospective, in that they are researching a place to dine, and may use the landing page and the menu to help them research and decide whether to choose our restaurant.

Actual customers may include both those that are dining in the restaurant, or those who live locally and may choose to come to the restaurant to pick-up a take-away order.  In either case dine-in and take-away customers live locally, as they must at some point be physically present at the restaurant location.

The employees of the restaurant include various users assigned different roles in the running of the business.  They include wait staff, kitchen staff, and managers, however in the current pen and paper process, the lines that delineate these roles can be somewhat fuzzy.  For example a kitchen staff member could also perform waiting duties, and a manager could perform any function.


## Tech Stack

The following technology is planned for use in the development, deployment and maintenance of the web application.

### Front-end

Supported browsers:
  ---
  ||Google Chrome|Mozilla Firefox|Apple Safari|
  |---|---|---|---|
  |Mobile: iOS|v1.0|v2.0|v3.0|
  |Mobile: Android||||
  |Desktop: macOS||||
  |Desktop: Windows||||


JavaScript / ECMAScript version?
React version:
Key React dependencies: react-router-dom, styled-components, axios, 

### Back-end

Hosting: Heroku
Rails version: 
Ruby version?
Key dependencies: devise, devise-jwt, aws-sdk-s3, cors (stripe?)

### Database

Hosting:
PostgreSQL version:

### Development tools

VS Code, git 

## Dataflow Diagram

### Menu, Orders and Users

Note: Payments feature is not included in MVP and is shown here for illustrative purposes only. Online payment is planned for a future version

![Dataflow Diagram - Menu, Orders, Users](link)

## Application Architecture Diagram

![Application Architecture Diagram](link)

## User Stories

### Menu

- As a customer, I want to browse available dishes, so I can decide what to order.
- As a customer, I want to search the menu for a particular dish, so I can find it quickly without scrolling for ages.
- As a customer, I want to filter the menu to dishes of a particular category/style/ingredient/hotness/food allergy, to customise the list to my needs.
- As a manager, I want to manage the list of available dishes, so I can ensure customers are well informed.

### Orders

- As a customer, I want to build an order so I can purchase multiple dishes at once
- As a customer, I want to see the status of my order, so can know it's progress
- As a waiter, I want to see all current orders, so I may assist customers with any queries.
- As a chef, I want to see the pending orders/dishes, so I can prioritise and cook them.
- As a manager, I want to see pending orders/dishes, so I can monitor the kitchen's progress and restaurant operations.
- As a manager, I want to edit orders, so that I can make changes for customer service or other reasons.

### Users

- As the owner and administrator of the website, I want to be able to restrict access to staff-only features (such as the orders dashboard), so that general users of the site will not be able to access these functions.

## Wireframes

### Mobile
### Tablet
### Desktop

## Trello screenshots

