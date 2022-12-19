# GoTickets-Business-System-using-SDLC-concepts


GoTickets - A portal for all your events’ ticketing needs 
With the return of offline events post COVID-19 lockdown, lack of awareness about these events is leading to losses for event business, and even more so, willing customers aren’t able to attend them. To solve this problem, we came up with the idea of creating a platform that lists down all these events on a common platform, where a customer can view events around them and businesses can post relevant & necessary information about their events. We hope to bridge the gap between supply and demand that is created by miscommunication & lack of knowledge.

Welcome to the GoTickets website. The website asks the user to login into their account or create a new account. The website gives an option to the user to login as a customer or business partner or admin. A user can have 2 accounts with different roles, but each account has a unique name/ID. The information is stored in the customer table along with the roles. The user then lands on the dashboard page based on their roles. To understand each user’s flow, we separate it into 3 categories role wise :

A. Admin - Upon logging in, the admin can view the dashboard that has event requests. The admin ensures that the event is in compliance with the policies of the company GoTickets. Once the event reviewing is done, the admin updates the event data store with the status “approved or disapproved”. The system notifies the event BP of this update. 

B. Business Partner - Upon logging in, the business partner (BP) can view a dashboard with their registered events. Every BP has to pay a yearly subscription to register themselves on the website. The subscriptions vary depending on the number of events a BP is allowed to post. The subscriptions are stored in a Static subscription table. Once the BP provides their CC details, the system sends them to the Credit Card Clearing House for approval. Upon approval, the BP is notified of successful payment and an order receipt is generated, that is stored in a BP order data store. Once the registration is complete, the BP can submit their event request to the system admin by filling some key details about the event like event duration, genre, type, description, list of actors, directors, producers etc. Upon the system admins approves the event request, the event is ready to be displayed on the website dashboard. At the end of the event cycle (i.e. till an event exists on our system), the record of sales is shared with the respective event BP. This information is stored in the sales data store. The system pays x amount of sales income to the event BP at the end of every event cycle. This information is also stored in the sales data store.

C. Customer - Upon logging in, the customer can view all events on the dashboard. The website displays events based on the city of the customer, however the customer can change their city preferences to view events in other places. The customer gets to view events based on the time, genre, type of event like movie, stand-up comedy, theater, exhibitions etc. The website displays the ratings for each. The customer selects an event, within an event, he/she enters the event time and venue, and then finally selects his/her preferred seats and adds it to their cart. All these options are displayed to the user for selection. The user must select at least one ticket to proceed further. The website then displays a menu of food & beverages available at the venue for that event & time. The user chooses (optional) one or more food/beverages and adds it to the cart with event tickets. During the above selections, if at any point, the event/ticket/food become unavailable, the system notifies the customer of the same and provides them with the best alternative. The system also notifies the food/beverage vendor manager with the out-of-stock items. The user can approve (or disapprove) the new suggestion and the cart is updated. Finally the user is prompted to pay for the order value. The order values consist of cart value, tax value and discount value thereby displaying the sum total to the user. The tax value is stored in a static tax data store where the tax is calculated based on the city. The discount value is obtained from the discount data store where discount is calculated based on the order frequency of the user. Once the user provides their CC details, the system sends them to the Credit Card Clearing House for approval. Upon approval, the user is notified of successful payment and an order receipt. The order is recorded in the Customer order data store. The system updates the event, tickets and food/beverages data store with the sold items. Post event, the system prompts the user to rate the event on a scale of 1 to 5. The user input is stored in the ratings data store. The event ratings get calculated based on this user input and is displayed on the event dashboard.

Project Sponsor : GoTickets enterprise.

Business Need: Project has been initiated to provide information and services about various events happening across the country and provide a one stop portal for all events’ ticketing needs , enabling scheduling according to the geographic locations, time preferences etc. A user can either host an event or choose to be a consumer for an event. 

Business Requirement : Using the website or application, customers will be able to search for and purchase event ticket/s, along with food/beverages. The specific functionality that the system should have includes the following : 
Search and browse events based on categories, title, locations(city), timings, price and rating etc. 
Check the availability of the event based on user search.
Enable users to book the tickets for the event. 
Allow users to book food/beverages along with the booking of tickets.
Get payment from the user and provide order confirmation for the same.
 Request user to provide feedback post event.
Get event details from the Business Partner.
Ability to create an event on the website.
Allowing the admin to approve/disapprove newly created events.

Business Value : We expect that GoTickets will increase sales by enabling existing customers to book an event from a wide variety of events’ list and reaching new customers by practicing creative marketing over various platforms. With efficient ticket & food inventory management and lesser event booking failures, customer satisfaction will increase. Conservative estimates of tangible value to the company include the following: 
$350,000 in sales from booking events. 
$100,000 in increased customer satisfaction due to efficient inventory management 
$100,000 additional revenue is generated from the discounts offered.
By delivering a one stop solution for all the ticketing needs, not only does it promote time efficiency but generates $200,000 revenue.

Special Issues Or Constraints :
 There is a discussion over how to incorporate the web traffic of users who are just there to browse and not register or create accounts.
Because customers have access to various other websites where they can browse  and book events from, we need to bring this system to market as soon as possible so we don't lose business. 
The current patrons have been asking for worldwide ticketing facilities, we need to provide this service to avoid competition, thereby resulting in loss of business.

 Nonfunctional requirements:
1. Operational 
  1.1 Event database will be constructed to facilitate searches based on different parameters like location, event type and descriptions, price etc.
  1.2 The system will run on any web browser.
  1.3 The system can run on mobile devices.

2. Performance
  2.1 Downtime after a failure of the system shall not exceed 4 hours.
  2.2 The meantime to view a webpage over a 56kbps modem connection shall not exceed 2 seconds.
  2.3 The system should be available for use 24 hours per day, 365 days per year
  2.4 The system should support 5000 simultaneous users.

3. Security
  3.1 Only the admins can view the event requests on the system.
  3.2 Transaction data must be transmitted in encrypted form.
  3.3 The system includes all available safeguards from viruses, worms, Trojan horses etc.
  
4. Cultural and political
  4.1 All software shall be written in the USA.
  4.2 The system should be able to distinguish between U.S. currency and currency from other nations. 
  4.3 The system shall not use icons that could be considered offensive in any of the marketing counties/areas.
  4.4 Personal information is protected in compliance with the Data Protection Act. 




