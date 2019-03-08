# Deep Q-learning (DQN) to solve the mountain car problem

* The mountain car problem is a classical control problem
([MountainCar-v0](https://github.com/openai/gym/wiki/MountainCar-v0)).

* DQN finishes training whenever it detects 5 consecutive successes or it reaches the maximum number of trials/episodes.

## Software Requirement:
* Python with [PyTorch](https://pytorch.org/) and [OpenAI Gym](https://gym.openai.com/)

## Example commands to run
```
python dqn_mountain_car.py                                # default
python dqn_mountain_car.py -figure=false -print=false     # No figures and Not printing details
```

## TODO:
* Make this code work with GPU

## Reference
* [REINFORCEMENT LEARNING (DQN) TUTORIAL by PyTorch](https://pytorch.org/tutorials/intermediate/reinforcement_q_learning.html)
