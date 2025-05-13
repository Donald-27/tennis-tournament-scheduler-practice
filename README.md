# tennis-tournament-scheduler-practice
This simple program helps determine how many tennis matches can be played simultaneously in the first round of a tournament.
Tennis Tournament Scheduler
This simple program helps determine how many tennis matches can be played simultaneously in the first round of a tournament.

 Problem Description
You are hosting a tennis tournament.

There are P players already registered.

You have reserved C tennis courts.

Each game:

Requires 2 players

Takes up 1 court

You want to maximize the number of games that start at the same time.

The task is to calculate the maximum number of games that can be hosted in parallel (i.e., at the same time).

Example 1

P = 5
C = 3
Explanation:

Players: 5 Max 2  pairs  2 games

Courts: 3  Can host up to 3 games

 So 2 games can be played at once.

Result:
solution(5, 3)  # Output: 2


Example 2

P = 10
C = 3
Explanation:

Players: 10  5 pairs 5 games

Courts: 3  Only 3 games can be hosted

 So, 3 games can be played at once.

Result:

python
Copy code
solution(10, 3)  # Output: 3
 How It Works
We use the following logic:

A game needs 2 players, so total possible games = P // 2

We can't use more courts than we have, so final answer = min(P // 2, C)

