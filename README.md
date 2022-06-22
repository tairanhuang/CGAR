# CGAR: Critic Guided Action Redistribution in Reinforcement Leaning

Code for the paper

CGAR: Critic Guided Action Redistribution in Reinforcement Leaning

Paper link:

Tairan Huang, Xu Li, Hao Li, Mingming Sun, Ping Li

IEEE Conference on Games (CoG), 2022

## Requirements
Install Mujoco from: http://www.mujoco.org/index.html

To install requirements:

```setup
pip install -r requirements.txt
```

## Running

To get the results in the paper, run this command in sac or cgar-sac:

```train
python train.py device=cuda:0 seed=1 env=walker_walk hydra.run.dir=log K=200
```

>We use Python 3.6.8 and set seeds as 1,2,3,4,5. We conduct all the experiments on Titan X. The results could be found in log/eval.csv.
>The implementation of SAC comes from https://github.com/denisyarats/pytorch_sac
