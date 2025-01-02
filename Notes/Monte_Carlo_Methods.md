# Monte Carlo Methods 

- **Estimate** the value of a certain policy (by computing the value of the states?)
- The state and action values are also estimated
- This is done by making a prediction about these values 
- Therefore the value of a policy is estimated by predicted state values 

## Follow-Up questios:
1. How is the value of a certain policy estimated? By the estimated value of states?
2. How can the value of a policy be quantified by the value of states?
3. How are the state values estimated by prediction? What role does prediction play in estimating the state values?

## Advantage over DP
- MC methods do not need to fulfill the assumption that the entire environment needs to be known from before. 
- More scalable (Can work for larger state and action space)

Q. What is a Monte-Carlo method?
- A(ny) method that uses randomness to solve problems. 
    - What is the necessity of randomness to solve these problems?
    Random sampling helps us avoid the need for considering the entire sample space, thus approximates solutions. It also handles uncertainty (There might be samples we did not sample and therefore leave samples to consider as uncertains.)
- Random sampling --> Track observables --> Make estimation about the observable property --> This property helps you to solve the problem
    - Random sampling of what? Depends on the problem
    - What observable properties? Give examples.
    Next state, reward, value of some user-defined function x. 
    - How does the estimation happen?
    Example: Expectation over the randomly sampled object.


---


Monte Carlo (MC) methods are a class of algorithms used in reinforcement learning to estimate the value of states or state-action pairs based on sample episodes. These methods rely on averaging the returns (total rewards) received from multiple episodes to make these estimations.

## Key Concepts

- **Episode**: A sequence of states, actions, and rewards that ends in a terminal state.
- **Return**: The total accumulated reward from a given state or state-action pair until the end of the episode.
- **First-Visit MC**: Estimates the value of a state or state-action pair based on the first time it is visited in an episode.
- **Every-Visit MC**: Estimates the value of a state or state-action pair based on every time it is visited in an episode.

## Advantages

- **Model-Free**: MC methods do not require knowledge of the environment's dynamics.
- **Simple to Implement**: They are straightforward to implement and understand.

## Disadvantages

- **High Variance**: Estimates can have high variance due to the randomness in episodes.
- **Requires Episodic Tasks**: MC methods are best suited for tasks that naturally break into episodes.


