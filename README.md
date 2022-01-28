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

Once a suitable dish is found, customers can then add it to their order, building up a full order for the table. Once finalised, they will view a summary of the items on their order, and be asked to confirm their order, after which it begins processing.

At this stage, payment for the order will still be handled manually, however in future versions of the application a payment gateway is planned.

While processing the status of the order can be monitored by the customer.

### Kitchen

From the landing page, kitchen users will be able follow a link to a login page, so they may access the interface for the kitchen role.

From this interface, they will be able to see pending dishes from finalised orders that are waiting to be cooked by the kitchen.  

As those dishes are cooked the chef can update the status of the dish, which can be viewed by the customer or others.

### Wait staff

Wait staff are the initial customer service contact for customers in the restaurant.  After logging in, they will be able to view details of all orders, and can escalate an issue to a manager for remediation.

### Manager

The manager of a restaurant is usually tasked with ensuring a smooth operation and dealing with any customer service issues that may arise.  To enable this, the manager is given greater privileges to modify orders and their contents.

After logging in, the manager can view all orders and change any detail of an order, even if it is already cooked or delivered to the customers table.  They could change the price charged for a dish, or delete it entirely from the order. This enables them to provide appropriate remediation for any customer service issues such as quality or errors on behalf of the restaurant.

The manager is also able to make changes to the menu, such as adding, removing or editing menu items.  They may also hide an item from customer view if it is no longer available. 

Managers will also have the ability to view the same interface as wait staff and kitchen users, enabling to monitor these aspects of the restaurant operation.

### App Administrator

The application administrator is a special role that has the ability to create new users, and view, edit or delete existing users.  The administrator can assign role to users, which enables them to perform the associated functions as detailed above.

### Future Features, 
- Bookings
- Payment gateway
- User accounts for customers
- Ratings and comments
- Email notifications
- Live messaging
- Promotions

## Target Audience

- Customers of the restaurant
- Employees/Managers of the restaurant

## Tech Stack

### Front-end

React version:
JavaScript / ECMAScript version?
Key dependencies: react-router-dom, styled-components, axios
Supported browsers:

### Back-end

Rails version:
Ruby version?
Key dependencies: devise, devise-jwt, aws-sdk-s3, cors (stripe)
Hosting: 

### Database

PostgreSQL version:
Hosting:

### Development tools