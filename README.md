# plurality

This is a program written in C for the CS50x course by Harvard University. The program implements a "plurality" voting system.

Usage

To use the program, first compile it using the following command:

go
Copy code
make plurality
After the program has been compiled, run it from the command line with the following syntax:

css
Copy code
./plurality [candidate1] [candidate2] ... [candidateN]
where [candidate1], [candidate2], ..., [candidateN] are the names of the candidates running for election. The program will then prompt the user to enter the number of voters and then ask each voter to enter their choice. The program will then output the winner of the election.

Background

In a plurality voting system, each voter is allowed to vote for one candidate, and the candidate with the most votes wins. If there is a tie for the most votes, the program should output all candidates who tied.

Implementation

The program makes use of a candidate struct to store information about each candidate, including their name and the number of votes they have received. The program prompts the user for the number of voters, and then uses a loop to ask each voter to enter their choice. Each vote is then counted and the candidate with the most votes is determined. If there is a tie, all candidates who tied are output.

Examples

yaml
Copy code
$ ./plurality Alice Bob Charlie
Number of voters: 5
Vote: Alice
Vote: Charlie
Vote: Bob
Vote: Bob
Vote: Charlie
Charlie
In this example, there are three candidates running for election: Alice, Bob, and Charlie. There are five voters, and the votes are as follows: Alice, Charlie, Bob, Bob, Charlie. Therefore, Charlie wins the election with two votes.
