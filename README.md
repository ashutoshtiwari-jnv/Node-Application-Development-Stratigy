# Node-Project-Development
Documentation to build and run Node project with latest tools and frameworks.

# Repository & File Structure:
Any project have a good repository and file structure, it will help developers to manage project dependecies, features,tests, etc peoperly in the project. a unstructured code create mess as project goes bigger. a good structured code make project scalable, managable, and developer can easily find and fix any bug and implement, any new feature without much change the old code.
#### Below is the one repo/file structure:
<b><code>
ProjectXYZ:
    |-src:
    |    |-controllers
    |    |  |- All controllers
    |    |  |- index.ts
    |    |
    |    |-db
    |    |  |- migrations
    |    |  |     |- 1234.users.ts (migration for users)
    |    |  |     |- index.ts
    |    |  |- models
    |    |  |     |- users.ts (model for users)
    |    |  |     |- index.ts (All relations should be here)
    |    |  |- seeders
    |    |  |- index.ts // db connections should be there
    |    |
    |    |-config
    |    |  |- db_config.ts
    |    |  |- constants.ts
    |    |
    |    |-routes
    |    |  |- index.ts
    |    |
    |    |-middlewares
    |    |  |- vlidators
    |    |  |      |- xyz_validator.ts
    |    |  |      |- index.ts
    |    |  |- All other middlewares should be here.
    |    |  |- index.ts
    |    |
    |    |-services
    |    |  |- All third party services should be here (like: kafka, logger, redis etc)
    |    |-utils
    |    |  |- All utility functions should be here
    |    |-app.ts  // This file containes server class and middleware reserved here.
    |    |-index.ts  // Call servers instance, db instance etc.
    |     
    |-tests
    |-.env.example
    |-dockerfile
    |-package.json
    |-README.md
    |-tsconfig.json
</code></b>


## Http Server Configuration:
## Database Selection:
## ORM Selection & DB Configuration:
ORM stands for Object-Relational Mapping. In a Node.js project, an ORM (such as Sequelize or TypeORM) is a tool that enables developers to interact with a relational database using an object-oriented paradigm.

Here's a breakdown of what ORM does:

**Abstraction of Database Operations:** With an ORM, developers can perform database operations (such as querying, inserting, updating, and deleting data) using familiar programming constructs like classes, objects, and methods, rather than writing raw SQL queries.

**Mapping of Objects to Database Tables:** ORM libraries map JavaScript objects to corresponding database tables and vice versa, allowing developers to work with database entities as if they were regular JavaScript objects.

**Data Validation and Type Casting:** ORMs often provide built-in mechanisms for data validation and type casting, ensuring that the data being saved to the database meets certain criteria and is of the correct data type.

**Database Agnostic:** ORMs abstract away the specific details of the underlying database system, making it easier to switch between different database engines without needing to change much of the application code.

**Relationship Management:** ORMs support defining and managing relationships between different database tables/entities, such as one-to-one, one-to-many, and many-to-many relationships.

Overall, ORMs simplify database interactions and help streamline the development process by providing a higher level of abstraction and reducing the amount of boilerplate code needed to work with databases in Node.js projects.

Top ORMs in market:
1. Sequalize (Recommended: Supports Model, Migration, Seeder)
2. Prisma (2nd Recommendation)
3. TypeORM
4. KnexJs

**Note:** Code related to ORM should be in the db repo.

To know more about ORMs, Please go through below link:
- https://amplication.com/blog/top-6-orms-for-modern-nodejs-app-development
- https://www.eversql.com/best-orm-for-node-js/
- https://medium.com/@aabedraba/choosing-a-database-solution-and-orm-for-node-js-6c256ced72ff
## Request Validator:
## Caching:
## Logger:
## Project Documentation in .md file:
## API Documentation:
This is the one of the important part of the project development. It will help developers and testers to understand apis in the project their request and responses. There are so many tools are available in the market for this. Just choose one of them which is best suitable for your project.
    https://blog.hubspot.com/website/api-documentation-tool

## Unit Test: 
This is the era of test driven development. In each project client, and senior tech fellow expect proper unit test write for the project with high test coverage & report. So this is the responsability of each and every developer, to add a proper unit test feature with best unit test framework. Jest is the one of the very famous unit test framework in the market for Node projects.
 * <b>Jest:</b> https://basarat.gitbook.io/typescript/intro-1/jest  
For more information of unit test frameworks click on the link: https://blog.logrocket.com/comparing-best-node-js-unit-testing-frameworks/

## Message Broker Selection:

## Rate Limtiter Configuration:

## Dockerizing/Containerization:
