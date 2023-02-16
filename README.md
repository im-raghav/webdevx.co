## How to run the app?

```bash
#-- Setup and start the server
cd server
npm install # or yarn install
npm start # or yarn start

#-- Setup and start the client
cd client
npm install # or yarn install
npm start # or yarn start
```

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Q. Describe any other approaches that can be better than the above solution performance-wise. 
Ans. 
While WebSockets can be a good approach for real-time communication between a client and a server, it may not be the most performant solution for saving data to a server and retrieving it across different devices. Here are a few alternative approaches to consider:

-Server-side storage: Instead of relying on local storage on the client-side, we could store the user's progress on the server-side, such as in a database. This would ensure that the progress is accessible across different devices and browsers, without requiring real-time communication between the client and server.

-API calls: Another approach could be to have the client make API calls to the server to save and retrieve the user's progress. This would allow for more control over the data being transmitted and can be used to optimize performance by sending only the data that has been modified.

Overall, the best approach will depend on the specific requirements of application, as well as performance and security needs. It's important to consider factors such as the size and frequency of the data being transferred, the level of security required, and the resources available to store and retrieve the data.
--------------------------------------------------------------------------------------------------------------------------------------------------------------------
OPEN QUESTION :
1) What is your approach to debugging the backend application? 
Ans. 
-Logging: By logging the relevant information at different stages of the application, we can easily trace the execution path and identify the source of any errors. This is particularly helpful when an application is deployed in a production environment, where it's not always feasible to debug the application interactively.

-Use Debuggers: We can use a debugger to step through your code line by line and inspect the values of variables and other data structures in real-time. This can help us identify where the problem is and how to fix it.

-Unit Testing: Unit tests can help catch issues early in the development process before they become larger problems. By writing and running tests regularly, we can quickly identify when changes to the codebase have introduced errors.

-Reproduce the error: In order to fix a bug, it's important to be able to reproduce the error. This can be challenging when debugging backend applications since there are often many moving parts involved. However, by identifying the conditions that cause the bug to occur, we can isolate the issue and fix it.

-Break the problem into smaller parts: Debugging a complex application can be overwhelming. Breaking the problem into smaller parts can help make it more manageable. You can start by identifying the most critical features and functions of your application and focus your debugging efforts on those areas.

-Collaborate: Collaborating with colleagues, or other developers can help us gain new insights and identify solutions we might not have considered before.
--------------------------------------------------------------------------------------------------------------------------------------------------------------------
2) What are migrations in a database? Why they are important? Describe how you would solve the data type conversion, and character set mismatch issues when applying
schema conversion and data migration.
Ans. 
Migrations in a database refer to the process of making changes to the schema or structure of the database, such as adding or modifying tables, columns, indexes, or constraints. Migrations are important because they allow for the smooth and controlled evolution of the database over time, while preserving the existing data and minimizing downtime.

Here are some general steps you can take to solve issues with data type conversion and character set mismatch:

-Identify the problem: First, we need to identify the specific issue with the data type conversion or character set mismatch. This can be done by analyzing error messages, examining the data itself, and reviewing the database documentation.

-Plan the solution: Once we have identified the issue, we can plan the solution. This may involve modifying the existing data to conform to the new data type or character set, or modifying the conversion process to better handle the data.

-Convert the data: Once we have a plan in place, we can convert the data. This may involve using a conversion tool or writing custom scripts to modify the data. It's important to thoroughly test the conversion process and ensure that the converted data is correct and consistent.

-Verify the data: After the data has been converted, it's important to verify that it has been converted correctly. This may involve running validation scripts or spot-checking the data to ensure that it conforms to the new data type or character set.

-Document the changes: Finally, it's important to document the changes to the database schema and any modifications made to the data. This will help ensure that future migrations are smooth and can be easily understood.

