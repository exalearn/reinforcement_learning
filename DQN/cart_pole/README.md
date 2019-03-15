# Deep Q-learning (DQN) to solve the cart-pole balancing problem

* The cart-pole balancing problem is a classical control problem
([CartPolev0](https://github.com/openai/gym/wiki/CartPole-v0)).

* DQN finishes training whenever it detects 5 consecutive successes or it reaches the maximum number of trials/episodes.

## Software Requirement
* Python with [PyTorch](https://pytorch.org/) and [OpenAI Gym](https://gym.openai.com/)

## Hyper Parameters

| parameters      |      description                               | data type | range         | default value  |
|-----------------|:-----------------------------------------------|----------:|--------------:|---------------:|
| episodes        | the number of episodes to training             | integer   | [1, infinity) | 2000           |
| steps           | time steps in each episode                     | integer   | [1, infinity) | 200            |
| alpha           | learning rate                                  | double    | (0, 1)        | 0.01           |
| gamma           | discount factor                                | double    | [0,1]         | 0.9            |
| batch_size      | the size of mini batch for a neural network    | integer   | (0, infinity)**      | 32             |
| target_update   | time steps to update target network            | integer   | (0, infinity)***     | 100            |
| memory_capacity | the maximum capacity of replay memory          | integer   | (0, infinity)***     | 2000           |
| eps             | the initial value of epsilon                   | double    | [0, 1]        | 0.9            |
| eps_min         | the minimum value of epsilon                   | double    | [0, eps]      | 0.01           |
| eps_decay       | the rate of epsilon decay                      | double    | [0, 1]        | 0.99           |

## Other command line options

| parameters      |      description                               | data type | default value  |
|-----------------|:----------------------------------------------:|----------:|---------------:|
| reward_shaping  | Enable reward shaping?                         | bool      | True           |
| figure          | Show figures?                                  | bool      | True           |
| print           | Print details every time step?                 | bool      | True           |

## Example commands to run
```
python dqn_cart_pole.py                                # With default parameter settings
python dqn_cart_pole.py -episodes=200 -alpha=0.05      # hyper parameters
python dqn_cart_pole.py -figure=false -print=false     # No figures and not printing details  (much faster)
python dqn_cart_pole.py -reward_shaping=false          # It will take more time to train
```
## An example result
![alt text](https://github.com/exalearn/reinforcement_learning/blob/master/DQN/cart_pole/epi_reward.png)

## Reference
* [REINFORCEMENT LEARNING (DQN) TUTORIAL by PyTorch](https://pytorch.org/tutorials/intermediate/reinforcement_q_learning.html)
