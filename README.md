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
#### Teacher Authentication
- GET /api/teacher/login - Show login page for teachers.
- POST /api/teacher/authenticate - Authenticate teacher login.
- GET /api/teacher/dashboard - Teacher dashboard (requires authentication).
- GET /api/teacher/logout - Logout teacher.

#### Student Authentication
- GET /api/student/login - Show login page for students.
- POST /api/student/authenticate - Authenticate student login.
- GET /api/student/dashboard - Student dashboard (requires authentication).
- GET /api/student/logout - Logout student.
- GET /api/student/change-password - Show change password page.
- POST /api/student/update-password - Update student password.

#### Admin Authentication
- GET /api/admin/login - Show login page for admin.
- GET /api/admin/register - Show registration page for admin.
- POST /api/admin/login - Authenticate admin login.
- GET /api/admin/logout - Logout admin.
- GET /api/admin/dashboard - Admin dashboard (requires authentication).
- GET /api/admin/form - Show form page for admin.
- GET /api/admin/table - Show table page for admin.

#### Academic Year Management
- GET /api/academic-year/create - Show form to create an academic year.
- POST /api/academic-year/store - Store a new academic year.
- GET /api/academic-year/read - Fetch all academic years.
- GET /api/academic-year/delete/{id} - Delete an academic year.
- GET /api/academic-year/edit/{id} - Show form to edit an academic year.
- POST /api/academic-year/update - Update an academic year.

#### Announcement Management
- GET /api/announcement/create - Show form to create an announcement.
- POST /api/announcement/store - Store a new announcement.
- GET /api/announcement/read - Fetch all announcements.
- GET /api/announcement/edit/{id} - Show form to edit an announcement.
- POST /api/announcement/update/{id} - Update an announcement.
- GET /api/announcement/delete/{id} - Delete an announcement.

#### Class Management
- GET /api/class/create - Show form to create a class.
- POST /api/class/store - Store a new class.
- GET /api/class/read - Fetch all classes.
- GET /api/class/read/edit/{id} - Show form to edit a class.
- POST /api/class/update - Update a class.
- GET /api/class/delete/{id} - Delete a class.

#### Subject Management
- GET /api/subject/create - Show form to create a subject.
- POST /api/subject/store - Store a new subject.
- GET /api/subject/read - Fetch all subjects.
- GET /api/subject/delete/{id} - Delete a subject.
- GET /api/subject/edit/{id} - Show form to edit a subject.
- POST /api/subject/update/{id} - Update a subject.

#### Assign Subjects to Class
- GET /api/assign-subject/create - Show form to assign a subject to a class.
- POST /api/assign-subject/store - Store subject assignment.
- GET /api/assign-subject/read - Fetch all assigned subjects.
- GET /api/assign-subject/delete/{id} - Delete an assigned subject.
- GET /api/assign-subject/edit/{id} - Show form to edit an assigned subject.
- POST /api/assign-subject/update/{id} - Update an assigned subject.

#### Teacher Management
- GET /api/teacher/create - Show form to create a teacher.
- POST /api/teacher/store - Store a new teacher.
- GET /api/teacher/read - Fetch all teachers.
- GET /api/teacher/edit/{id} - Show form to edit a teacher.
- POST /api/teacher/update/{id} - Update a teacher.
- GET /api/teacher/delete/{id} - Delete a teacher.

#### Assign Teacher to Class
- GET /api/assign-teacher/create - Show form to assign a teacher to a class.
- POST /api/assign-teacher/store - Store teacher assignment.
- GET /api/assign-teacher/list - Fetch assigned teachers.

_____________________________________________________________________________

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
