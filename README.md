# Edu-Flow
Edu-Flow is an online school management system designed to streamline academic operations. Manage student records, schedule classes, and facilitate seamless communication between teachers, students. With features like automated grading, secure payments, Edu-Flow simplifies school administration, making learning more efficient and organized.

  

## Team members
<table>
	 <thead> 
		 <tr> 
			 <th>ID</th> 
			 <th>Name</th> 
			 <th>Email</th> 
			 <th>Role</th> 
		 </tr> 
	 </thead> 
	 <tbody> 
		 <tr> 
			 <td>20220104071</td> 
			 <td>Zarif Mahmud</td> 
			 <td></td> 
			 <td>Lead (Frontend+Backend+Database)</td> 
		 </tr> 
		 <tr> 
			 <td>20220104060</td> 
			 <td>Ma.Tanzil Islam</td> 
			 <td>tanimtanzilislam9@gmail.com</td> 
			 <td>Frontend+backend+Database</td>   
		 </tr> 
		 <tr> 
			 <td>20220104063</td> 
			 <td>Sanaf Salehin</td> 
			 <td>sanafsalehin@gmail.com</td> 
			 <td>Frontend+Backend+Database</td>   
		 </tr> 
		 <tr> 
			 <td>20220104069</td> 
			 <td>Afia Adilah</td> 
			 <td>afiaadilah246@gmail.com</td> 
			 <td>Frontend+Backend</td>   
		 </tr> 
	 </tbody> 
 </table>

  

## Target Audience

  

The target audience for Edu-Flow includes schools, colleges, and educational institutions in cities like Dhaka and Chattogram, particularly school administrators, teachers, students, and parents seeking a streamlined academic experience. Working parents who want real-time updates on their child's progress, institutions looking to digitize operations, and educators needing efficient class management tools are key segments. Emphasis should be on affordability, user-friendly interfaces, and integration with local payment methods like bKash. Tech-savvy students and parents who rely on digital platforms for communication and learning can be engaged through targeted marketing campaigns. By addressing these diverse needs, Edu-Flow can become an essential solution in Bangladesh's evolving education sector.

  
  

## Tech Stack
<table>
	 <thead> 
		 <tr> 
			 <th>Teck Stack</th> 
			 <th>We Use</th> 
		 </tr> 
	 </thead> 
	 <tbody> 
		 <tr> 
			 <td>Backend</td> 
			 <td>Laravel</td> 
		 </tr> 
		 <tr> 
			 <td>Frontend</td> 
			 <td>php</td>   
		 </tr> 
		 <tr> 
			 <td>Database</td> 
			 <td>phpMyAdmin</td>  
		 </tr> 
		 
		 
	 </tbody> 
 </table>
  
## UI Design

Figma Design   : <a href="https://www.figma.com/design/698MIXaZPQRPmjMFVvdZzh/Untitled">Figma Design Link</a>


## Project Features

### User Section
<ul>
	<li>Multi User Authentication</li>
	<li>Student, Teacher, and Admin Profiles</li>
	<li>CRUD Operations for User Management</li>
	<li>Search/Filter Students & Staff</li>
	<li>Fee Payment & Invoice Management</li>
	
</ul>

<ul>
	<li>Multi-Teacher Authentication</li>
	<li>Single Admin for a Single Institution</li>
	<li>Manage Courses,Subjects</li>
	<li>CRUD Operations for Class & Student Records</li>
	
</ul>

### Admin Section
<ul>
	<li>Single Admin Authentication</li>
	<li>Forgot Password & Account Recovery</li>
	<li>Manage Student & Teacher Records</li>
	<li>Manage Fee Payments & Transactions</li>
	<li>Announcement Management for Important Updates</li> 
</ul>
##  API Endpoints
### *Authentication*

#### Customer Authentication

-   *POST* /api/customers/register - Customer registration.
-   *POST* /api/customers/login - Customer login.
-   *POST* /api/customers/logout - Customer logout.
-   *POST* /api/customers/forgot-password - Forgot password (email recovery).
-   *POST* /api/customers/reset-password - Reset password with token.

#### Restaurant Authentication

-   *POST* /api/restaurants/register - Restaurant owner registration.
-   *POST* /api/restaurants/login - Restaurant owner login.
-   *POST* /api/restaurants/logout - Restaurant owner logout.
-   *POST* /api/restaurants/forgot-password - Forgot password.
-   *POST* /api/restaurants/reset-password - Reset password with token.

#### Admin Authentication

-   *POST* /api/admin/login - Admin login.
-   *POST* /api/admin/logout - Admin logout.

----------

### *Customer Management*

-   *GET* /api/customers/me - Fetch customer details (My Account).
-   *PUT* /api/customers/me - Update customer account details.
-   *DELETE* /api/customers/me - Delete customer account.

----------

### *Restaurant Management*

#### By Restaurant Owner

-   *GET* /api/restaurants/me - Fetch restaurant owner details.
-   *PUT* /api/restaurants/me - Update restaurant owner details.
-   *DELETE* /api/restaurants/me - Delete restaurant account.
-   *GET* /api/restaurants/my-orders - View orders placed at their restaurant.
-   *PATCH* /api/restaurants/my-orders/:orderId - Update order status (e.g., accepted, prepared, delivered).
-   *PATCH* /api/restaurants/menu/prices - Update menu item prices.
-   *POST* /api/restaurants/menu - Add a new menu item.
-   *PUT* /api/restaurants/menu/:itemId - Edit menu item details.
-   *DELETE* /api/restaurants/menu/:itemId - Remove menu item.

#### By Admin

-   *GET* /api/restaurants - Fetch all restaurants.
-   *PATCH* /api/restaurants/:restaurantId/approve - Approve restaurant registration.
-   *DELETE* /api/restaurants/:restaurantId - Remove restaurant.

----------

### *Order Management*

#### Customer Orders

-   *POST* /api/orders - Place an order with multiple items from a restaurant.
-   *GET* /api/orders - View all orders by the customer.
-   *GET* /api/orders/:orderId - View details of a specific order.
-   *DELETE* /api/orders/:orderId - Cancel an order (if not yet processed).

#### Payment Options

-   *POST* /api/payments/cash-on-delivery - Apply cash on delivery.
-   *POST* /api/payments/online - Apply online payment (e.g., via bKash, card).
-   *POST* /api/payments/verify/:paymentId - Verify online payment.

----------

### *Menu Management*

-   *GET* /api/menu - Fetch menu for a restaurant.
-   *GET* /api/menu/:itemId - Fetch details of a specific menu item.

----------

### *Admin Panel Management*

-   *GET* /api/admin/dashboard - Admin dashboard data (e.g., total sales, active restaurants).
-   *GET* /api/admin/customers - Fetch all customers.
-   *DELETE* /api/admin/customers/:customerId - Remove a customer.
-   *GET* /api/admin/restaurants - Fetch all restaurants.
-   *PATCH* /api/admin/restaurants/:restaurantId - Modify restaurant details.
-   *GET* /api/admin/orders - View all orders.

----------

### *Search and Filtering*

-   *GET* /api/restaurants/search - Search restaurants by name, cuisine, or location.
-   *GET* /api/menu/search - Search menu items across restaurants.

----------

### *Reviews and Ratings*

-   *POST* /api/reviews - Add a review for a restaurant.
-   *GET* /api/reviews/:restaurantId - Fetch reviews for a restaurant.
-   *PATCH* /api/reviews/:reviewId - Edit a review.
-   *DELETE* /api/reviews/:reviewId - Delete a review.<?php
## Milestones
<table>
	 <thead> 
		 <tr> 
			 <th>Milestones</th> 
			 <th>We Cover</th> 
		 </tr> 
	 </thead> 
	 <tbody> 
		 <tr> 
			 <td>Checkpoint 1</td> 
			 <td>
				 <ul>
					<li>Frontend, Backend, Database setup</li>
					<li>Admin registration and login pages</li>
					<li>Admin authentication</li>
                    <li>Admin Dashboard setup</li>
                    <li>Academic management</li>
                    <li>Add and view Record of academic year</li>
                    <li>Class Management</li>
                    <li>Add and view Record of Classes</li>
                    <li>Student management</li>
		     <li>Add and View studens records</li>
					 
				</ul>
			</td>
		 </tr> 
		 <tr> 
			 <td>Checkpoint 2</td> 
			 <td>
				 <ul>
                     <li>Table for User, Restaurants and MenuItem at Database</li>
					 <li>Order History</li>
					 <li>Multi Item Cart functionality</li>
					 <li>Approve or Reject new Restaurants registration by Admin</li>
					 <li>Restaurant Dash Board</li>
					 <li>Admin Dashboard</li>
				 </ul>
			 </td>   
		 </tr> 
		 <tr> 
			 <td>Checkpoint 3</td> 
			 <td><ul>
					 <li>Customers can search restaurants by name or foodItem name</li>
					 <li>Customers can leave reviews for Restaurants</li>
					 <li>Admin can remove inactive or problematic restaurants</li>
					 <li>Payment options by Stripe</li>
					 <li>Approve or Reject new Restaurants registration by Admin</li>
				 </ul>
				</td>  
		 </tr> 
	 </tbody> 
 </table>
