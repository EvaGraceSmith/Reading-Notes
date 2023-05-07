## Express, NPM, TDD, CI/CD
____

Express software helps you more easily write server software, and learning test driven development helps you improve the quality of your code.  

### [An introduction to NodeJS and Express](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs/Introduction)

#### 1. Explain middleware, answer as though I were a non-technical recruiter.

"Middleware is software that helps different programs or systems communicate with each other. Think of it as a bridge or a translator between different applications.

For example, let's say you have a website that needs to access data from a database. The website and the database are two different systems that don't speak the same language, so you need something in between to help them understand each other. That's where middleware comes in - it sits between the website and the database and handles the communication between them.

Middleware can also perform other tasks, such as security, data transformation, and routing. It's a very useful tool for integrating different systems and making sure they work together seamlessly.

In summary, middleware is software that helps different applications talk to each other by acting as a bridge or a translator. It's a valuable tool for integrating different systems and making sure they work together smoothly." - ChatGPT

#### 2. Express the most popular *backend framework for Node. js*.

#### 3. Express is “unopinionated.” What does that mean?

"In the context of web development using the Node.js platform, "unopinionated" typically means that the framework or library does not impose a particular way of structuring your code or solving a problem.

Express is often described as an "unopinionated" web framework because it provides a set of basic features for building web applications, such as routing and middleware, but it doesn't force you to use a particular architecture or design pattern. Instead, you have the flexibility to structure your application in the way that best suits your needs.

For example, Express doesn't dictate how you should organize your controllers, models, and views, or which database you should use. You're free to choose the tools and practices that work best for you and your team.

This approach can be contrasted with "opinionated" frameworks or libraries, which often come with strong conventions and opinions about how to structure your code or solve a particular problem. While opinionated frameworks can be helpful in providing a clear structure and reducing cognitive load, they can also be limiting and force you to work in a particular way, even if it doesn't align with your needs or preferences." - ChatGPT


#### 4. What is a module and why is modularity useful to us as developers?

"In software development, a module is a self-contained unit of code that performs a specific function and can be reused in different parts of an application or in different applications altogether. Modules typically encapsulate data and functionality into a single unit, making it easier to manage and maintain complex codebases.

Modularity is the practice of breaking down a large system into smaller, more manageable components, or modules. This approach has several benefits:

Reusability: By separating code into modules, developers can reuse code across different parts of an application or even in different applications altogether. This can save time and effort by reducing the need to write the same code multiple times.

Encapsulation: Modules typically hide their implementation details from the rest of the application, providing a clean interface for other parts of the code to interact with. This can reduce the risk of bugs and make it easier to change the implementation details without affecting other parts of the codebase.

Maintainability: Large codebases can be difficult to manage and maintain, especially if there are many dependencies between different parts of the code. Modularity can make it easier to isolate and fix bugs, update functionality, and add new features without affecting other parts of the codebase.

Scalability: Modularity can make it easier to scale applications by allowing developers to add or remove modules as needed, without affecting other parts of the codebase.

Overall, modularity is a useful practice for developers because it can help reduce complexity, increase reusability, and make code easier to manage and maintain over time." - ChatGPT


### [What is NPM?](https://docs.npmjs.com/about-npm)
___

#### 1. What version of npm are you running on your machine?

9.6.4

#### 2. What command would you type to install a library/package called ‘jshint’ into your node project?

npm i jshint



### [What is TDD? (Test Driven Development)](https://www.agilealliance.org/glossary/tdd/#q=~(infinite~false~filters~(postType~(~'page~'post~'aa_book~'aa_event_session~'aa_experience_report~'aa_glossary~'aa_research_paper~'aa_video)~tags~(~'tdd))~searchTerm~'~sort~false~sortDirection~'asc~page~1))
___

#### 1. Explain why tests are important. Please explain as though I were your non technical elder.

"Test Driven Development (TDD) is a software development practice that involves writing automated tests before writing the code that will make those tests pass. The goal of TDD is to improve the quality of the code by catching defects early and ensuring that the code is working correctly.

TDD is important because it helps ensure that the code works as intended and is free of errors. By writing tests before writing code, developers can identify potential issues early in the development process, when it is easier and less expensive to fix them. TDD also helps ensure that the code is maintainable and can be easily modified in the future, which is important because software is constantly evolving.

In addition to improving the quality of the code, TDD can also improve the efficiency of the development process. By catching defects early and reducing the need for manual testing, TDD can help reduce the time and cost of developing and maintaining software.

Overall, TDD is an important practice in software development that can help ensure the quality and maintainability of the code, and improve the efficiency of the development process." - ChatGPT


#### 2. What are three expected benefits of testing

* "Many teams report significant reductions in defect rates, at the cost of a moderate increase in initial development effort
* The same teams tend to report that these overheads are more than offset by a reduction in effort in projects’ final phases
* Although empirical research has so far failed to confirm this, veteran practitioners report that TDD leads to improved design qualities in the code, and more generally a higher degree of “internal” or technical quality, for instance improving the metrics of cohesion and coupling" - [Agile Alliance](https://www.agilealliance.org/glossary/tdd/#q=~(infinite~false~filters~(postType~(~'page~'post~'aa_book~'aa_event_session~'aa_experience_report~'aa_glossary~'aa_research_paper~'aa_video)~tags~(~'tdd))~searchTerm~'~sort~false~sortDirection~'asc~page~1))


#### 3. Name at lest 2 individual pitfalls and at least 2 team pitfalls commonly encountered while writing tests.

"Typical individual mistakes include:

* forgetting to run tests frequently
* writing too many tests at once
* writing tests that are too large or coarse-grained
* writing overly trivial tests, for instance omitting assertions
* writing tests for trivial code, for instance accessors

Typical team pitfalls include:

* partial adoption – only a few developers on the team use TDD
* poor maintenance of the test suite – most commonly leading to a test suite with a prohibitively long running time
* abandoned test suite (i.e. seldom or never run) – sometimes as a result of poor maintenance, sometimes as a result of team turnover" -[Agile Alliance](https://www.agilealliance.org/glossary/tdd/#q=~(infinite~false~filters~(postType~(~'page~'post~'aa_book~'aa_event_session~'aa_experience_report~'aa_glossary~'aa_research_paper~'aa_video)~tags~(~'tdd))~searchTerm~'~sort~false~sortDirection~'asc~page~1))

### CI/CD
___

#### 1. What are three benefits of Continuous Integration?

"Continuous Integration (CI) is a software development practice that involves automatically building and testing code changes as they are made, typically on a shared code repository. Here are three benefits of CI:

* Early Detection of Integration Issues: CI helps detect integration issues early in the development process by constantly building and testing code changes as they are made. This means that if a change introduced by one developer breaks the build or causes tests to fail, the entire development team is notified immediately, and the issue can be fixed before it becomes a bigger problem.

* Faster Feedback Loop: With CI, developers receive feedback on their changes within minutes, allowing them to quickly iterate and make improvements. This can help reduce the time it takes to develop and release new features or bug fixes.

*  Increased Confidence in Code Quality: By automating the build and testing process, CI can help increase confidence in the quality of the codebase. Developers can be more confident that their changes are not introducing new bugs or breaking existing functionality, and the entire team can be more confident that the codebase is stable and reliable.

Overall, CI can help improve collaboration, reduce the risk of integration issues, increase code quality, and speed up the development process." - ChatGPT


#### 2. What is the difference between Continuous Delivery and Continuous Deployment?

"Continuous Delivery (CD) and Continuous Deployment (CDep) are both software development practices that involve automatically building, testing, and releasing code changes. The main difference between the two is in the scope of the automation:

* Continuous Delivery (CD): CD is a practice where code changes are automatically built, tested, and prepared for release. The goal of CD is to have a release-ready codebase at all times, so that new features and bug fixes can be released quickly and reliably. In CD, the actual release of the code is still done manually, usually by a human.

* Continuous Deployment (CDep): CDep takes the automation a step further by automatically deploying code changes to production as soon as they pass all tests and checks. This means that new features and bug fixes are released automatically without human intervention, as soon as they are ready.

In other words, the key difference between CD and CDep is that CD focuses on preparing code changes for release, while CDep actually releases them automatically.

Both CD and CDep can be useful practices for software development, depending on the needs and goals of the development team. CD can help improve collaboration and reduce the time it takes to release new features or bug fixes, while CDep can help reduce the risk of human error and speed up the deployment process. However, CDep requires a high degree of confidence in the quality of the codebase and the reliability of the deployment process, and may not be appropriate for all applications or teams." -ChatGPT


#### 3. Explain how GitHub fits into this process assuming the listener comes from a non-technical background

"GitHub is a website where people who write computer programs can store their work and collaborate with others. It's kind of like a virtual library for computer code.

When people write computer programs, they often make changes to their code over time. These changes can cause problems, so it's important to keep track of them. GitHub helps people do this by keeping a record of all the changes made to a program over time. This is called "version control."

In addition to version control, GitHub has tools that help people work together on programming projects. For example, if two people are working on the same program, they can use GitHub to coordinate their efforts and make sure they don't accidentally overwrite each other's work.

GitHub also has tools that can automatically test programs to make sure they work correctly. This is important because it helps catch mistakes before the program is used by other people.

Overall, GitHub is a website that helps people who write computer programs collaborate, keep track of changes, and make sure their programs work correctly." - ChatGPT


### Bookmark and Review
____

[nodeJS docs](https://nodejs.org/en/docs)

[npm docs](https://docs.npmjs.com/)

[express docs](https://expressjs.com/en/4x/api.html)

[http status codes](https://www.restapitutorial.com/httpstatuscodes.html)

[supertest](https://github.com/ladjs/supertest)

### Reflection
___
#### What are your learning goals after reading and reviewing the class README?
* I am excited to write and test an express server!
* I also want to learn more about 'super test'



## Things I want to know more about
___
* I want to become more familiar and comfortable with writing a server.

* I want to learn best practices for writing test that are easy to maintain and follow.
