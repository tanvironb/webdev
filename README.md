# UIA Food and Beverage system management
### Section: 01
### Group: 04
### Members:
#### KEHMESS EL MOCTAR    |              (2113559)
#### FARUQ MD OMAR        |              (2134787)
#### AHMAD KHALEEL        |              (1927975)
#### HASSAN DAMAD         |              (2128989)
#### MD TANVIR AHMMED SHOPNO |           (2219061)



# Introduction
In a technological and advancing world, where time is a precious commodity, We will focus on  the necessity of efficiency, convenience and the availability of Foods and beverages in the mahallah canteens and the restaurants. This facility will be managed through a webpage at the International Islamic University Malaysia (IIUM). It will recognize the user experience for both students and mahallah’s canteen and other restaurants in UIA. 
We propose the implementation of a UIA food service should be more convenient. UIAfood will be a dedicated website linked with the International Islamic University Malaysia (IIUM), designed to enhance the dining experience for its community. This platform will provide students with comprehensive information about the various restaurants, their foods and their availability available within the university’s canteens, showcasing promotions and discounts to make the restaurants food and beverage which is affordable and convenient. Additionally, UIAfood extends its services beyond campus by connecting users with international restaurants, facilitating easy ordering and delivery from these establishments.
 This integration ensures that students have diverse and accessible food choices, both within and outside the university, streamlining the process of discovering various countries' cultural food and connecting all restaurants together in one page. 

# Objectives
Increased food accessibility and connecting the food and beverage stalls and also the mahallah canteens in one site for the students and others.
People can order foods from the mahallah canteens and the other UIA food stalls also facilitating delivery systems which will be allowing them to track their order.
Users may check the availability of the foods or shop before making the order from the site.     
Provide a user-friendly platform that is accessible to a wide range of users so that students and other people can give their desired foods from their place.
A low-cost, high-performance food and beverage service which may reduce the unavailability of foods in UIA among the students and other people in various situations.
To assist administrators in keeping track of ordering records, locating them in the database, and managing order details as well as cancelled orders.

					 				
			
# User Interface and Experience

 **Intuitive Design**:


The website will be designed to work seamlessly on various devices, including desktops, tablets, and smartphones.
Simple and clear menus and search functionalities will help users find what they need quickly.

**Restaurant Listings**:


Each restaurant will have extensive details available, including location, hours of operation, and contact information.
Menus will be displayed with descriptions, prices, and images of the dishes.

**Food Availability Tracking**:

Users will be able to see real-time updates on the availability of menu items to avoid ordering disappointments.
Notifications will alert users when popular items are back in stock.

### Ordering and Delivery System

**Seamless Ordering Process:**

Users can place orders through a straightforward and intuitive process.

**Delivery Management:**

The system will coordinate with delivery services to ensure timely and efficient food delivery. (remove?)
Users can track their orders in real-time from preparation to delivery.

**Payment Gateway Integration:**

The platform will support various payment methods, including credit/debit cards, online banking, and mobile wallets.
Transactions will be secure, using encryption and fraud detection for safe payment processing.

## Promotions and Discounts

**Exclusive Deals:**

The website will highlight ongoing promotions, discounts, and special deals from participating restaurants.

### Reviews and Ratings

**User Reviews:**

Users can rate their experiences and provide feedback through a rating system.

### Administrative Tools

**Order Management:**

Restaurant owners will have access to a dashboard to manage orders, update menus, and track sales.
Administrators can view and manage all orders, including their processing, preparation, and delivery statuses.


# Entity-Relationship Diagram (ERD) for the UIAfood system:


## Entities:
![ERD WEB DEV](https://github.com/tanvironb/webdev/assets/170326332/7db17011-9c5c-46b4-b2de-2de0c9f03f91)

**User**: Represents users of the system, including students and potentially staff/faculty.

**Attributes**: User ID (primary key), Name, Email, Phone number
**Restaurant**: Represents restaurants participating in the UIAfood system, including both on-campus canteens and off-campus restaurants.


**Attributes:** Restaurant ID (primary key), Name, Location (text or foreign key to a Location table), Contact Information (phone, website)
**Dish:** Represents individual food items offered by restaurants.


**Attributes:** Dish ID (primary key), Name, Description, Price, Image (URL or file reference)
**Order:** Represents an order placed by a user.


**Attributes:** Order ID (primary key), User ID (foreign key to User table), Restaurant ID (foreign key to Restaurant table), Order Date, Order Time, Status (e.g., Pending, Preparing, Delivered, Cancelled)
**Order_Item:** Connects orders with dishes (many-to-many relationship).


### Attributes (primary key): Order ID (foreign key to Order table), Dish ID (foreign key to Dish table), Quantity
### Relationships:
One user can place many orders (one-to-many between User and Order).
One restaurant can have many dishes (one-to-many between Restaurant and Dish).
One order can include many dishes (many-to-many between Order and Dish, represented by the Order_Item table).

# Sequence Diagram

![WhatsApp Image 2024-05-21 at 10 53 09_796e49db](https://github.com/tanvironb/webdev/assets/170326332/8e0c1807-cbef-4e9a-af55-5e5db810e61e)

# References
For website template https://bootstrapmade.com/demo/Yummy/ 
