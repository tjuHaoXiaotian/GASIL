# Independent Generative Adversarial Self-Imitation Learning In Cooperative Multiagent Systems

This is the code for implementing the GASIL algorithm presented in the paper: Independent Generative Adversarial Self-Imitation Learning In Cooperative Multiagent Systems. 

## Code structure


## Experiments and results
### Cooperative predator-prey

#### Description
<center><img width = '300' height ='300' src ="https://raw.githubusercontent.com/tjuHaoXiaotian/GASIL/master/files/img/predator-prey.png"/></center>

Cooperative predator-prey is a more difficult version of the ’Predator-prey’ task used in MADDPG (Lowe et al. 2017). There are N slower cooperating agents (predators) must cooperatively chase one of the M faster prey in a randomly generated environment. Agents observe the relative positions of all predators and prey and the velocities of the prey only. Actions are accelerations in four directions (up, down, left and right). Each time the cooperative agents collide with a prey simultaneously, the agents will be rewarded by some reward based on the prey they captured. Different prey (e.g., Lion, Wildebeest
and Deer) has different values and different risks in the meantime. This means there are different penalties for miss-coordination on different targets. we assume that the predator can hold a prey for some game steps `t` before the other partners’ arrival.

In our experiments, we set N to 2, M to 3 and `t` to 8. In the figure above, 2 predators are in red (translucent red represents the hands of predator) and 3 prey is in blue and purple. Among the three prey, the purple one has the highest value and penalty (if misscoordination). For the other two, the lighter blue one has the lowest value and risk).
#### Results  

<video src="https://raw.githubusercontent.com/tjuHaoXiaotian/GASIL/master/files/video/cooperative_predator_prey_ddpg.mp4" controls="controls">
</video>

---


### Cooperative rowing 


### Starcraft I


## Have a try


