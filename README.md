# CRUD
This is a simple Node.js application that uses Express framework to create a CRUD (Create, Read, Update, Delete) web application for employee management.

The application uses MongoDB as the database. The models/Employee.js file defines the Employee model. The dbConnect.js file contains the code to connect to the database.

The index.js file is the main file of the application. It defines the routes for the application. The get / route renders the index.hbs view which displays a list of all employees. The get /add route renders the add.hbs view which allows users to add a new employee. The post /add route creates a new employee in the database. The get /delete/:_id route deletes an employee from the database. The get /update/:_id route renders the update.hbs view which allows users to update an existing employee. The post /update/:_id route updates an existing employee in the database.

To run the application, install the dependencies by running the following command:

```
npm install
```

Then, start the application by running the following command:

```
npm start
```

The application will be running on port 3000. You can access the application by visiting http://localhost:3000 in your browser.

The `add.hbs` file is a handlebars template that is used to render the add record form. The form has the following fields:

* Name
* Age
* Salary
* Email address
* Mobile number
* Designation
* City

The form is submitted to the `/add` route.

The `index.hbs` file is a handlebars template that is used to render the main page of the CRUD application. The template includes a header, a navbar, a table of data, and a footer. The header includes the title of the page and a link to the add page. The navbar includes links to the main page, the add page, the update page, and the delete page. The table of data lists the ID, name, age, salary, email, phone, designation, and city of each record in the database. The footer includes the copyright information.

Here is a step-by-step explanation of the code in the `index.hbs` file:

1. The first line of the file includes the handlebars template engine.
2. The second line includes the header template.
3. The third line includes the title of the page.
4. The fourth line includes the navbar template.
5. The fifth line includes the container div.
6. The sixth line includes the h5 tag with the title of the application and a link to the add page.
7. The seventh line includes the table-responsive div.
8. The eighth line includes the table tag.
9. The ninth line includes the header row of the table.
10. The tenth line includes the loop over the data array.
11. The eleventh line includes the table row for each record in the data array.
12. The twelfth line includes the link to the update page for each record.
13. The thirteenth line includes the link to the delete page for each record.
14. The fourteenth line includes the footer template.
15. The fifteenth line includes the copyright information.

The `update.hbs` file is a handlebars template that is used to render the update record form. The file starts with the `{{>header}}` and `{{>navbar}}` handlebars templates, which render the header and navbar components respectively.

The next section of the file contains the `<div class="container">` element, which is used to create a container for the form. The container contains a heading that says "CRUD Application" and a form that is used to update the record.

The form has six input fields, one for each of the following fields: name, age, salary, email, phone, designation, and city. The form also has a submit button that is used to submit the form data to the server.

The `update.hbs` file is a simple template that can be used to render the update record form. The template uses handlebars syntax to render the header, navbar, and form components.

