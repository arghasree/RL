# Dynamic Programming 

The main idea is to break down problems into sub problems. 

Why do this?
- The problem to solve can in some way be described in terms of a recursive problem. 


## Key Components

- **State**: Sub-problem/ Representation of the sub-problem 
- **Transition**: Relationship between the sub-problems/ states.
- **Recurrence Relation**: An equation that desribes how to extract a solution to a subproblem using other subproblems. For example, (1) in VI, describing the value of a state using the the value of another state. (2) In Fibonacci series, this can be: $$F(n)=F(n−1)+F(n−2)$$.

Using these components an MDP can be solved!

## Assumptions

- The environment is fully known and can be described as an MDP.
- The state and action spaces are finite.

## Algorithms

1. **Policy Iteration**
2. **Value Iteration**


## Limitations

- DP methods require a complete and accurate model of the environment.
- They are computationally expensive for large state and action spaces.

## Example

Computing the optimal values of all the states can be solved using DP:
State: States of the MDP \
Transition: Transitional probability \
Recurrence Relationship: Bellman Equation:
                        $$V(s) = \sum_{s'}^{}P(s'|s,a)[R + \gamma V(s')]$$

## Notes
DP is model-based as it requires an accurate model of the environment in form of transition probabilities. 


