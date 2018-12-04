# Project4_AI_Gym

Searching Algorithms:  
    BFS: Breadth First Search - Considers closest path to origin of search first.  
    DFS: Depth First Search - Just keeps going until it reaches a dead end or a goal.  
    UCS: Assumes all steps have the same cost.  
    A*S: Uses a heuristic function to speed up BFS.  
    
Adversarial Search:  
    Reflex Agent: An agent that considers only the current state, and determines a best plan of action using an expected value of all adjacent states.  
    Minimax Search: A process by which an agent "looks ahead" and assumes that its adversaries will make the best possible move every turn.  
    Expectimax Search: Similar to minimax, except instead of assuming adversaries will make the best move, it considers all possible moves and their respective probabilities.  
    Alpha Beta Pruning: An algorithm which speeds up minimax by stopping branches of the search tree if they are already proven to be insignificant.  
    
Reinforcement Learning:  
    Policy Extraction: A process by which given a value function you can return the optimal policy.  
    Policy Evaluation: Given a policy, you can return the value function that it provides.  
    Policy Iteration: Starting with a random policy, repeat policy evaluation and policy extraction until a final policy is converged on.  
    Value Iteration: Given a random value function, you can iteratively improve it until it converges. Afterward this you can extract a policy.  
    Q-Learning/Approximate Q-Learning: A process by which an agent can learn from trial and error to generate a policy based on rewards at each step.  
    Epsilon Greedy Strategy: Adds an exploration element to the learning steps which encourages the agent to sometimes make a decision which is not known to be optimal, in the hopes of finding a new strategy.  
    Cross-Entropy: A way of comparing two vectors for their similarity - used for loss function in training neural networks.  
