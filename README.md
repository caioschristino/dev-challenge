## Challenge for Developers

### Introduction
This is our programming challenge. Our goal is to know more about your programming skill level and experience, and then we can be on the same page during the interview.

### What we will evaluate:
* We want to evaluate your ability to deliver clean code with sufficient documentation for other developers to understand what you did and actively contribute to the project.

* README.md is well written, with the instructions needed to run the application, etc.
The code is well written, clean, and cohesive.

* Implementation of the solution is working as expected.

* There are well written automated tests (i.e., the unit and integration tests cover the expected behavior).

* There is a linter/static code analyss.
* RESTful API design is implemented, correctly using the HTTP verbs and the proper Status Code.

### Programming language
You can choose between Ruby or Elixir.

### How to share your code with us
We want you to experience how we work on a daily basis. That's why we ask you to use a standard git-flow as follows below.

Create a README.md file describing how to configure your project, containing the commands that must be executed to run the software and the tests.

If you have made use of any Linter, send the file together with the project.
Open a single pull request to the master branch of the private repository that we have invited you to contribute with all the code of the exercise.

## Exercise

### Introduction

Google Maps is a web mapping service developed by Google. It offers satellite imagery, aerial photography, street maps, 360° interactive panoramic views of streets (Street View), real-time traffic conditions, and route planning for traveling by foot, car, bicycle, air (in beta), and public transportation.

### Global requirements

- Register an user;
- Register an address associated to an user;
- Destroy an address by id and user;
- Update an already persisted address by id and user;
- Filter an address by the user.

### User stories

**Story 1: Register an user**

```
As a User
I want to provide my username
So that I can see registers of any address I want.
```

Requirements

- The information that must be retrieved is the username.

**Story 2: Register an address associated with an user**

```
As a User
I want to be able to add an address,
So that I can easily find them later by my username.
```

Requirements

- A address must contain zip code, number, city, district, complement, state, and the associated user;
- Validates the existence of the address before saving using the Google Maps API;
- You should persist only Brazilian addresses.

**Story 3: Updates an already persisted address by id and user**

```
As a User
I want to be able to update an address that I have added before.
```

Requirements

- A Address can update only these fields: complement, number.

**Story 4: Destroy address by id and user**

```
As a User
I want to be able to destroy an address that I have added before.
```

Requirements

- A Address can be destroyed only by the id and username;

**Story 5: Filter address by the user.**

```
As a User
I want to be able to find all addresses that I have added.
```

Requirements

- A Address can be found only by the username;

## Instructions

In order to implement the user stories listed above, please follow the instructions below:
- Your REST API must be implemented using JSON;
- Each action must have its specific route respecting the convention of `HTTP verb` and `status code`;
- Using Docker to configure the environment is recommended, but not mandatory;
- Deploy the application where to prefer.
