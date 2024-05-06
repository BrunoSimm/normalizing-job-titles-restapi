# Bruno Simm - Feefo Assessment

# Normalizing Job Titles

## Prerequisites

- **JDK (Java Development Kit) 21**
- **Maven**

## Solution Overview

The `Normaliser` class works by first computing the frequency of each character in each normalised job title provided during initialization. It then compares the character frequencies of the given job title with those of the normalised titles to find the most similar match.

### Key Components

- **Constructor**: Initializes the Normaliser object with a list of normalised job titles.
    - By pre-computing character frequencies for each normalised job title, the normalise() method can quickly find the most similar match for a given title.
- **normalise()**: Takes a job title as input and returns the most similar normalised title from the list.
- **calculateQualityScore()**: Computes a quality score based on the similarity of character frequencies between two sets of frequencies.
- **computeLetterFrequencies()**: Computes the frequency of each character in a given job title.

## Test Cases

- Unit test cases have been created to validate the scenarios provided in the assessment and also validate other common scenarios.
- Testing path: **src/test/java/org/brunosimm/NormaliserTest.java**
- Execute the following steps to complile the code and execute tests:
    - mvn clean compline
    - mvn test

### Running the application
Execute the following steps:
- mvn clean
- mvn package
- java -jar .\target\oop_assesstment-1.0-SNAPSHOT.jar