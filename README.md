# JessicaVaz_T3A1


# Q1 

During our course, we have been using GIT as it's widely known and it's a very popular choice for managing code and keeping track of code changes. Apart from Git, other common source control programs are Mercurial and Subversion. When using source control for a large project, we want to ensure the GIT covers all features, and also includes the documentation as it's very important in all scale programs. The repository is hosted on the platform GitHub which offers plenty of features including branch merge, code comparison and code collaboration.

The first step is to initialise a repository in the main or master branch, which will store the project's source code and it's files. When initialising the repository, we also need to add the README.md file which contains the project's documentation. README.md file contains all of the information about the program including name and description, table of contents, all the steps required to run the application, the usage cases, the tech stacked used to build the program, contribution guidelines, license information and plenty more. The gitignore template is another option we can add when initialising the project, this file will contain all the files git should ignore when pushing content to the repository.

Through the building process, different branches are created to allow developers to work on different features independently without code conflicts. It's recommended to create a different branch for each feature as this allows independently testing and experimenting without compromising the rest of the code. When creating news branches for specific features, the conventional name used is <b>feature</b>, this ensure a clear description of what's the purpose of the extra branch. Name example bellow:

    feature/authentication

With every commit, we should include meaningful messages to describe what changes has been added or changes. A good practise to have the type of commit before the message, they provide extra details for the commit messages. Other good practices includes keeping the message short and clear.

Example of conventional commit bellow:
* git commit -m "docs: added a brief description" 
* git commit -m "feat: added a JWT to auth" 
* git commit -m "fix: fixed a bug in user auth fn" 
* git commit -m "test: test done in user's auth" 

Once all the testing has been done and the code works as it supposed, features branches can be merged into the main branch, which stores source code and production ready code. Features branches can also be deleted safely after being merged, however this is optional. The first step to merge the branch is to perform a pull request. A pull request contains information describing the branch's purpose, and it's code. Developers working in the projects can review the code, suggest improvements, provide feedback and ensure it doesn't have any conflicts with other existing branches. In case of an existing conflict, developers are required to solve the conflict first in order to proceed with the pull request. Another good feature is that Github makes it possible to assign reviewers and assignees to each branch or pull request. This ensures a structured review process and accountability for code quality.

When all required tasks and requirements has been reached, the pull request will be ready to merge. Once the process is done, an acknowledgement message will be provided and all of the content from the extra branch will be merged into the main branch. Once all branches has been merged, and the code is working as it should, the code will be ready for deployment.


### Example of a gill pull request from past Coder academy project
[Example of git pull requests](./git1.png)

References:

Workbook assignment: JessicaVaz_T2A1-A

freeCodeCamp.org. (2022). How to Write Better Git Commit Messages – A Step-By-Step Guide. [online] Available at: https://www.freecodecamp.org/news/how-to-write-better-git-commit-messages/.

‌




















# Q2	
What are the most important aspects of quality software?

# Q3	
Outline a standard high level structure for a MERN stack application and explain the components

# Q4	
A team is about to engage in a project, developing a website for a small business. What knowledge and skills would they need in order to develop the project?

# Q5	
With reference to one of your own projects, discuss what knowledge or skills were required to complete your project, and to overcome challenges

# Q6	
With reference to one of your own projects, evaluate how effective your knowledge and skills were for this project, and suggest changes or improvements for future projects of a similar nature

# Q7	
Explain control flow, using an example from the JavaScript programming language

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