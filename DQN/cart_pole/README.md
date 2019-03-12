# Deep Q-learning (DQN) to solve the cart-pole balancing problem

* The cart-pole balancing problem is a classical control problem
([CartPolev0](https://github.com/openai/gym/wiki/CartPole-v0)).

* DQN finishes training whenever it detects 5 consecutive successes or it reaches the maximum number of trials/episodes.

## Software Requirement
* Python with [PyTorch](https://pytorch.org/) and [OpenAI Gym](https://gym.openai.com/)

## Example commands to run
```
python dqn_cart_pole.py                                # With default parameter settings
python dqn_cart_pole.py -figure=false -print=false     # No figures and not printing details  (much faster)
```
## An example result
![alt text](https://raw.github.com/exalearn/reinforcement_learning/blob/master/DQN/cart_pole/epi_reward.pdf)

## Reference
* [REINFORCEMENT LEARNING (DQN) TUTORIAL by PyTorch](https://pytorch.org/tutorials/intermediate/reinforcement_q_learning.html)
