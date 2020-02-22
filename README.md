## Description
This my program created for new 2020 cs50x pset3, it takes at max 9 numbers of candidates as command line arguments, then it prompts the user for a maximum number of 100 votes going to all candidates.

For each vote, it then prompts the user to enter in the names of candidates based on their preference (ranking from 1 - Maximum Number of Candidates).

The process goes like the following:
1. The program would check if any of the candidate has a majority (1 + the greast integer of the half all number of votes). If there is any, he/she would be outputted as the winner of the election
2. If there isn't any majority vote, the program would then eliminate the candidate with the lowest number of votes.
3. Then the next preference of the vote(s) with their first preference as the previous eliminated candidate would be considered and added to the number of votes into that candidate.
4. Repeat 1-3 until there is a winner or there is a tie between remaining candidates.

Extra: If a tie between multiple candidates occurs, all of them would be considered winners.

## Usage
```python
$ make runoff
$ ./runoff [candidate ...] # array of up to 9 names of candidates being elected
Number of voters: number # be positive integers up to 100
Rank 1: candidate # first preference of voter number 1
Rank 2: candidate # second preference of voter number 1
Rank 3: candidate # third preference of voter number 1

Rank 1: candidate # first preference of voter number 2
.
.
.
```

## What I have learned
* Applications and usage of nested arrays
* Organized information transferring and utilization between function
