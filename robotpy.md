
# Robot Framework vs pytest comparison of testing frameworks
* **[Robot Framework](https://robotframework.org/) used for acceptance/functional testing.** Has a simple plain text syntax and can be extended easily with Python or Java libraries. It can run on the .net-based IronPython and on Jython which is Java based.
* **[Pytest](https://docs.pytest.org/en/latest/) is the TDD 'all in one' testing framework.** Can test all and levels of software. It is considered by many to be the best testing framework with many projects on the internet having switched to it from other frameworks, including Mozilla and Dropbox. This is due to its many powerful features such as ‘assert‘ rewriting, a third-party plugin model and a powerful yet simple fixture model.

## What are the differences between Robot Framework and pytest:

|  | RobotFramework | PyTest |
| ------ | ------ | ------ |
| Execution on the client(web browser) | **YES.** Rich library and can also be easily integrated with Selenium for browser automation to test front-end components  | **YES.** Test any part of the stack including front-end components|
| Execution on the server-side | **YES.** Used for back-end tests as well | **YES.** Used for database and server components and functionality  |
| Fixtures. This ensures specific environment for a single test | **No inbuilt way.** However it can integrate with unittest and use fixtures that way | **YES.** Powerful simple fixture model that is unmatched in any other testing framework. 
| Supports data generators for tests | **YES.** The _Robot Framework Faker_ library. It contains 147 keywords used for generating random test data  | **YES.** Hook function called _pytest_generate_tests_ which is called when collecting a test function and one can use it to generate data  |
| Licence | Apache License 2.0 | MIT License  |
| Mocks | **YES.**  Access Python's mock library for mocking  | **YES.** By either using unittest.mock or using pytest-mock a thin wrapper that provides mock functionality for pytest  |
| Organizing tests in groups  | **YES.** One can create a test suite with Robot  | **YES.** Tests can be grouped with pytest by use of markers which are applied to various tests and one can run tests with the marker applied  |
