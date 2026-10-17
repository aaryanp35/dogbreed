# Dog Breed Fetcher (Java)

This is a CSC207 (Software Design, University of Toronto) mini assignment.

## What it does

The assignment is a small client for the [Dog CEO API](https://dog.ceo/dog-api/) that looks up the sub-breeds of a dog breed:

- `BreedFetcher` defines the lookup interface, and `BreedNotFoundException` reports unknown breeds.
- `DogApiBreedFetcher` is meant to call the Dog CEO API with OkHttp and parse the JSON response.
- `CachingBreedFetcher` is meant to wrap any fetcher and cache results in a map, so repeated lookups skip the network.
- `Main.getNumberOfSubBreeds` is meant to count the sub-breeds for a breed.

## Key concepts

- Calling a REST API and parsing JSON
- Interfaces and wrapper classes (caching as a decorator)
- Checked versus unchecked exceptions
- Writing JUnit 5 tests

## Status

This repository currently holds the course starter scaffold. The three implementation tasks (`DogApiBreedFetcher`, `CachingBreedFetcher`, and `Main`) are not complete, so the provided tests fail.

## Running the tests

From the project root (JDK 11 or newer, with Maven):

    mvn test

---

Course starter code provided by the CSC207 teaching team; implementation by Aaryan Patel.
