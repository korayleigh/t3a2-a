# T3A2 Part A - Documentation

This repository contains documentation for a web application project which is to be completed as a group as part of a course in web development  The brief for this project was to create a web application for a real business client, which solved a challenge their facing the business.  The 'real' requirement has been dropped, however, due to the difficulties presented by the COVID-19 pandemic.  Our project will create a restaurant menu and ordering web application for an imaginary restaurant.

This repository contains documentation only; the source code for the [back end is here](https://github.com/korayleigh/t3a2-b-backend), and the [front end is here](https://github.com/korayleigh/t3a2-b-frontend)

---
## Purpose

Our web application is designed to replace manual pen and paper processes for browsing the restaurant menu, and placing an order.  It was conceived for use by customers when seated in the restaurant, however it can also provide for take-away orders.

Customers will be able to browse the restaurant menu on their own smart device while seated at their table, view the details of dishes, add them to their cart and finalise the order.  This allows the restaurant to run more efficiently, with lower reliance on human wait staff, and less chance of human errors such as communication, or mislaid orders.

The web application will also replace other processes in the restaurant relating to orders, such as as notifying the kitchen of pending dishes, and the customer service and other functions performed by the manager.  The web application will provide interfaces for different types of users to enable them to see the order information most relevant to them, and interact with it according to their role.

---
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

---
## Target Audience

The target audience for this web application is both customers and employees of the restaurant.

Customers may be prospective, in that they are researching a place to dine, and may use the landing page and the menu to help them research and decide whether to choose our restaurant.

Actual customers may include both those that are dining in the restaurant, or those who live locally and may choose to come to the restaurant to pick-up a take-away order.  In either case dine-in and take-away customers live locally, as they must at some point be physically present at the restaurant location.

The employees of the restaurant include various users assigned different roles in the running of the business.  They include wait staff, kitchen staff, and managers, however in the current pen and paper process, the lines that delineate these roles can be somewhat fuzzy.  For example a kitchen staff member could also perform waiting duties, and a manager could perform any function.

---
## Tech Stack

The following technology is planned for use in the development, deployment and maintenance of the web application.

### Front-end

#### Supported browsers:
  ||Google Chrome|Mozilla Firefox|Apple Safari|
  |---:|:---:|:---:|:---:|
  |Version|97.0|96.0|15.3|

#### ECMAScript

**version:** ECMAScript 2020 (ES11)
#### React

**version:** 17.0.2

**Key React Dependencies**:
|Dependency|Version|
|---|---|
|react-scripts|v5.0.0|
|react-router|v6.2.1|
|styled-components|v0.1.0|
|axios|0.25.0|

#### Hosting

Netlify

### Back-end

#### Hosting

Heroku

#### Ruby on Rails

**Rails version:** 7.0.1
**Ruby version:** 2.7.4

**Key Rails Dependencies**:
|Dependency|Version|
|---|---|
|devise|4.8.1|
|devise-jwt|0.9.0|
|aws-sdk-s3|1.111.3|
|cors|1.0.1|


### Database

#### Hosting
Heroku

#### Database type and version
PostgreSQL v14.1

### Development tools

- VS Code v1.63
- git v2.30

---
## Dataflow Diagram

### Menu, Orders and Users

Note: Payments feature is not included in MVP and is shown here for illustrative purposes only. Online payment is planned for a future version

![Dataflow Diagram - Menu, Orders, Users](docs/dataflow_diagram/dataflow_diagram_menu_and_orders_and_payment_and_users.drawio.png)
[Click here for full image](https://github.com/korayleigh/t3a2-a/blob/main/docs/dataflow_diagram/dataflow_diagram_menu_and_orders_and_payment_and_users.drawio.png)

---
## Application Architecture Diagram

![Application Architecture Diagram](docs/application_architecture_diagram/application_architecture_diagram.drawio.png)
[Click here for full image](https://github.com/korayleigh/t3a2-a/blob/main/docs/application_architecture_diagram/application_architecture_diagram.drawio.png)

---
## User Stories

The following user stories describe the intended features of the web application.

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

---
## Wireframes

### Mobile
### Tablet
### Desktop

---

## Planning Methodology

For our planning methodology, we have adopted an agile approach, with task management achieved through Kanban, implemented on the Trello platform.

As we are a team of two, we are able to emphasise flexibility as a smaller team is easier to manage. The two of us are in constant communication, and continually review and revise every aspect of the project, both on a macro level (features, design, vision), and also on a micro level (implementation details).

We have daily meetings that at the very least review our progress for the day, any blockers, and what we plan to do next. These meetings cover the status of each ongoing task, and usually include more general planning and discussion elements as well.

Every task that comes to mind that might need doing goes into the ‘Backlog’ column of our Kanban board on Trello. At the Backlog stage, additional details surrounding due dates, team member allocation and complexity are (unless obvious) not included. This stage is simply to ensure that a given task is not neglected down the track. It is important to note that a given task may or may not actually get done - wishlist features for example also go into the Backlog column.

From the Backlog column, we move any tasks that need doing as a priority to the ‘To Do’ column. It is at this stage that supplementary details are added including those mentioned above, and checklists. If a task’s complexity estimate is deemed to be ‘too large’ (this is a flexible definition depending on many factors, but usually not above a 5 or an 8) then this card is broken down into smaller tasks.

Once we are working on a task, it moves to the ‘Doing’ column. Each person only has 1-2 tasks in progress at a time - in line with general Kanban principles - which aims to increase the rate of ‘flow’ (the speed with which tasks get done). Having a set task limit helps because in addition to our individual tasks, we need to review the other team member’s work.

In using this however, we found that on occasion, a task was not able to progress through to completion because of some other prerequisite that needed doing. Because of this, we later added a 'Blocked' column, to hold any tasks that have been started, need further work, and cannot be worked on right now. This had the added benefit of really being able to limit our 'Doing' tasks to 1 per person most of the time.

Items are moved to the ‘Code Review’ column, when they are completed by the assignee, and need to be reviewed and approved by the team member (i.e. when the pull request has been made). If significant reworks are required, another card may be added at this stage with details of the changes. For minor amendments, these are made immediately, and only then do the cards move on to the next phase.

The ‘Test’ column is for code that has been written and reviewed, but needs to have testing implemented.

Once reviewed (and if relevant, tested), cards are moved to the ‘Complete’ column.

### Trello screenshots