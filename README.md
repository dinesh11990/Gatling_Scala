# Gatling Scala Performance Testing - ReqRes.in

## Overview
This repository contains a Proof of Concept (PoC) for performance testing using **Gatling** with **Scala**. The PoC tests various API endpoints of [ReqRes.in](https://reqres.in), a popular REST API for testing and prototyping.

## Tech Stack
- **Gatling**: Load testing framework for performance testing.
- **Scala**: Used for scripting test scenarios.
- **sbt**: Build tool for Scala-based projects.

## Project Structure
```
├── src
│   ├── test
│   │   ├── scala
│   │   │   ├── simulations
│   │   │   │   ├── ReqResSimulation.scala
│   │   │   ├── resources
│   │   │   │   ├── gatling.conf
├── build.sbt
├── README.md
```

## Installation & Setup
### Prerequisites
Ensure you have the following installed:
- **Java 8 or higher**
- **Scala**
- **sbt (Scala Build Tool)**

### Clone the Repository
```sh
git clone https://github.com/dinesh11990/Gatling_Scala.git
cd Gatling_Scala
```

### Run the Simulation
To execute the test:
```sh
sbt gatling:test
```

## Test Scenarios
The `ReqResSimulation.scala` file contains different API test scenarios:
1. **GET /users?page=2** - Retrieves a list of users.
2. **POST /users** - Creates a new user.
3. **PUT /users/{id}** - Updates a user.
4. **DELETE /users/{id}** - Deletes a user.

## Test Reports
After running the tests, Gatling generates detailed HTML reports in the following directory:
```
target/gatling/
```
Open the report in a browser to analyze response times, throughput, and error rates.

## Contributing
Feel free to contribute by submitting issues or pull requests.

## License
This project is licensed under the MIT License.

