# navigation_dqn

## Environment Details

**State Space:** The state space has `37` dimensions and contains the agent's velocity, along with ray-based perception of objects around agent's forward direction.

**Action Space:**  At each time step, the agent has four actions at its disposal:
- `0` - walk forward 
- `1` - walk backward
- `2` - turn left
- `3` - turn right

**Rewards:** A reward of `+1` is provided for collecting a yellow banana, and a reward of `-1` is provided for collecting a blue banana.

**Solved Criteria:** The task is considered solved when the agent gets an average score of +13 over 100 consecutive episodes.

## Linux Dependencies

To be able to run the code in this repository, you will need to manually download the unity environment from [here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip), and modify its path in the Navigation_DQN.ipynb jupyter notebook.

You will also need to install PyTorch and the [Unity ML Agents package](https://github.com/Unity-Technologies/ml-agents).

## Structure

**model.py:** Python file that contains the Neural Network model.

**dqn_agent.py:** Python file that includes the Q-Network and the ReplayBuffer classes, and helpfer Q-learning functions.

**Navigation_DQN.ipynb:** Jupyter Notebook the contains the training code.

**checkpoint.pth:** The saved PyTorch model weights.

