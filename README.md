# Tideman — Ranked-Pairs Voting (C)

**What it is:** A ranked-choice voting program that tallies pairwise preferences, sorts by strength of victory, and locks edges without creating cycles (Tideman/Ranked Pairs).

Built as part of [CS50x](https://cs50.harvard.edu/x/2022/).

## How it works
1. Read candidates and ballots.
2. Record pairwise preferences in a matrix.
3. Build candidate pairs and sort by margin.
4. Lock pairs into a directed graph while preventing cycles (DFS).
5. Print the winner (source of the DAG).

## Run it
```bash
make tideman
./tideman Alice Bob Charlie
