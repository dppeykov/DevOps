DevOps Interview Questions 👨🏻‍💻
===============================

### 1. Define DevOps and what does it mean to you?

> **DevOps is a culture and a way of thinking**, it is not a particular tool or set of tools. A good way to think of DevOps is through the CAMS principle:

> **CAMS** = **C**ulture, **A**utomation, **M**easurements, **S**haring 
>  - __Culture:__ result of the way teams interact. In DevOps the operations (sys admins) and the developement teams are working closely toghether towards a common goal;
>  - __Automation:__ used to speed up the feedback between teams by using tools that allow collaboration and repeatable processes. Examples are tools for revision control (version control = git), continuous integration (Jenkins, GitLab, CircleCI ...) and configuration management (Chef, Ansible, Puppet ...); Additional principle is **people over processes over tools** - once the people understand the culture, they can start creating the automation: 
>     - Who is responsible for a job function;
>     - Defining the process around them;
>     - Selecting and implementing the tools;
>  - __Measurement:__ used to track the progress/improvements. Helps finding bottlenecks and degradations during deployment; The metrics are telling what is happening and whether the changes are improving anything or not; DevOps is advising to focus on the key metrics of the systems like cost, revenue, etc;
>  - __Sharing:__ allows for exchanging of ideas, problems and solutions between the teams. Contributes to the transparency of thoughts and the open culture of the teams/company; **Kaizen (discrete continues improvement)** = sharing ideas and problems is the heart of collaboration and DevOps;

> The **practice of operations (Ops = Linux admins, Windows admins, DBAs ...) and development engineers (Dev = programmers, QA, front & back-end ...) participating together in the entire service lifecycle**, from desing through the development process to production support.

> **Benefits**: more frequent deployment (delivering value faster), less fails and faster revcovery.


### 2. Can you describe the DevOps LifeCycle?

> The DevOps lifecycle consists of **8 stages** in a constant loop. The first 4 activities (plan, code, build, test) are focused more on the development processes and teams, while the other 4 (release, deploy, operate, monitor) - on the operations.

![alt text](https://www.360logica.com/blog/wp-content/uploads/2017/10/devops-unified-workflow_1.png "DevOps LifeCycle")


### 3. What are the differences between Lean, Agile and DevOps?

> To compare Lean and Agile to DevOps we need to know what the first 2 are. 

>**Lean** - an approach to software development focused on optimizing development resources with the initial goal of delivering MVP (Minimum Viable Product). Once the MVP is released to the market, the development team takes feedback and makes adjustments (adds/removes/improves) to the software product based on the customer's requests. 

> **Agile** - a framework for multiple approaches for software development, most commonly of which is the SCRUM approach.
> - **SCRUM** uses 2 weeks periods for application development, called __sprints__. During each sprint the development team uses input from the business (**feedback cycle**) to add specific features and/or repair bugs. at the end of the sprint a **new version** of the application is released.

> **Differences** - communication & operations - in the Lean & Agile the teams are separated, but the DevOps combines them and improve the communication. Also the Lean & Agile are focusing either on MVP or sprints to deliver the product, while the DevOps is trying to use continuous delivery and deployment.


### 4. How would you explain CI/CD (Continuous Integration/Delivery)?

> **Continuous Integration** - the developers **code in a local repo** and **commit** their changes on a **regular basis**. Then the code can be **integrated** with another team's code if needed. The next step is **testing** and checking for errors.

> **Continuous Delivery** - allows the developers to build, test and **release** their software. It adds to the CI. Including tests in the process allows the team to be confident of the quality of the product.

> __(lint, unit testing, typesciprt, prettier ...) --> Code PR --> Tests --> Build --> Merge --> Acceptance tests --> Manual Deployment__

> **Continuous Deployment** - add to CI/CD by including the **deployment of the software without human interaction**. Example is GitHub pages.

> __(lint, unit testing, typesciprt, prettier ...) --> Code PR --> Tests --> Build --> Merge --> Acceptance tests --> Auto Deployment__

> **CI/CD tools**: 
 - self-hosted (build by the company itself, usualy internal) - Bamboo, TeamCity, Jenkins
 - Software as a Service (SaaS - cloud-based tools) - TravisCI, Codeship, CircleCI
 - Cloud Service Providers - AWS, Google Cloud, Azure
 - Code Repositories (provides CI/CD services and code tracking) - GitHub, GitLab, Bitbucket 
 
 ![alt text](https://i.stack.imgur.com/yOofB.png "CI/CD")
 
