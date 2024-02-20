Please find the below steps for the documentation

**Task 1**: Spacefaring Data Model

First, I have defined data model in a CDS (Core Data Services) file -->  data-model.cds with the below fields

ID, stardustCollection, wormholeNavigationSkill, originPlanet, spacesuitColor, department and position. 

Please note that the relationship is established with departments and posi1ons entities.

**Task 2**: Cosmic Service Definition

I have defined a CAP service definition for the Galactic Spacefarer entity -- > cat-service.cds

Enabled draft for Spacefarers entity because the CRUD operations needs to be performed.

and other 2 entities(Departments, Positions) I have defined and restricted with read only annotation.

**Taks 3**:  Cosmic Event Handlers

Implemented After event handler for sending an email when ever a new entry is created on spacefarer

Please note that I have used nodemailer library to send emails which is working as expected. SendGrid would be another option but for this I need to create a destination. So to make it more simpler I have used Nodemailer library. 

The service definition have been declared for before event handler for spacefarer .

I Assume that the validation logic is as follows:
Stardust collection must be a positive integer.
Wormhole navigation skill must be one of 'Beginner', 'Intermediate', 'Expert'.

**Task 4**: Galactic List Report Fiori Application

Created the list report fiori elements application and all the fields in Spacefarers entity are available in the application. Also it supports the sorting, filtering, and pagination. 

We have create button on header level where we can create a new spacefarer and delete button will be enabled once we select one of the line item/s. 

**Task 5**: Cosmic Object Page Fiori Application

User can click on the respective line item and it will navigate to object page. User has possiblity to edit all the fields. 

**Please note** : I have used .csv files to store data. You can also delete the folder csv and enter your own entries with create button. I will also attach the PDF document for application demonstration. Also I have deleted node modules from the project , please install node modules after importing the project to BAS.
