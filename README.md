# CRUDApp
Created for academic purposes in Mapua University under course CSS123L in 2023, now archived. Readme ripped from attached PDF report file.

## Alice Lot & Co. Real Estate Management Program Project
A project in Object-oriented Programming (CSS123-Laboratory)

# PROJECT CONTEXT:
## DESCRIPTION:
This is a Real-Estate program built from the ground up using Java Language. The primary design patterns used in its development are the Factory Method Pattern and the Decorator Pattern. This program allows for the modification, deletion, and addition of lots per block in subdivisions. The program is capable of handling up to 20 lots per block within a 5-block subdivision. The cost, transaction dates, and name of purchasers are also recorded per lot. Not only that, but the Report Tab also gives a detailed review of the lot sales and statistics.

## PURPOSE:
This program is built with the purpose of making real-estate businesses easier to be monitored and managed. This program provides a linear and organized structure that allows for a more efficient management of real-estate transactions. Thus, streamlining workflow in administrative tasks such as updating lot status and keeping track of sale statistics and real-estate business reports.

## BENEFIT:
This program shall mainly benefit real-estate owners and corporations. To elaborate, this program will grant the realtors a better experience in managing their real-estate businesses due to its linear design and organized structure. Thus, boosting sales efficiency and swift transactions with the support of a secure, database-backed system.

# PROJECT DESIGN:
## UML Use Case Diagram:
![UML Use Case Diagram](/readmeImages/UseCaseDiagram.png)

- Actors in this diagram are known as admins, since they are the users who usually deal
with lot management in the real estate business. An actor should have login credentials
such as a username and password.
- The Alice Lot & Co. System is associated with the lot management system as it is
responsible for the functionality of the program.
- The Alice Lot & Co. System is associated with the Filter & Search as it is responsible for
handling tailored details needed by the admin.
- Filter & Search are included in the Lot Management System by default as it is part of the
functionality of the lot management system of Alice Lot. & Co. Real Estate Program.
- The Alice Lot & Co. Database is associated with the login system as it is responsible for
storing the login credentials of the admins.
- The Alice Lot & Co. Database is associated with the statistical report section as it is
responsible for storing the details of each lot recorded and stored in the program’s
database.
- The Admin can either access the lot management system or the statistical report section.

## UML Class Diagrams:
![Whole UML Class Diagram](/readmeImages/ClassDiagram.png)

### Part 1 - Alice Loc & Co. System Diagram:

![System Diagram](/readmeImages/SystemDiagram.png)

This part of the diagram represents the Lot Management System part of the Alice Lot & Co. Real Estate Program. It shows the classes involved in determining the status of the registered lot as well as the credentials of each lot registered in the Lot & Co. Real Estate Program’s database. Using the Factory Design Pattern, the admins will be able to generate or alter the status of each of their client’s registered lots. The Lot management system also allows admins to search or filter results for searching specific lots using the search function which will be explained in the **Part 2** of the Class Diagrams for this program. Classes *ReservedStatus, ForSaleStatus,* and *Purchased Status* are the implemented objects of the *Status* Interface, which determines if the Lot is reserved for a person. The lot is up for sale, or was recently purchased by a customer. For the statistical report section, which class name is named as “Report”, it gets its statistical results by describing the amount of lots registered in the program’s database, such as the average amount of lot size and lot price of all available lots as well as tally the amount of lots under each status available.

### Part 2 - Alice Lot & Co. Filter System Diagram:

![Filter System Diagram](/readmeImages/FilterSystemDiagram.png)

This part of the diagram represents the Lot Management Filter & Search System part of the Alice Lot & Co. Real Estate Program, which is part of the functionality of the Main Lot Management System of the Program. It shows the classes involved in filtering results returned by the program
to better get the necessary information needed by the admin. By default, the lot management system will display all available lots stored in the database. But with the *Search* interface of the Lot Management System, it will be able to display lots based on the admin’s needs using the
available filters. The admin can search based on the lot’s block number, minimum and maximum price and size, and its status.

## Design Patterns Used:
### Factory Method Pattern:
![Factory Method  Pattern](/readmeImages/FactoryMethodPattern.png)
The program uses the Factory Method Pattern when programming the core features of the Real Estate Management Program such as generating new lots for sale, determining the status for each lot, and building accounts that manage the software. This is best seen in the **Part 1 Class of the Diagram**, as the class file *“Status Factory”* generates the status of each lot available in the real estate business.

### Decorator Pattern:
![Decorator Pattern](/readmeImages/DecoratorPattern.png)
The program uses the Decorator Pattern when programming the filter and search functionality of the program, allowing the user to search specific lots determined by their needs more precisely. This is best seen in the Part 2 of the Class Diagram, as the class file “LotSearchDecorator” implements class files that filter results based on specific parameters without fundamentally changing the code structure.

## Dependency Used:
### FlatLaf:
The ***FlatLaf*** developed by **JFormDesigner** is an open-source cross-platform Look and Feel for Java that was used to design the GUI of the Real Estate Management Program, which provides a minimalistic, elegant and modern type of feel in the program’s GUI.

# SAMPLE SCREENSHOTS:
## Log-in Page:
![Log-in Page](/readmeImages/LoginPage.png)
## Main Page
### Lot Listing:
![Lot Listing Page](/readmeImages/LotListingPage.png)
### Statistical Report Page:
![Statistical Report Page](/readmeImages/StatisticalReportPage.png)
### Adding and Editing Lot pop-up:
![Adding and editing Lot pop-up](/readmeImages/AddingandEditingPopup.png)