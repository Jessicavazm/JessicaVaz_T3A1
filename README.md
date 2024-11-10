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


<b>References:</b>

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

<b>References:</b>

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


:

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


<b>References:</b>

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


<b>References:</b>

Project assignment: JessicaVaz_T2A2


# Q6	

### Tracking project phrase
How effective my skills and knowledge were?

When using GIT, I feel my set of skills and knowledge were enough to perform all tasks during the whole project duration. Git has been introduced in our web development course in the first stage, and it has been very present in all of our projects, because of this, I am confident my skills related to GitHub are sufficient.

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

Furthermore, I believe that my knowledge in ER Diagram and relationship types improved significantly after completing this project as I had to create and make several changes until the ER Diagram would reflect what I had in my for my project. 

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

<b></b>:

Project assignment: JessicaVaz_T2A2


# Q7	
<b>Control Flow</b> plays a crucial part in a program because it dictates the order in which the program executes the code. In another words, it dictates the program's flow. The default way the computer reads the code is top to bottom, line by line, until it comes across statements which can redirect the flow. All the examples given in the question will be in JavaScript. 

Some of the most common statements that can change the flow includes: 

### If/Else statements
Conditional statements that execute specific code blocks based on whether one or more conditions evaluate to true. If a condition is true, the code within the 'if' block runs; otherwise, it is skipped. The 'else' block contains code that executes only if all previous conditions are false. In JavaScript, to chain multiple IF's, 'else if' are used.

The syntax for IF/ ELSE statements is described bellow:
    
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
Switch case is another type of conditional statement. It works by comparing an expression's value against different potential 'cases'. Each case contains a statement that will be executed if the case matches the expression's value. Encapsulated statements inside the correct case also will be executed. 

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
The program's flow can be interrupted when it reaches a loop. Loops execute a block of codes on repeat until a condition is met. JavaScript has few different types of loops.

### While loop
A while loop is used to run interactions until a specific condition is met or until the loop has reached the end of the iterable data structure. A while loop runs repeatedly, evaluating the condition at the start of every iteration. If the condition is truthy, the body statements are executed, then the condition is evaluated again, and if the condition evaluates to Falsy, the loop never runs. A common use case for a while loop is when the loop length is indeterminate, however it can be used with a specified number of times as the example bellow demonstrate.

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

### Do...while loop
A do..while loop is very similar to the while loop. The difference is that the body precedes the condition and the loop runs at least one iteration - even if the condition is Falsy in the first iteration. In the do...while loop, the evaluation actually happens at the end of iteration, that's the reason why the loop always runs at least once. This loop is useful for testing user input against specific conditions. A common use case for a do...while loop is when the loop length is indeterminate.

Syntax:

    do {
    body;
    } while (condition);


### For loop
A for loop is typically used to execute statements a specific number of times when the number of iterations is known in advance. For loops are made of 3 expressions: initialise, condition, and update. 
The first expression initialises the loop, the second expression contains the condition and the third expression contains an expression to be executed once the loop has been completed. A for loop runs while the condition expression is truthy, when it becomes Falsy, the loop ends. 

Syntax:

    for (initialise; condition; update) {
    // loop body
    }

Example:

    for( let i = 0; i < 5; i++ ) {
    console.log( "This loop will run five times.")
    }

When initialising the variable, it's a common practice to use 'let' to declare the variable, and use 'i' to identify the variable. Since indexes start at 0, this will be reflected when declaring a FOR loop. The third expression is used to increment the identifier by one.

### For...in loop
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

### For...of loop
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
- Continue statement: It is used to stop the current iteration, and skip to the next iteration if the condition still true. Continue statement is commonly used in JavaScript loops to skip current value instead of exiting the loop completely.

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

<b>References:</b>

developer.mozilla.org. (n.d.). Control flow - MDN Web Docs Glossary: Definitions of Web-related terms | MDN. [online] Available at: https://developer.mozilla.org/en-US/docs/Glossary/Control_flow.

web.dev. (n.d.). Control flow. [online] Available at: https://web.dev/learn/javascript/control-flow.


# Q8	
JavaScript is considered a *weakly typed language*, also called dynamically typed, which means it's more flexible when it comes to data type checks. Operations in JS can be performed without a strict data type check, in case of an expression being evaluated with two different types, JS will try to coerce both types into the same type in order to perform the evaluation. 

This process is called <b>Type coercion</b> in JavaScript. This is one of the main difference between JavaScript and Python programming languages. Python on the other hand is considered a *strong typed language*, this means Python won't allow operations to be performed on different data types without an implicit declaration beforehand. If we tried to perform that operation in Python, we would end up with an error.

There are two types of coercion in JS, the <b>implicit type</b> which JavaScript automatically converts the data type in order to make the expression work, and the <b>explicit type</b> when the user converts the type manually. Type coercion is applicable in all data types (primitive types or objects), when this process happens in objects, JS will try to convert the object into a primitive type using toString() or valueOf() methods. It's important to remember that if none of those methods are called, JS will convert to its default method: String. 

Another important aspect about data type coercion is that JavaScript only has three different types of coercion: 
- to string
- to boolean
- to number 

It's important to mention that the strict equality operator does not trigger an implicit coercion. When using the <b>strict operator (===)</b>, the expression will check both data type and value in order to evaluate the operation, while the <b>loose operator (==)</b> only checks the value itself. 


### Example of explicit type coercion in primitive types:
String coercion:
    
    String(123) // explicit
    123 + ''    // implicit way is triggered by the binary + operator

Symbol coercion: It can only be converted by explicitly declaration
    
    String(Symbol('my symbol'))   // 'Symbol(my symbol)'

    console.log(Symbol("id") + ""); // TypeError: Cannot convert a Symbol value to a string


Boolean conversion: It can be performed applying the Boolean () function. Double negation !! is a quicker way to convert data type into Boolean value.

    let num = 0;
    let isZero = Boolean(num);  // false, because 0 is a "falsy" value

    let value = "JavaScript";
    let isTruthy = !!value;  // true, because JS is a non empty string

    List of falsy values: 
    - Empty string '' 
    - 0     
    - -0
    - NaN - Not a number
    - Null
    - Undefined
    - False

Numeric conversion: It can be performed by using Number() function.
    
    Number('123')   // 123


### Example of implicit type coercion in primitive types:
String and Number: JS typically converts number into string.

    let result = "5" + 1;  // "51" (number 1 is coerced to a string)
    let sum = "5" - 1;     // 4 (string "5" is coerced to a number)

    let a = 10;
    let b = "20";
    let result = a + b;  // "1020" (a number is coerced to a string for concatenation)

Boolean: When a non-boolean value is used in a comparison or logical context, JS coerces the non-boolean value to boolean. This type of coercion is often triggered by logical operators (OR, AND, NOT || && !).

    if ("hello") {  // "hello" is a non-empty string, so it is coerced to true
      console.log("This runs");
    }

Coercion with Template Literals ${} : JS automatically convert values into string.

    let name = "Jessica";
    let age = 31;
    console.log(`Name: ${name}, Age: ${age}`);  // "Name: Jessica, Age: 31"


### Example of type coercion in Objects 
In the example bellow, the expressions are calling the valueOf() and toString() methods to convert data type into primitive type. 

The valueOf () function is used when the value expected is a numeric data type and toString() when the expected value is string data type.

    let obj = { valueOf: () => 42 };
    let result = obj + 10;  // Result will be 52, since valueOf() is called

    let obj = { toString: () => "Hello" };
    let result = "Message: " + obj;  // Result will be "Message: Hello"
    
Example of a default coercion in obj:

    let obj = {};
    let result = obj + "";  // "[object Object]" (default string representation)


### Example of implicit type coercion in Special Objects(built-in objects):
Arrays: JS will coerce array elements into a string using the toString() method.

    let arr = [1, 2, 3];
    let result = arr + "";  // "1,2,3" (array is coerced to a string)

Dates: JS will coerce date object into a string, usually in a date format.
    
    let date = new Date();
    let result = date + "";  // "Fri Nov 09 2024 12:34:56 GMT-0500 (Eastern Standard Time)"

Function Object: JS returns the string representation of the function's source code.
    
    function greet() {
        return "Hello";
    }
    console.log(greet + "");  // "function greet() { return 'Hello'; }"

### Custom coercion 
RegExp coercion: JS first call the toString() method to coerce regular expression into string.
    
    let regex = /abc/;
    console.log(regex.toString());  // "/abc/"

Map and Set objects: JS doesn't convert map and set objects automatically into a string, the method JSON.stringify() needs to be call first in order to perform the coercion.

    let set = new Set([1, 2, 3]);
    console.log(JSON.stringify([...set]));  // Outputs "[1,2,3]"


<b>References:</b>

Samoshkin, A. (2018). JavaScript type coercion explained. [online] freeCodeCamp.org. Available at: https://www.freecodecamp.org/news/js-type-coercion-explained-27ba3d9a2839/.

GeeksforGeeks (2020). What is Type Coercion in JavaScript ? [online] GeeksforGeeks. Available at: https://www.geeksforgeeks.org/what-is-type-coercion-in-javascript/.

‌
# Q9	
In JavaScript, data types are divided in two main groups: the primitive types and the object types. Another important feature of JS is 

### Primitive data types
Primitive data types are the 'simple' type, they are stored directly at the base of the program and their values are immutable. All the primitive data types can be tested using typeOf operator, apart from the 'Null' type. If we try to use typeOf on 'Null', we will get 'object' instead. One way around this is to use the strict equality operator when checking if a variable is a Null type. 

Most primitive data types has 'object wrappers' which works as mini helpers that allows methods to be applied directly in the variables. In the example bellow, toExponential() method is called on the variable num to format the number 42 into an exponential notation.

    let num = 42;
    console.log(num.toExponential()); // "4.2e+1"

Wrappers are not available in Null and Undefined type, trying to use object wrappers on those methods will result in a TypeError exception.


### Primitive data types

### String
Represents a collection of characters
- One of the most common data type.
- It can be created with single '' or double quotes "".
- Backticks `` allows string interpolation.
- Use concat() or + to concatenate two strings.
- Most common methods for string:
    - length - Returns the number of characters in a string.
    - toUpperCase() and toLowerCase() - Convert strings to uppercase or lowercase.
    - indexOf() - Finds the first occurrence of a substring. Returns -1 if not found.
    - includes() - Checks if a substring exists within the string. Returns true or false.
    - slice() – Extracts a section of a string and returns it as a new string.
    - replace() – Replaces a specified value with another in a string (only the first match).
    - split() – Splits a string into an array based on a specified separator.

String declaration and string interpolation:

    let name = "Jessica";
    let age = 31;
    let greeting = `Hello, my name is ${name} and I'm ${age} years old.`;
    console.log(greeting); // "Hello, my name is Jessica and I'm 31 years old."

Using replace() method:

    let phrase = "Hello, world!";
    console.log(phrase.replace("world", "Jessica")); // "Hello, Jessica!"

Using toUpperCase() && toLowerCase():

    console.log("hello".toUpperCase()); // "HELLO"
    console.log("WORLD".toLowerCase()); // "world"

### Number 
Represents numbers both integers and float
- JavaScript numbers are stored as 64-bit floating-point values.
- JS can store numbers from -2^53 to 2^53 in this data type, numbers larger than 2^53 are stored in BigInt instead.
- NaN Not a Number: this is also part of the number data type, it's used for arithmetics operations when it encounters a result that can not be processed as a number.
- Infinity and -Infinity: Represents values beyond the minimum and the maximum limits. (Dividing a positive number by 0 in JS, would return 'infinity').
- Common methods to work with numbers in JS includes: 
    - Number.isInteger() => checks if the numbers is integer
    - Number.isIntegerNaN() => checks if the numbers is Not a Number
    - toBeFixed() => it rounds a number to a specified number of decimals places and it returns a string
    - parseInt() and parseFloat() => Convert strings to integers and floating-point numbers

Example in JS codes:

Converting string into number, and floating-point numbers:

    console.log(parseInt("42")); // 42
    console.log(parseFloat("3.14")); // 3.14

Using toFixed () method:

    let num = 3.14159;
    console.log(num.toFixed(2)); // "3.14"

Using isInteger() method:

    console.log(Number.isInteger(42)); // true


### BigInt 
Represents very large numbers
- Useful for numbers larger than 2^53
- It works by adding the letter n by the end of the Number.

Declaring an bigInt variable:

    let big = 123456789012345678901234567890n;

### Boolean 
Represents logical values True || False
- Used to control the flow of the program.
- It's commonly used in conditional and comparison operations.
- To create a Boolean variable, you need to assign either True or False value to the declared variable. 
- Booleans can be used with Logical operators: 
    - AND (&&) - Returns true if both operands are true.
    - OR (||) - Returns true if at least one operand is true.
    - NOT (!) - Inverts the Boolean value.

Example of a Boolean data type:

    let isRaining = true;

    if (isRaining) {
        console.log("Take an umbrella!");
    } else {
        console.log("No need for an umbrella today.");
    }


### Undefined
Represents the absence of a value. Common events when undefined is returned:
- A return statement without a value, by default returns undefined.
- Accessing a object's property that does not exist also returns undefined.
- Declaring a variable without initialising first returns undefined.
- When using searching methods, if no element is found it also returns undefined.

Declaring a variable without initialization:

    let myVariable;
    console.log(myVariable); // Output: undefined

Parameters not given in the greet function:

    function greet(name) {
    console.log("Hello, " + name);
    }
    
    greet(); // Output: Hello, undefined

### Null
Represents 'nothing', absence of an object.
- You need to explicitly assign null to a variable.

### Symbol
Represents a unique, immutable identifier, useful for object keys
- Introduced in ES6 (ECMAScript 2015).
- Often used as an identifier for object's properties.
- Creates uniques keys using symbol() function.
- Able to hide obj properties in searching calls.

Example of declaring a Symbol with the same name:

    let sym1 = Symbol("description");
    let sym2 = Symbol("description");

    console.log(sym1 === sym2); // Output: false


### Non-Primitive data types

### Objects
Collection of key-value pairs, including objects, arrays, and functions.
- The only mutable data type in JS
- Similar to Python Dictionary
- Object keys are interpreted as strings or symbols
- Object values can be values of any type, including other objects
- Dot notation doesn't work on numerical data type keys.
- Wrapped in curly braces and includes key-value pairs, or properties, with property names and values.

### How to declare an object 

    let student = {}
    student["name"] = "Jess"

Create a dictionary and populate it:

    let person = {
        name : "Jess",
        age : 21 
    }

How to get specific values:

    person.age
    person.name

How to change values:

    person.age = 31
    person.name = "Jessica"


### Array
An array is a special kind of object, it's a collection of indexed values. In JS, an array is represented by an ordered sequence of elements separated by commas and wrapped in square brackets. Array is a way to collect multiple pieces of data together in one variable.

Important features of arrays:
- Arrays are dynamic in JS, that means it can smaller in size or bigger.
- First element in the array is 0, second element is 1, and so on.
- Arrays can hold different data types.
- Vast list of methods to manipulate arrays in JS.
- High order functions for processing elements such as map(), filter() and reduce().
- Arrays are iterable using loops.
- JS supports matrix arrays.
- Immutable Array Methods returns a new array instead of modifying the original one.
- JS supports sparse arrays

Example of array declaration:

    let cuteAnimals = ["koala", "wombat", "dog"];

Example of adding an extra element in an array:

    let arr = [1, 2, 3];
    arr.push(4); // Adds 4 at the end
    console.log(arr); // [1, 2, 3, 4]

Example of array with different data types:

    let mixedArray = [42, "hello", { name: "Jessica" }, [1, 2, 3]];

Fetching a specific element in a Matrix array in JS:

    let matrix = [
        [1, 2, 3],
        [4, 5, 6],
        [7, 8, 9]
    ];
    console.log(matrix[1][1]); // 5


### Functions
- First class citizen:
    - Assigned to variables
    - Nested in other objects/ functions
    - Passed as args
    - Returned from other functions
- Functions can be anonymous
- Functions can be called before they are declared
- Functions in JS have properties: name && length
- JS supports Async Functions and Promises
- JS supports IIFE (Immediately Invoked Function Expressions)

How to declare a function:

    function greet(name) {
        return `Hello, ${name}!`;
    }
    console.log(greet("Jessica")); // Output: Hello, Jessica!


How to check functions properties:

    function myFunc(a, b) {}
    console.log(myFunc.name); // "myFunc"
    console.log(myFunc.length); // 2


<b>References:</b>

W3Schools (2020). JavaScript Data Types. [online] W3schools.com. Available at: https://www.w3schools.com/js/js_datatypes.asp.

MDN (2019). JavaScript data types and data structures. [online] MDN Web Docs. Available at: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures.

‌
# Q10	
JavaScript has a rich number of methods available to manipulate <b>arrays</b>. Some of the most common methods will described bellow with JS coding examples to further explain the process.

How to declare an array:
    
    let myArr = ["Jess", 31, "Melbourne"]

Note: myArr variable will be used in the following examples. To not overcrowd the file, I won't keep declaring myArr.

### Concat() method
This method add two arrays together and returns a new array
    
    let myArr2 = ["Australia", 1]

    let merged_arrays = myArr.concat(myArr2);
    console.log(merged_arrays) // ["Jess", 31, "Melbourne", "Australia", 1]

### Push() method
This method adds elements at the end of the array, it does change the original array.
    
    myArr.push("Australia")
    console.log(myArr) // ["Jess", 31, "Melbourne", "Australia"]

### Pop() method 
This method removes the last item in the array and returns it

    myArr.pop(); // "Melbourne"

    console.log(myArr) // ["Jess", 31]

### Shift() method
This method removes the first item in the array and returns it

### Unshift() method 
This method add items to the beginning of the Array, it does change the original array.

    myArr.unshift("Girl")
    console.log(myArr) // ["Girl", "Jess", 31, "Melbourne"]

### Splice() method
This method removes an element from a specified index. The first parameter is the element index position and the second parameter is the delete count(how many elements to be deleted). This methods changes the original array. When second parameter has not been declared, this method will delete every element starting from the given index.

It's possible to add elements with the splice method by passing the number 0 in the second parameter.
The syntax will consist of 3 parameters instead. The first is the element index from where the adding will start, the second parameter is 0, the third parameter are the elements to be added to array.

How to remove elements with splice:

    myArr.splice(0, 1); //  Removes 1 element at index 0
    console.log(myArr) // [31, "Melbourne"]

### Slice() method 
This method returns sub-arrays. This does not change the original array. Assigning the new sub-array to a variable is the best use case for this method.

Syntax:
    
    array.slice(start, end)

### Searching methods
- indexOf() method: Returns the first index of an element, or -1 if not found.
- includes() method: Checks if an element exists in the array.
- find() and findIndex() methods: Search based on a condition.

JS coding examples:

    let numbers = [10, 20, 30, 40];
    console.log(numbers.indexOf(20)); // 1
    console.log(numbers.includes(50)); // false

    let found = numbers.find(num => num > 25);
    console.log(found); // 30

    let index = numbers.findIndex(num => num > 25);
    console.log(index); // 2

### Filter() method
This method returns a new array with the items that has passed the condition.

Syntax:

    let results = array.filter(function(item, index, array) {
    // returns true if the item passes the filter
    });

Example:

    let ages = [18, 22, 16, 25];
    let adults = ages.filter(age => age >= 18);
    console.log(adults); // [18, 22, 25]

### Map() method 
This method creates a new array by applying a function on each element.

Example:

    let numbers = [1, 2, 3, 4];
    let doubled = numbers.map(num => num * 2);
    console.log(doubled); // [2, 4, 6, 8]

### Reduce() method
This method reduces all elements to a single value. It's useful for calculations.

Example:

    let sum = [1, 2, 3, 4].reduce((total, num) => total + num, 0);
    console.log(sum); // 10

### Sort(): 
This method sorts elements in place.

Example:

    let names = ["Jessica", "Aamod", "Zara"];
    names.sort();
    console.log(names); // ["Aamod", "Jessica", "Zara"]

### Reverse() method
This method reverses the order of elements.

Example:

    names.reverse();
    console.log(names); // ["Zara", "Jessica", "Aamod"]

### forEach() 
This method iterates over each element in the array.

    const colors = ['green', 'yellow', 'blue'];
    colors.forEach((item, index) => console.log(index, item));
    // returns the index and the every item in the array
    // 0 "green"
    // 1 "yellow"
    // 2 "blue"

### ...Spread operator
This operator can copy arrays, or combine arrays.

Example:

    let array1 = [1, 2];
    let array2 = [3, 4];
    let combinedArray = [...array1, ...array2];
    console.log(combinedArray); // [1, 2, 3, 4]

<b>References:</b>


#### Personalised functions
Personalised function is another way to manipulate arrays in JS, you can create a function with a specified condition. This type of manipulation can be a bit more specific than the JS built-in methods.

    Example of using a function to manipulate an array:

    const numbers = [10, 45, 3, 7, 29];

    function sortDescending(array) {
        return array.sort((a, b) => b - a);
    }

    const sortedNumbers = sortDescending(numbers);
    console.log(sortedNumbers);
    // Output: [45, 29, 10, 7, 3]


MDN Web Docs. (2019). Array. [online] Available at: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array.

Ayodeji, B. (2019). How to Manipulate Arrays in JavaScript. [online] freeCodeCamp.org. Available at: https://www.freecodecamp.org/news/manipulating-arrays-in-javascript/.


# Q11	
In JavaScript, an object is a collection of <b>key-value pairs</b> that represent the properties of the object. Methods are functions that belong to an object and are used to manipulate its data. In other words, a method is a property of an object that has a function as its value. 

Object methods are often used to create, retrieve, update, and delete data within objects. A property's key can be any string and a property's value can be a string, number, boolean, object, function, null or undefined. Most objects in JS are assigned to a variable which facilitates manipulation, however objects can exist without being named or assigned to a variable. 

Common cases when an object is not directly linked with a variable:

- When an anonymous object is being passed as an argument to a function.
- Directly define and return objects in the return statement.
- Objects can be used directly in expressions, conditions, or configurations without being stored in variables.
- IIFEs: when objects are created inside of a function, the object here is function scoped.


Below, I will describe JavaScript built-in methods along with coding examples for further explanation.

#### How to create an object 
JS objects can be created using obj literals or object constructor. Using object constructor allows many instances to be created through the object "blueprint".

    // Creating a new obj using obj literals:

    let person = {
        name: "Jessica",
        age: 31
    }; 


    // Creating a new obj using obj constructor:

    function Car(make, model) {
    this.make = make;
    this.model = model;

    this.getDetails = function() {
        return `${this.make} ${this.model}`;
    };
    }

    // Creating new instances of the Car object:

    const car1 = new Car("Toyota", "Camry");
    const car2 = new Car("Honda", "Civic");

#### How to access the properties
To access the object's properties both square notation or dot notation can be used. Dot notation is mostly used as it is more clear to read.

    console.log(person.name); // "Jessica" (dot notation)
    console.log(person["age"]); // 29 (bracket notation)

#### How to add properties
To add new properties dot notation can be used on object.

    person.city = "Melbourne";
    console.log(person.city); // "Melbourne"

#### How to update object's properties
To update a property, you need to reassign the value using dot notation.

    person.age = 30;
    console.log(person.age); // 30


#### Deleting properties
To delete a property, the 'delete' method will be used.

    delete person.city;
    console.log(person.city); // undefined

#### Manipulate objects with loops (for...in)
For...in loop can interact over the object's properties.

    for (let key in person) {
        console.log(`${key}: ${person[key]}`);
    }
    // Output:
    // name: Jessica
    // age: 30

#### hasOwnProperty() method
This method check if an object has a specified property.

    console.log("name" in person); // true
    console.log(person.hasOwnProperty("age")); // true

#### Object destructuring() method
JavaScript supports destructuring, allowing properties to be unpacked into individual variables.

    const { name, age } = person;
    console.log(name); // "Jessica"
    console.log(age); // 30

#### Object.assign() and ...Spread operator.
This method merges two objects into a new one and it can also create shallow copies.

    Merging example:

    let address = { city: "Melbourne", country: "Australia" };
    let personWithAddress = { ...person, ...address };
    console.log(personWithAddress);
    // { name: "Jessica", age: 30, city: "Melbourne", country: "Australia" }


    Creating shallow copy example:

    let original = { name: "Jessica" };
    let copy = { ...original };
    copy.name = "Iryna";
    console.log(original.name); // "Jessica" (original is unaffected)


#### Setter and Getter in JS Objects
JS allows setter and getter methods to be used in objects define properties.

    let rectangle = {
        width: 5,
        height: 10,
        get area() {
            return this.width * this.height;
        },
        set dimensions({ width, height }) {
            this.width = width;
            this.height = height;
        }
    };

    console.log(rectangle.area); // 50
    rectangle.dimensions = { width: 7, height: 14 };
    console.log(rectangle.area); // 98

#### Retrieving object's keys, values and entries with methods
- Object.keys() returns an array of keys.
- Object.values() returns an array of values.
- Object.entries() returns an array of key-value pairs.

Examples:

    console.log(Object.keys(person)); // ["name", "age"]
    console.log(Object.values(person)); // ["Jessica", 30]
    console.log(Object.entries(person)); // [["name", "Jessica"], ["age", 30]]

#### This keyword 
<b>.this</b> keyword is used to access and manipulate other properties of the same object. This keyword refers to the object executing the function. It's important to mention that the value of 'this' can change, making 'this' very dynamic.

Example:

    let person = {
        name: "Jessica",
        greet() {
            console.log(`Hello, my name is ${this.name}`);
        }
    };
    person.greet(); // Output: "Hello, my name is Jessica"


#### Extra JS object methods:
- Object.freeze() makes an object immutable, preventing any changes.
- Object.seal() allows modifying existing properties but prevents adding or deleting properties.


#### Personalised function to manipulate an object

    function updateUserAge(user, newAge) {
        user.age = newAge;
        return user;
    }

    let updatedUser = updateUserAge(user, 32);
    console.log(updatedUser); // Output: { name: "Jessica", age: 32 }


# Q12	
<b>JavaScript Object Notation (JSON)</b> is a lightweight text data format, however it's syntax is derived from JS objects, key- value pair, hence the reason why they look similar. One of main benefits of having a similar syntax to JS objects it that the conversion between both JSON and JS objects can be done very easily. JSON is extremely compatible with numerous programming languages.

JSON is commonly used to transfer data between the browser and the server. JavaScript has two built-in methods to manipulate JSON data format: JSON.parse() and JSON.stringify() methods. Since JSON is a data format, there aren't plenty manipulation that can be performed on them, instead you need to convert JSON into JS objects or arrays first and then you can use one of the numerous methods JavaScript offers.

#### JSON format
- Data is stored in *name/value* pairs.
- Data is split by commas.
- JSON keys must be string type placed within double quotes.
- JSON strings cannot contain functions, undefined, or special JavaScript values like Infinity or NaN.
- JSON value can be string, number(int or float), boolean, array, object or null.
- Curly braces hold objects.
- Square brackets hold arrays.


Example of JSON text format:

    {
        "name": "Jessica",
        "age": 31,
        "city": "Melbourne"
    }   

#### JSON.parse() method
The JSON.parse() method converts JSON strings into JavaScript objects. This method is commonly used when receiving data from a web server or external source such as API, as data is often sent in JSON format. By parsing the JSON string, you turn it into a JavaScript object, which can then be manipulated using JavaScript’s built-in methods and properties.

Example:

    const jsonString = '{"name": "Jessica", "age": 31, "city": "Melbourne"}';   

    const person = JSON.parse(jsonString);

    console.log(person.name); // Output: "Jessica"
    console.log(person.age);  // Output: 31
    console.log(person.city); // Output: "Melbourne"

When using the parse() method on JSON array, the method will return a JS array instead of a JS object.

    const jsonArrayString = '[{"name": "Jessica", "age": 31}, {"name": "Jairo", "age": 29}]';

    // Parsing the JSON string to convert it to a JavaScript array
    const users = JSON.parse(jsonArrayString);

    console.log(users);
    // Output: [ { name: 'Jessica', age: 31 }, { name: 'Jairo', age: 29 } ]

#### JSON.stringify() method
The JSON.stringify() method converts a JavaScript object into a JSON string. This is often used when sending data to a server for storage (local or session storage), as JSON strings are a standard data format for web communication.

Example:

    const person = {
        name: "Jessica",
        age: 31,
        city: "Melbourne"
    };

    // Converting the JavaScript object into a JSON string
    const jsonString = JSON.stringify(person);

    console.log(jsonString);
    // Output: '{"name":"Jessica","age":31,"city":"Melbourne"}'


The JSON.stringify() method can also accept additional arguments to format the output, making the JSON string more readable. For example, you can specify the number of spaces for indentation, which is useful for debugging or logging data.

Example of pretty-printing using JSON.stringify() method:

    const prettyJsonString = JSON.stringify(user, null, 2);
    console.log(prettyJsonString);
    /* Output:
    {
        "name": "Jessica",
        "age": 31
    }
    */

#### JSON.stringify() Replacer Function
This method can take a replacer function as a second argument, which allows you to select which properties to include or exclude when converting an JS object into JSON string.

Example:

    const user = { name: "Jessica", age: 31, password: "secret123" };
    const jsonString = JSON.stringify(user, (key, value) => {
        return key === "password" ? undefined : value; // Exclude the password
    });
    console.log(jsonString); // Output: '{"name":"Jessica","age":31}'
