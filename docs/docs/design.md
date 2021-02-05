# Software Design
The design document will have a functional description of the application's core pages, a UML diagram, a sequence diagram, a wireframe to provide a visual representation of the application, and the design philosophy behind it.

Technologies

The P.A.L.S CRM system will be a react-django application with SQL databases.  

Login Page

The CRM system has two different kinds of users, tutors and administrators. Each has different roles and responsibilities within the application. Therefore, requiring two different dashboards. To establish this differentiation the user will be met with a login page upon entering the application. Based on the privileges of the login credentials entered, the user will proceed to either the tutor or admin dashboard. 

Admin Dashboard

The admin needs to be able to create student profiles, tutor accounts, other admin accounts, events, and courses, so these will be grouped under the enrollment tile. They will each have a unique page that can be filled out and appended to the database. The admin must be able to pair students with tutors, courses, and events. Like profile creation, this will be handled by the enrollments tile. Any newly created tutors, students, courses, and events will be added to the lists in the enrollments tile automatically. All associations will allow many-to-many pairing. The admin will be able to view donors using a nav bar button. Any reports submitted by tutors will be visible and scrollable for admins in the reports tile, allowing them to either approve or deny any submissions. Admins will also be able to create their own reports on the number of students, number of tutors, and hours spent tutoring or learning. And, all the information will combine with prior reports providing key statistics in the analytics tile.
	
Key subpages	
These are the core components of the app that will be used regularly.

Enrollments: Will be used to pair students with tutors, events, and courses by displaying lists for each and allowing pairing using a fragment. Designed with the intent of limiting the number of times a student, course or event name has to be entered.

Reports: Will have a button to create a report and a viewable list of reports in need of approval. Admins will also have an option to create new reports for tutors

Analytics: Will provide important analytics based on data from all reports
	

Tutor Dashboard

The tutor will be able to view their schedule on their dashboard and add appointments, which will display a list of paired students. They will be able to see what reports they have submitted on the right side of the screen. And will be able to file out forms using the create reports tile on the left.


## Architecture/Component Diagram
This is a short description of the architecture.
[![Architecture](https://raw.githubusercontent.com/UAlberta-CMPUT401/example-documentation/master/docs/images/architecture.png)](https://raw.githubusercontent.com/UAlberta-CMPUT401/example-documentation/master/docs/images/architecture.png)

## UML Class Diagram
This is a short description of logical entities of the domain in a UML diagram.
[![UML](https://raw.githubusercontent.com/UAlberta-CMPUT401/example-documentation/master/docs/images/UML.png)](https://raw.githubusercontent.com/UAlberta-CMPUT401/example-documentation/master/docs/images/UML.png)

## Sequence Diagram
The sequence diagram describes the the core dynamic behaviors of the system.

[![Sequence](https://raw.githubusercontent.com/UAlberta-CMPUT401/example-documentation/master/docs/images/sequence.png)](https://raw.githubusercontent.com/UAlberta-CMPUT401/example-documentation/master/docs/files/sequence.pdf)
