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
    |    |  |- models
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

## Logger:
## API Documentation:
This is the one of the important part of the project development. It will help developers and testers to understand apis in the project their request and responses. There are so many tools are available in the market for this. Just choose one of them which is best suitable for your project.
    https://blog.hubspot.com/website/api-documentation-tool

## Unit Test: 
This is the era of test driven development. In each project client, and senior tech fellow expect proper unit test write for the project with high test coverage & report. So this is the responsability of each and every developer, to add a proper unit test feature with best unit test framework. Jest is the one of the very famous unit test framework in the market for Node projects.
 * <b>Jest:</b> https://basarat.gitbook.io/typescript/intro-1/jest  
For more information of unit test frameworks click on the link: https://blog.logrocket.com/comparing-best-node-js-unit-testing-frameworks/
