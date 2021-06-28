# To build a REST api backend with NodeJS/NestJS

- all counters are maintained in memory
- must have a get request to /counters for a list of counters in a map/dictionary format for example: {"abc": 4, "xyz": 3}
- must have a post request to /counters which creates a new counter with an initial value {"counter": initialValue}
- must update (PUT) counter by 1 using put at /counters/:counter, no body is required. If there is no counter in memory this should fail (404 not found)
- must delete counter at /counters/:counter which decreases a counter value by 1, if value <= 0 the counter disappears. Does fail if counter does not exist.
- get request to /counters/:counter returns value of counter in the format {"counter": 5}. The request should fail  if the counter does not exist (404 not found). 

### Bonus

- write your tests using Jest
- AWS Lambda
- DynamoDB

### Developer notes:

Resources utilized:

- [The jest docs](https://jestjs.io/)
- [A jest cheatsheet](https://github.com/sapegin/jest-cheat-sheet#truthiness)
- [A blog with extensive information on nestjs](https://wanago.io/2020/07/06/api-nestjs-unit-tests/)
- [The nest JS docs](https://docs.nestjs.com/)
- [The nest JS section of Maximillian S's course on udemy](https://www.udemy.com/course/react-the-complete-guide-incl-redux/learn/lecture/25599450?start=15#overview)
- [Faker docs](https://www.npmjs.com/package/faker)



### Difficulties
- Time constraint due to work and move in July first
- Coding: 
  - I struggled a bit with why the exception tests were not running. Turns out I needed to pass a callback. [This medium article helped](https://medium.com/@afolabiwaheed/how-to-test-a-function-thats-expected-to-throw-error-in-jest-2419cc7c6462)



