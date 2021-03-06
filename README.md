# Project4_AI_Gym

For all programming assignments I used some of Dr. Wocjan's code as a base so I wouldn't have to start from scratch. There are some remnants of this, but none should really affect runtime heavily.

1. With how large the state space is I figured it would be easier to run a search of random policies than it would be to come up with one of my own. To do this, I generated 1000 weight vectors which could successfully make it to 200. Then, I simulated each weight vector in 100 trials, and recorded the overall reward through these 100 trials. At the end I selected the weights from the policy which scored the highest, and used those weights as my discrete policy: [-0.15075671,0.61489836,0.70569531,0.89512992]

2. This one was rather simple. I used a policy which looked at velocity and position, determined if the direction (sign) of the position and velocity were the same relative to the center, and used that to decide if the cart should push right or left.

3. This one was a little bit tricky, but not too bad. I designed a reward function for the purpose of training with cross entropy which looked at the furthest point traveled by the car in both directions, and used the distance between them. One tricky part of the problem was that the action to push right was value 2, whereas the cross entropy with one hot encoding considered it to be action 1, so this had to be considered. It took 28 iterations of training to converge.
