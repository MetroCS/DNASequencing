# DNA String Comparison Project
Scaffolding for student projects that involve evaluating
string comparison algorithms in the context of DNA matching.

How shall we compare algorithms?

There are really two different comparisons we want to think about:
- How well an algorithm measures biological/string similarity
- How efficiently the algorithm runs

### Test Data Provided
- DNA_sequence_database.txt - A sample database of labeled DNA sequences
- DNA_query.txt - A sample query DNA sequence

## Implementations
These are the implementation and test classes provided:
```
- AlgorithmComparisonManager.java
- DNASearchComparison.java
- DNASearchDemo.java
- DNASequence.java
- ExamplePositionMatchAlgorithm.java
- MatchResult.java
- SequenceMatcher.java
- SequenceMatcherTest.java
- SequenceScoringAlgorithm.java
```
ExamplePositionMatchAlgorithm is a simple implementation of a SequenceScoringAlgorithm as an example.

(Note: In this project we capitalize the acronym DNA fully in identifiers.)

### To add another algorithm:
Create a class implementing SequenceScoringAlgorithm.
 - Define `getName()`
 - Define `score(...)`
 - Define `higherScoreIsBetter()`
Add the algorithm to the list in DNASearchDemo.


---
## Usage
### To compile:
```
javac -cp junit17.jar:. *.java
```

### To run:
```
java DNASearchComparison DNA_query.txt DNA_sequence_database.txt
```

### To run unit tests:
```
java -jar junit17.jar --class-path . --select-class SequenceMatcherTest
```

### To produce API documentation:
```
javadoc -cp junit17.jar:. -d docs *.java
```

---
DNA Sequencing, Copyright (C) 2026 Dr. Jody Paul

This program is free software: you can redistribute it and/or modify
it under the terms of the [GNU General Public License](LICENSE) as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see [https://www.gnu.org/licenses/](https://www.gnu.org/licenses/).

This README.md document &copy; Dr. Jody Paul is licensed under [CC-BY-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)
