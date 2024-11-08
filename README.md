# JessicaVaz_T3A1


# Q1 
During our course, we have been using GIT as it's widely known and it's a very popular choice for managing code and keeping track of code changes. Apart from Git, other common source control programs are Mercurial and Subversion. 

When using source control for a large project, we want to ensure the GIT covers all features, and also includes the documentation as it's very important in all scale programs. The repository is hosted on the platform GitHub which offers plenty of features including branch merge, code comparison and code collaboration.

The first step is to initialise a repository in the main or master branch, which will store the project's source code and it's files. When initialising the repository, we also need to add the README.md file which contains the project's documentation. README.md file contains all of the information about the program including name and description, table of contents, all the steps required to run the application, the usage cases, the tech stacked used to build the program, contribution guidelines, license information and plenty more. The gitignore template is another option we can add when initialising the project, this file will contain all the files git should ignore when pushing content to the repository.

Through the building process, different branches are created to allow developers to work on different features independently without code conflicts. It's recommended to create a different branch for each feature as this allows independently testing and experimenting without compromising the rest of the code. When creating news branches for specific features, the conventional name used is <b>feature</b>, this ensure a clear description of what's the purpose of the extra branch. Name example bellow:

    feature/authentication

With every commit, we should include meaningful messages to describe what changes has been added or changes. A good practise to have the type of commit before the message, they provide extra details for the commit messages. Other good practices includes keeping the message short and clear.

Examples of conventional commit bellow:
* git commit -m "docs: added a brief description" 
* git commit -m "feat: added a JWT to auth" 
* git commit -m "fix: fixed a bug in user auth fn" 
* git commit -m "test: test done in user's auth" 

Once all testing is complete and the code functions as intended, the feature branches can be merged into the main branch, which stores the source code and the production ready code. Features branches can also be deleted safely after being merged, however this is optional step. The first step to merge the branch is to perform a pull request. A pull request contains information describing the branch's purpose, and it's code. 

Developers working in the project can review the code, suggest improvements, provide feedbacks and ensure it doesn't have any conflicts with other existing branches. In case of an existing conflict, developers are required to solve the conflict first in order to proceed with the pull request. Another good feature is that Github makes it possible to assign reviewers and assignees to each branch or pull request. This ensures a structured review process and accountability for code quality.

When all required tasks and requirements has been reached, the pull request will be ready to merge. Once the process is done, an acknowledgement message will be provided, and all of the content from the extra branch will be merged into the main branch. Once all branches has been merged, and the code is working as intended, the code will be ready for deployment.


#### Git commits and pull requests example
Example of source control process from my past project in term 2 in Coder Academy.

![Example of git pull requests](./git1.png)


References:

Workbook assignment: JessicaVaz_T2A1-A

freeCodeCamp.org. (2022). How to Write Better Git Commit Messages – A Step-By-Step Guide. [online] Available at: https://www.freecodecamp.org/news/how-to-write-better-git-commit-messages/.


# Q2
Quality aspects ensure the quality of a software, how functional and well-structured the application is. Every software should aim to incorporate the quality aspects in order to deliver a better user experience. Softwares can be measured based on a group of aspects or on a singular aspect. 

Some of the most important aspects are listed bellow with a brief description on each of them:

#### Usability
User usability is a very important aspect, as it determines the overall software success. Softwares should be easy to navigate, preferably it should not require much training and it should require the minimum amount of clicks to perform a task. 

Another very important aspect is that softwares should consider and accommodate users with different disabilities. Ways to ensure this aspect is successful is collecting user stories, having an user product owner in place and ensuring designs are visually appealing and engaging without overwhelming the users.

#### Functionality
Software functionality is another very important aspect as the software should be able to perform the intended functions and offer the users all the functions needed to perform a specific task. Software developers are responsible for the software functionalities.

#### Code Quality
Software codes should be written in an efficient way, without bugs and semantically correct. Developers should follow the best practices and adherence to standards to ensure high quality code.

#### Reliability 
Software should be able to handle errors gracefully without crashing or losing data. It must perform all tasks given different conditions. Mean Time Between Failure and Mean Time To Repair measurements can be used to check reliability aspect.

#### Maintainability
Developers should prioritise code maintainability to adapt to evolving user needs, as software must keep pace. The codebase should be structured for easy updates, allowing developers to implement changes, fix bugs, and add new features. 

#### Integrity
Integrity aspect shows how easy the software can integrate with the dependant softwares in order to increase functionality.

#### Security
Security is also on the top of the list, users must have their data protected when using the software. Software security ensures software is protected against cyber crimes, and have methods in place to protect users in case of cyber attacks. 

Measurements such as authentication and authentication can greatly reduce the risk of cyber crimes. Another important practise is to regularly implement security checks to ensure software is often protected. Regular checks also can prevent a future security breach.

#### Testability
This indicates how easy the software allows testers to perform testing on the software, how long does it takes to write a testing for the specific software, and how much time it needs to run the testing. One way to reduce costs here is for developers to perform unit and integration testing during the development stage before testers comes into place.  

### Photo example of software quality aspects
![Photo example of software quality aspects from the website codoid](./q2%20copy.png)

References:

Codoid (2019). The Basics of Software Quality Attributes. [online] Codoid. Available at: https://codoid.com/software-testing/the-basics-of-software-quality-attributes/.

Butinar, M. (2023). Don’t Save on Quality: Essential Attributes of Good Software. [online] Available at: https://biosistemika.com/blog/dont-save-on-quality-key-attributes-of-software/.

‌VM. (2023). 15 Key Factors for High-Quality Software. [online] Available at: https://vmsoftwarehouse.com/15-key-factors-for-high-quality-software.

‌
# Q3 
<b>MERN</b> is a pre-built stack web development application based on JavaScript which includes MongoDB, Express.js, React.js, and Node.js technologies. Apart from this variation, there are plenty more of other variations of the *MEAN Stack*. 

The MERN structure follows the MVC (Model-View-Controller) pattern, separating the backend from the frontend, which ensures a clear division of responsibilities and enables independent development. This separation allows developers to work on different parts of the project without interference, enhancing scalability. Testing can also be done separately, allowing bugs to be identified and resolved more efficiently. It's important to mention that all technologies in MERN stores data in the same format.

Frontend developers will be more focused on user's interface, while Backend developers will handle the server logic side, data processing and storage. The skill set needed for the backend includes MongoDB, Express.js, and Node.js, while frontend developers will work with React.js, along with additional technologies like HTML, CSS, and programming languages such as Python and JavaScript. 

MERN is divided into a three-tier architecture (Frontend, Backend, and Database) and it enables the creation of a full-stack application using JavaScript and JSON.

### Components
<b>M - MongoDB (document database)</b>: Mongo is a database which is very compatible with Express.js and Node.js. The database is responsible for storing any data such as user's profiles, product related data, and performing CRUD operations. MongoDB Node.js driver is used to connect DB to Node.js. Another important feature is that, Mongo DB stores data in JSON format.

The process first starts when React.js captures the data from the client server and sends it over to Express.js, where it will be processed and later on, it will be stored in Mongo database. I have attached a photo of the process bellow for more detailed explanation.

<b>E - Express.js (Node.js web framework)</b>: Express is a JavaScrypt frameworks that runs inside Node.js server. It's responsible for handing HTTP requests such as GET, POST, PUT or DELETE and response body.

<b>R - React.js (a client-side JavaScript framework)</b>: React is the top tier, it's the JavaScript framework which allows the creation of dynamic and interactive interfaces in the client-side. React is responsible for creating and linking interactive elements to the server side and rendering these elements using HTML. 

<b>N - Node.js (the premier JavaScript web server)</b>: Node is a JavaScript open source environment. Node runs on the V8 JS engine and it allows developers to write code on the server side. V8 compiles JS code and turn it into machine code. 
Some important features of Node.js:

- Capable of handling enquires made by other programming languages including Python, PHP and Ruby.
- Node is built on a single threaded architecture, it uses event loop and event queue to manage all incoming requests. This method is also known as Non-blocking I/O model.
- It uses asynchronous coding, which can be implemented by callback functions, promises and async/await syntax.
- Modular structure, different functionalities are organised into different modules.
- Uses NPM- Node Package Manager which allows developers to make use of open source packages speeding the development process.

#### Photo of MERN three-tiers structure from mongodb website
![Example of the MERN structure from mongodb website](https://images.contentstack.io/v3/assets/blt7151619cb9560896/blt4b651817f6dec60f/666848e371203e8537986b38/mern-stack.png)


#### Photo example of how 'PUT' http request looks like in MERN stack
![Example of PUT HTTP request in MERN](https://images.contentstack.io/v3/assets/blt7151619cb9560896/bltdf6ce2d4c4ce0204/66684a2f04c62927f26f013d/mern-stack-example.svg)


References:

MongoDB (n.d.). MERN Stack Explained. [online] MongoDB. Available at: https://www.mongodb.com/resources/languages/mern-stack.

W3Schools (2019). Node.js Introduction. [online] W3schools.com. Available at: https://www.w3schools.com/nodejs/nodejs_intro.asp.


Amankwah, K. (2023). MERN Stack Project Structure: Best Practices. [online] DEV Community. Available at: https://dev.to/kingsley/mern-stack-project-structure-best-practices-2adk.

‌
# Q4	
#### Front end and Back end
Web developers are divided in two groups: Front and back end. Frontend developers will be working with everything that is displayed on the browser itself and the Backend developer will work with logic and technical side of the website(this includes APIS and DB). Together, they write the codes that *creates* the website allowing it to be displayed on a browser. Some of the most important skills and knowledge they need in order to create a website includes:

- HTML: to define the website structure.
- CSS: to style the website.
- Javascript: to create the interactive content for the website.
- Server-side languages: Python, Nodejs to manage data, and create integration.
- Version control system: GIT, to track code changes and allow collaborations between developers.
- Flask: Python's micro web frame used to create API.
- PostgreSQL: to manage, store and retrieve data.
- SQLAlchemy: ORM to connect DB to API.

### Design 
UX/ UI designers to ensure positive user's experience while navigating the website. User Interface (UI) designers ensure the elements that users interact directly on the website such as menus and buttons are easy to navigate, clear and visually appealing. User Experience (UX) designers ensure the overall flow on the website is enjoyable and functional. Web designer is also required to create the designs on the website and represent the 'brand' online. 

### Testing
QA engineers are responsible for testing the application and ensuring the application is free of bugs and errors. They ensure website works as it's supposed to and the application quality has passed the requirements. QA are also responsible for creating reports about the website's usability to ensure better user's experience.

### Management
A product manager who will overview the website project is also required. This person will be responsible for coordinating the team, assigning tasks accordingly with each person's set of skills, set goals and deadlines for the team and assist them through the process. 

Project managers should have familiarity with project management tools such as Trello, Jira and Agile/ Scrum expertise. Apart from this, having familiarity with the other aspects of the project including development stages, testing stages would be highly beneficial.


References:

Workbook assignment: JessicaVaz_T2A1-A

Rightpeoplegroup.com. (2024). How to build the ideal website development team structure. [online] Available at: https://rightpeoplegroup.com/blog/how-to-build-the-ideal-website-development-team-structure.


# Q5	

### Marathon running term 2 project
Brief description of my project:

The Marathon Running API is designed to bring runners together. It has functionality for runners to log their workouts and keep track of workout sessions. In the workout log feature, users are allowed to choose from one of the available run types. Date and distance in kilometers are also required to ensure the log keeps all the crucial information for users to track their best sessions. However, the main functionality of my API is to allow users to be part of running groups.
Runnings groups will be later added to marathon events created by groups administrators.

### Tracking project phrase
For tracking the project I have created for the term 2, I have used GitHub and Trello for app tracking. When using the GitHub, understanding how git branches works, how to create pull requests and merge branches were essential step to keep my code modular as I was able separate my code and work on different branches simultaneously without interfering with other part of the program.

Trello management tool was also important, as it gave me acknowledgment of what tasks had be prioritized, what tasks had been finished, what features were ready for testing and what branches were ready for merging. Being able to create tasks, add labels, times and reminders on Trello helped to keep track of my progress through the whole process.

### Development phrase
My initial task was to create an ER diagram, and to help with this task I have used draw.io which is a diagram and flowchart software. For this task, I had to understand how ER diagrams work, how entities are connected, the type of relationship between entities can have between them. In draw.io, I had to understand what formats to use, and what type of arrows to use to demonstrate the right type of relationship connecting the entities. 

When starting the API project, it was crucial to understand how I could create a Virtual Environment to isolate my project, and download required packages to build the project. A understanding of Python PIP package would be necessary, as it was needed when installing dependencies.

My project was built using Python programming language and Flask (Python's micro framework), along with PostgreSQL database. The database was used to store, manage and retrieve the users, running groups and marathons information. SQLAlchemy dependency was used to allow integration with the database and convert Python objects into database tables (users, groups, marathons, workouts tables). It also allows SQL queries to be performed using Python language. 

When dealing with the database, I needed knowledge about data integrity, constraints, primary keys and foreign keys, schemas and data definition language (DDL). Marshmallow dependency was also used to help reading data to and from the database. The format used was JSON, which works in name- value pairs like dictionary. Flask extensions were used in the project when dealing with authentication and authorization. 

Another important field, I required knowledge about was the API endpoints, the different types of requests: GET, POST, DELETE, PUT AND PATCH and the required/ responses bodies. For testing purposes, I have used the Insomnia software which I had to put all the API knowledge into work. 

I have tested the features against different types of inputs, trying to catch errors gracefully and sending back an informative message with the help of SqlAlchemy. I have implemented built-in validation on main inputs including name, email and password using Marshmallow.validate extension. Authorization and authentication features were also tested in Insomnia using JWT. 


### Full Tech stack for the project:

- Virtual environment: it's used to isolate the project to not interfere with other projects. This is the first step when we start on the API project .After activating the Venv, we can start getting all the necessary dependencies to build the API project.

- Python: Programming language used to build the application and manage the dependencies. This is considered the 'base' of the project.

- Python-dot-env: This package is used to help setting up the environment variables that are used to keep sensitive data such as username, password secure. In our project, the environment variables holds the information from database URL and JWT secret key. This file is excluded from the git, but in order for our project to work we need a way to tell other developers or testers they have to set up the environment variables on their end.

- Flask: it's a lightweight yet powerful Python based framework that depends on Werkzeug (WSGI library), Jinja (for rendering the pages on server) and Click (for Flask commands lines and custom commands). All dependencies are installed automatically when you instal Flask.

- PostgreSQL: It's an open-source relational database management system. It's consist of tables (it stores the data into rows and columns), schemas (it organise and manages DB objects). Additionally, it's a very versatile system that supports a wide range of data types and integrates with different programming languages.

- Psycopg2: It works as the driver that connects the API to the DB. It allows your Python applications to connect to and interact with a PostgreSQL database.

- SQLalchemy: It's an Object-Relational Mapping (ORM), that converts Python objects(classes) into database tables. It also allows SQL queries using Python language.

- Marshmallow: It helps flask to read data from/ to the database. It's a Python library used for serialisation and deserialisation of data.
    - Serialise (convert Python objects into JSON).
    - Deserialise (convert input data into Python objects).

- Marshmallow_sqlalchemy: Extension that facilitates integration between marshmallow and sqlalchemy, it generates schemas based on sqlalchemy models that is used for data serialization/deserialization.

- Sqlalchemy.exc: It handles exception errors that might arise when dealing with database operations. It includes: data integrity errors, data errors.

- Marshmallow.exceptions: Used to handle validations errors when serializing and deserializing data.

- Flask_bcrypt: Used for handling sensitive data and password encryption.

- Flask_jwt_extended: Flask extension used for authentication methods by creating tokens.

- JWTManager: It helps in the process of token decoding and verification.

- Functools: It's used when creating decorators, it allows a function to take another function as a parameter by using the wraps method.

- OS: It's part of Python standard library, it's used to fetch environment variables from .env file and import into main.py file. It connects with the operating system.

- Datetime: Used to display time in attributes that requires time information.

- Marshmallow.validate: Built-in validators that can be used to enforce data validation. These validations are placed in the schemas. It can be used on name, email, password, one of (it's used to ensure that a field's value is one of a specified set of acceptable choices).


References: 

Project assignment: JessicaVaz_T2A2


# Q6	

### Tracking project phrase
How effective my skills and knowledge were?

When using GIT, I feel my set of skills and knowledge were enough to perform all tasks during the whole project duration. Git has been introduced in our web development course in the first stage, and it has been very present in all of our projects, because of this, I am confident my skills related to GIT are sufficient.

With Trello, I also believe my skills and knowledge were sufficient since we have been introduced to Trello in the first term. 

Examples:
- For Marathon running application, I have created different branches for each feature and I worked on them independently. This was extremely beneficial since, I could improve and scale my project without interfering with other parts of the code.
- In Trello, I was able to create a project tracking system with labels to tell me how urgent the task were, ensuring I was prioritizing the important tasks first. 

Improvements suggested:
- Adding the type of commit on the commit messages to make it more clear and organised.
- Adhere to a git commit style such as conventional style.
- Ensure to added only relevant information on Trello board to keep it simple and descriptive.
- Ensure to use labels, checklists and due-time whenever applicable in Trello


### Development phrase
How effective my knowledge and skills were?

During the development phrase, I believe my skills were enough. Initially, I had to change my project idea as I didn't think I could go ahead with the original idea which as a fitness tracker. I had struggle with the ER Diagram, understanding how the relationship between the entities worked, and how that impacted when writing my application. I came across many errors in my ER Diagram, which my tutor Aamod has helped me greatly to resolve and improve my idea. 

I believe that my knowledge in ER Diagram and relationship types improved significantly after completing this project as I had to create and make several changes until the ER Diagram would reflect what I had in my for my project. 

When it came the time to start the project, my skills and knowledge gained through ZOOM classes and ED content came in handy, I don't think I have struggled when creating VENV and getting all the necessary dependencies. Connecting my API to DB was also a smooth sail. 

To create my API, I have used Python programming language, and my skills and knowledge were ok but I wish I had more knowledge to not struggle a lot, and also to be able to scale my project further. 

With the database integration, I wish my skills and knowledge were more profound as I was stuck in this phrase more time than what I should. I run across numerous errors when dealing with the database. I believe having a deeper understanding of ORM, schemas, Primary and Foreign keys, back populating would be extremely beneficial for my next project.

Examples:
- I ran into a lot of issues when turning my ER diagram into actual code for the database. One big problem was that when I tried to fetch information from the database, I couldn’t get the right data because the relationships weren’t set up correctly. I had to go back and adjust how things were connected to make sure the database worked the way I planned in the diagram.
- Initially, I also used the wrong arrows to represent one-to-one, one-to-many, and many-to-many relationships in my ER diagram.

Improvements suggested:
- More profound studies on Python programming language, ORM (Object Relational Mapping) and Database Models and Schemas.
- Ensure ER Diagram is 100% correct before starting the project to not cause confusion.


### Testing phrase
How effective my knowledge and skills were?

My testing skills and knowledge improved as I have performed them. As I performed the testing, I could see the potential areas which might cause errors and handle them gracefully. Working with Insomnia was easy and enjoyable as it was a powerful tool for me to improve my application. 

I used Marshmallow to handle validation errors and SQLAlchemy for exception handling. The knowledge I gained from the Zoom classes was sufficient, but now that I feel more confident, I plan to explore additional types of errors and error-handling techniques for future projects.

Having a good understanding of HTTP request methods was very crucial for the testing phrase as well. Again, the zoom classes, especially when we create the API together and tested using Insomnia gave me a great insight of the different HTTP request methods, body of request and response.

Examples:
- I have applied validation on main user's input to ensure correct data type.
- I have created different folders in Insomnia for each model in my API to testing against different HTTP request methods to ensure organisation.
- Being able to understand what to expect when using each HTTP request method (GET, POST, PUT, DELETE, PATCH) allowed me to design the API more effectively. It helped me structure each endpoint properly, ensuring that the correct data was sent and received with each type of request, and made error handling more straightforward. 

Improvement suggested:
- Explore other testing softwares such as Postman.
- Explore different errors types and how to handle them gracefully.
- Ensure future projects has more validations in place.
- Implement sanitization for my future projects.

References: 

Project assignment: JessicaVaz_T2A2


# Q7	
<b>Control Flow</b> plays a crucial part in a program because it dictates the order in which the program executes the code. In another words, it dictates the program's flow. The default way the computer reads the code is top to bottom, line by line, until it comes across statements which can redirect the flow. All the examples given in the question will be in JavaScript. 

Some of the most common statements that can change the flow includes: 

### If/Else statements
Conditional statements that execute specific code blocks based on whether one or more conditions evaluate to true. If a condition is true, the code within the 'if' block runs; otherwise, it is skipped. The 'else' block contains code that executes only if all previous conditions are false. In JavaScript, to chain multiple IF's, 'else if' are used.

The syntax for IF/ ELSE statements is describe bellow:
    
    if (condition) {
    // Code to execute if the condition is true
    } else if (anotherCondition) {
    // Code to execute if the first condition is false and this condition is true
    } else {
    // Code to execute if all previous conditions are false
    }

Example:

    if ( number === 5 ) {
        console.log( "Five." );
    } else if ( number === 3 ) {
        console.log( "Three" );
    } else {
        console.log( "Neither five nor three." );
    }

### Ternary operator
The ternary operator is a conditional operator, it's more compact than If/ Else statements. Ternary operator uses 3 operands: the condition to be evaluated, the expression that will be executed if the condition evaluates to true, and the expression to be executed if the condition evaluates to false. 

Syntax:

    Condition ? expression1 : expression2

Example:

    let age = 20;

    let driving_age = age >= 18 ? "You can get behind the wheel!!" : "You are too young kid...";

    console.log(driving_age); // output: "You can get behind the wheel"

### Switch... case statements
Switch case is another type of conditional statement. It works by comparing by comparing an expression's value against different potential 'cases'. Each case contains a statement that will be executed if the case matches the expression's value. Encapsulated statements inside of the correct case also will be executed. 

Once the match case is found, it's important to call 'break' keyword to exit the evaluation, since JS will execute any statements placed after the matched-case, this process is called *falling through*.
Default case comes into action when none of the previous cases were the right value, default works similarly to 'else' in If/else statements. It's important to also note that variables declared inside each case can be accessed by the other cases within the same switch statement. One way to ensure case scope is maintained is to use block statement {}. 

Example:

switch ( 2 + 2 === 5 ) {
    case false:
    console.log( "False." );
    break;
  case true:
    console.log( "True." );
    break;
} // "False."


### Loops
The program's flow can be interrupt when it reaches a loop. Loops executes a block of codes on repeat until a condition is met. JavaScript has few different types of loops.

#### While loop
A while loop is used to run interactions until a specific condition is met or until the loop has reached the end of the iterable data structure. A while loop runs repeatedly, evaluating the condition at the start of every iteration. If the condition is truthy, the body statements are executed, then the condition is evaluated again, and if the condition evaluates to falsy, the loops never runs. A common use case for a while loop is when the loop length is indeterminate, however it can be used with a specified number of times as the example bellow demonstrate.

Syntax :

    while (condition to be evaluated) {
    loop body
    }

Example:

    let iterationCount = 0;
    while( iterationCount < 3 ) {
    iterationCount++;
    console.log( `Loop ${ iterationCount }.` );
    }
    > "Loop 1."
    > "Loop 2."
    > "Loop 3."

#### Do...while loop
A do..while loop is very similar to the while loop. The difference is that the body precedes the condition and the loop runs at least one iteration - even if the condition is falsy in the first iteration. In the do...while loop, the evaluation actually happens at the end of iteration, that's the reason why the loop always runs at least once. This loop is useful for testing user input against specific conditions. A common use case for a do...while loop is when the loop length is indeterminate.

Syntax:

    do {
    body;
    } while (condition);

### Loops

#### For loop
A for loop is typically used to execute statements a specific number of times when the number of iterations is known in advance. For loops are made of 3 expressions: initialise , condition, and update. 
The first expression initializes the loop, the second expression contains the condition and the third expression contains an expression to be executed once the loop has been completed. A for loop runs while the condition expression is truthy, when it becomes falsy, the loops end. 

Syntax:

    for (initialise; condition; update) {
    // loop body
    }

Example:

    for( let i = 0; i < 5; i++ ) {
    console.log( "This loop will run five times.")
    }

When initialising the variable, it's a common practice to use 'let' to declare the variable, and use 'i' to identify the variable. Since indexes start at 0, this will be reflected when declaring a FOR loop. The third expression is used to increment the identifier by one.

#### For...in loop
The for...in loop is a type of loop that allows you to iterate over the properties of an object. The for...in loop works by assigning each property of the object to a variable, one by one, and executing a block of code for each property.

Syntax:

    for (let variable in object) {
    // code to be executed
    }

Example:

    const carDetails = { "make": "Toyota", "model": "Corolla", "year": 2022 };

    for (const detail in carDetails) {
        console.log(detail); // This will print each key in the object
    };
    > "make"
    > "model"
    > "year"

How to fetch properties value using the key:

    const carDetails = { "make": "Toyota", "model": "Corolla", "year": 2022 };

    for (const detail in carDetails) {
        console.log(`${detail}: ${carDetails[detail]}`);
    }

#### For...of loop
The for...of loop can be used to work with iterables, for example: array, set and map. In the general case, for...of loop iterates over the elements of an iterable and runs the same statements for every element. The variable used in for...of loop can be a variable declared within the loop, or declared within the same scope.

Syntax:

    for (let item of iterable) {
    // code to be executed
    }

Example:

    const myIterable = [ apple, orange, berries ];
    for (const fruit of myIterable) {
    console.log(fruit);
    }
    > apple
    > orange
    > berries

#### When to use For and While loops
- Use a while loop when you want to execute a block of code repeatedly as long as a certain condition is true.
- Use a do...while loop when you want to execute a block of code at least once, and then repeatedly as long as a certain condition is true.
- Use a for loop when you know the number of times you want to execute a block of code.
- Use a for...in loop when you want to iterate over the properties of an object.
- Use a for...of loop when you want to iterate over the elements of an iterable object such as an array or a string.

### Statements
- Return statement: It is used within a function, when the return statement happens, the functions stops and sends the value back to the function's caller. If return is not specified, JavaScript implicitly returns undefined.
- Break statement: It's used to completely exit the current loop or switch interaction.
- Continue statement: It is used to stop the current iteration, and skip to the next iteration if the condition still true. Commonly used in JavaScript loops to skip current value instead of exiting the loop completely.

Example:

    let iterationCount = 0;
    while( iterationCount <= 5 ) {
    iterationCount++;
    if( iterationCount === 3 ) {
        continue;
    }
    console.log( `Loop ${ iterationCount }.` );
    }
    console.log( "Loop ended." );
    > "Loop 1."
    > "Loop 2."
    > "Loop 4."
    > "Loop 5."
    > "Loop ended."

### Try...catch blocks

- Try block: This block contains code that might throw an error. If no error occurs, the code runs as usual.
- Catch block: If an error occurs in the try block, JavaScript immediately jumps to the catch block, skipping any remaining code in the try block. The catch block handles the error.
- Finally block: It always executes regardless if an error was caught or not.

Example:

    try {
    let result = riskyOperation();
    console.log("Operation succeeded:", result);
    } catch (error) {
    console.log("An error occurred:", error.message);
    } finally {
    console.log("This will run no matter what.");
    }

References:

developer.mozilla.org. (n.d.). Control flow - MDN Web Docs Glossary: Definitions of Web-related terms | MDN. [online] Available at: https://developer.mozilla.org/en-US/docs/Glossary/Control_flow.

web.dev. (n.d.). Control flow. [online] Available at: https://web.dev/learn/javascript/control-flow.

‌
‌

# Q8	
Explain type coercion, using examples from the JavaScript programming language

# Q9	
Explain data types, using examples from the JavaScript programming language

# Q10	
Explain how arrays can be manipulated in JavaScript, using examples from the JavaScript programming language

# Q11	
Explain how objects can be manipulated in JavaScript, using examples from the JavaScript programming language

# Q12	
Explain how JSON can be manipulated in JavaScript, using examples from the JavaScript programming language