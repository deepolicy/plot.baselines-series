# plot.baselines-series

A series of running results of baselines ppo with different environments.

# To use the code

Save the output of baselines to .txt file in terminal, e.g., 

```
python -m baselines.run --alg=ppo2 --env=HalfCheetah-v2 --network=mlp --num_timesteps=2e7 > print.HalfCheetah-v2.txt
```

The codes in notebook can load value from .txt file and parse it to plot all the figures.

# Performances

PPO in baselines performs well in environments of Reacher-v2, Humanoid-v2 and HalfCheetah-v2.

Especially for Reacher-v2, where PPO can learn quickly.

While PPO make a bad performance on Hopper-v2, and the reward drops.

For Pendulum-v0, PPO get failure, because the reward never rise and even drop.