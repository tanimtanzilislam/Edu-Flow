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

### Teacher Section
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

Authentication
Teacher Authentication
POST /teacher/login - Teacher login.
POST /teacher/authenticate - Teacher authenticate.
POST /teacher/logout - Teacher logout.
Student Authentication
POST /student/login - Student login.
POST /student/authenticate - Student authenticate.
POST /student/logout - Student logout.
Admin Authentication
POST /admin/login - Admin login.
POST /admin/authenticate - Admin authenticate.
POST /admin/logout - Admin logout.
Teacher Management
GET /teacher/dashboard - Teacher dashboard.
GET /teacher/create - Create a new teacher.
POST /teacher/store - Store a new teacher.
GET /teacher/read - View list of teachers.
GET /teacher/edit/{id} - Edit teacher details.
POST /teacher/update/{id} - Update teacher details.
GET /teacher/delete/{id} - Delete a teacher.
Student Management
GET /student/dashboard - Student dashboard.
GET /student/create - Create a new student.
POST /student/store - Store a new student.
GET /student/read - View list of students.
GET /student/edit/{id} - Edit student details.
POST /student/update/{id} - Update student details.
GET /student/delete/{id} - Delete a student.
Academic Year Management
GET /academic-year/create - Create a new academic year.
POST /academic-year/store - Store an academic year.
GET /academic-year/read - View list of academic years.
GET /academic-year/edit/{id} - Edit an academic year.
POST /academic-year/update/{id} - Update academic year details.
GET /academic-year/delete/{id} - Delete an academic year.
Announcement Management
GET /announcement/create - Create a new announcement.
POST /announcement/store - Store an announcement.
GET /announcement/read - View all announcements.
GET /announcement/edit/{id} - Edit an announcement.
POST /announcement/update/{id} - Update an announcement.
GET /announcement/delete/{id} - Delete an announcement.
Class Management
GET /class/create - Create a new class.
POST /class/store - Store a class.
GET /class/read - View all classes.
GET /class/edit/{id} - Edit class details.
POST /class/update/{id} - Update class details.
GET /class/delete/{id} - Delete a class.
Subject Management
GET /subject/create - Create a new subject.
POST /subject/store - Store a subject.
GET /subject/read - View all subjects.
GET /subject/edit/{id} - Edit subject details.
POST /subject/update/{id} - Update subject details.
GET /subject/delete/{id} - Delete a subject.
Assign Subject to Class
GET /assign-subject/create - Assign a subject to a class.
POST /assign-subject/store - Store subject-class assignment.
GET /assign-subject/read - View subject-class assignments.
GET /assign-subject/edit/{id} - Edit subject-class assignment.
POST /assign-subject/update/{id} - Update subject-class assignment.
GET /assign-subject/delete/{id} - Delete subject-class assignment.
Assign Teacher to Class
GET /assign-teacher/create - Assign a teacher to a class.
POST /assign-teacher/store - Store teacher-class assignment.
GET /assign-teacher/list - View list of teacher-class assignments.
GET /assign-teacher/read/{id} - View a specific teacher-class assignment.
GET /assign-teacher/edit/{id} - Edit teacher-class assignment.
POST /assign-teacher/update/{id} - Update teacher-class assignment.
Fees Management
Fee Head Management
GET /fee-head/create - Create a new fee head.
POST /fee-head/store - Store a fee head.
GET /fee-head/read - View all fee heads.
GET /fee-head/edit/{id} - Edit a fee head.
POST /fee-head/update/{id} - Update a fee head.
GET /fee-head/delete/{id} - Delete a fee head.
Fee Structure Management
GET /fee-structure/create - Create a new fee structure.
POST /fee-structure/store - Store a fee structure.
GET /fee-structure/read - View all fee structures.
GET /fee-structure/edit/{id} - Edit a fee structure.
POST /fee-structure/update/{id} - Update a fee structure.
GET /fee-structure/delete/{id} - Delete a fee structure.

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
					<li>Customer registration and login pages</li>
					<li>customer authentication</li>
                    <li>Admin panel setup</li>
                    <li>Restaurant authentication</li>
                    <li>Restaurant panel setup</li>
                    <li>Customer Profile Setup</li>
                    <li>Admin Backend Category</li>
                    <li>fetching a list of restaurants and  menu display page</li>
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
