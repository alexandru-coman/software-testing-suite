# Software Testing Suite

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)

A Java project focused on systematic unit testing, code coverage, mutation testing, and AI-assisted test generation.

## Project overview

The project tests an availability-scheduling component that accepts a weekday and a time interval. The test suite verifies valid reservations, invalid input, boundary values, and conflicts with existing intervals.

The work combines black-box and white-box techniques with mutation analysis to evaluate the strength of the tests.

## Team

- Coman Ioan Alexandru
- Ionescu Alexandru Ioan
- Iordache Mihai
- Predescu Andrei

## Testing techniques

- Equivalence partitioning
- Boundary value analysis
- Category partitioning
- Statement coverage
- Decision and branch coverage
- Condition coverage
- Basis path testing using cyclomatic complexity
- PIT mutation testing
- AI-generated test comparison

## Tested behavior

The main method under test is:

```java
String addAvailability(DayOfWeek dayOfWeek,
                       LocalTime startTime,
                       LocalTime endTime)
```

It validates required parameters, rejects invalid intervals, detects overlaps, and confirms successful additions.

## Results

| Metric | Result |
| --- | ---: |
| Class coverage | 100% |
| Method coverage | 100% |
| Line coverage | 100% |
| Branch coverage | 100% |
| Mutation coverage | 100% |
| Surviving mutants | 0 |

## Environment

- Java JDK 23
- IntelliJ IDEA 2024.3.4.1
- JUnit 5
- Maven 3
- PIT Mutation Testing 1.4.11

## Repository contents

- [`TestareFunctionala.md`](./TestareFunctionala.md) — functional testing analysis
- [`testareStructurala.md`](./testareStructurala.md) — structural testing and CFG analysis
- [`prezentare.pptx`](./prezentare.pptx) — project presentation
- [`RaportAI.docx`](./RaportAI.docx) — AI-assisted testing report
- [`TSS/`](./TSS/) — Java source and test project

## Documentation and demo

- [Project presentation](./prezentare.pptx)
- [Demo video](https://youtu.be/kFzvszkvodQ)

## License

This project is released under the [MIT License](./LICENSE).
