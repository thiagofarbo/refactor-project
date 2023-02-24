## Change description

## Features

- I used the optional chaining (?.) syntax to check that event and event.partitionKey are defined before trying to access them, instead of using multiple if statements
- I've combined the if statements that check whether candidate exists and whether it's a string into a single condition using typeof.
- Removed the let candidate statement; and set candidate directly based on event.partitionKey or TRIVIAL_PARTITION_KEY.
- I moved the logic to generate a hash to after the candidate length check, as it is only needed if candidate is too long.

## Tech Stack

Below some technologies that are been using;

- [TypeScript] - HTML enhanced for web apps!
- [Jest] - awesome web-based text editor

## To run this application follow the information below.

To build the application.

```sh
cd rafactor-test
node deterministicPartitionKey.js
```

To run the tests.

```sh
npm test
```
