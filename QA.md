# overall architecture
Looks good, follows java/spring patterns.

# improvements
- Dont like lombok, creates issues with integrated testing and building in eclipse and intellij. Would prefer to create entities using JPA Hibernate from tables.
- There are no integration tests - these should be added using @Tag ("integration-test") and only run manually on commit to dev branch.
- There are unfinished tests - stops the build process
- The tests classes do not follow the testing pattern of package.class each test should be located in the class the its testing

# production ready
- Complete unfinished tests.
- Add integration tests.
- Use Jenkins/Bamboo to build and run unit tests on commit (CI/CD)
- Only use dev environment to run integration tests on commit to dev branch
- Use Jenkins/Bamboo to deploy to environments.
- Use postman / jmeter to validate uat and prod deployments

# Nice to have
- Introduce swagger to validate APIs.
- instead of beans to create entities use sql to create database and generate entities from tables. (DBAs know much more about databases than Java developers)
- Introduce H2 as a test database that runs locally - easier to test and validate end to end code.

# 3 for 2
Code added to PurchaseService and test added to PurchaseServiceTest
Commited to github https://github.com/mwjmurphy/pizza
