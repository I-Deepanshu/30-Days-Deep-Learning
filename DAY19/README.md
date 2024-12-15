# **DAY19 - Reinforcement Learning with Deep Q-Learning (CartPole-v1)**

Welcome to the **Reinforcement Learning with Deep Q-Learning** repository! This project demonstrates how to train an intelligent agent to solve the **CartPole-v1** problem using a Deep Q-Learning (DQL) algorithm implemented in PyTorch.  

---

## **Overview**  

Reinforcement Learning (RL) is a powerful paradigm in machine learning where agents learn optimal behaviors by interacting with an environment. This project focuses on:  

- Understanding the fundamentals of RL.  
- Implementing a Deep Q-Learning agent.  
- Solving the **CartPole-v1** environment provided by OpenAI Gym.  

---

## **Environment Details**  

The **CartPole-v1** environment requires the agent to balance a pole on a moving cart by taking discrete actions (move left or right). The goal is to maximize the total reward by keeping the pole upright for as long as possible.  

- **State Space**: 4 continuous variables (cart position, cart velocity, pole angle, pole velocity).  
- **Action Space**: 2 discrete actions (move left or right).  
- **Reward**: +1 for every timestep the pole remains balanced.  
- **Termination**: The episode ends if the pole falls or the cart moves out of bounds.  

---

## **Features**  

- **Deep Q-Network**: A fully connected neural network approximates the Q-values for state-action pairs.  
- **Experience Replay**: Enhances training stability by breaking correlations in consecutive samples.  
- **Epsilon-Greedy Policy**: Balances exploration and exploitation during training.  
- **Visualization**: Tracks and plots agent performance over episodes.  

---

## **Requirements**  

### **Dependencies**  

Install the following dependencies to run the project:  

- Python 3.8+  
- PyTorch  
- OpenAI Gym  
- NumPy  
- Matplotlib  

You can install the required libraries using:  

```bash
pip install -r requirements.txt
```  

---

## **Usage**  

### **1. Clone the Repository**  

```bash
git clone https://github.com/I-Deepanshu/30-Days-Deep-Learning/tree/main/DAY19
cd DAY19
```  

This will:  
- Train the agent in the CartPole-v1 environment.  
- Save the trained model as `q_network_cartpole.pth`.  
- Display the reward plot to visualize training progress.  

### **2. Test the Agent**  

To test the trained agent, run:  

```bash
python test.py
```  

This will load the saved model and demonstrate the agent’s performance in the environment.  

---

## **Repository Structure**  

```plaintext
reinforcement-learning-cartpole/
├── SAY19.ipynb                     # Script to train the agent
├── q_network_cartpole.pth          # Q-Network architecture
├── requirements.txt                # Python dependencies 
└── README.md                       # Project documentation
```

---

## **Results**  

### **Training Performance**  

The trained agent achieves near-optimal performance, balancing the pole for the maximum reward of 500 in most episodes.  

![Training Performance Plot](results/training_rewards_plot.png)  

### **Testing Performance**  

The agent successfully balances the pole for extended durations, demonstrating the effectiveness of Deep Q-Learning.  

---

## **Key Concepts**  

- **Reinforcement Learning**: Training agents through trial and error with rewards and penalties.  
- **Q-Learning**: A value-based RL algorithm using the Bellman equation.  
- **Deep Q-Learning**: Combines Q-Learning with deep neural networks for complex state spaces.  

---

## **Future Improvements**  

- Add support for more complex environments.  
- Implement advanced RL algorithms like **Double DQN** or **Dueling DQN**.  
- Optimize hyperparameters using automated search techniques.  

---

## **References**  

1. [OpenAI Gym](https://www.gymlibrary.ml/)  
2. [PyTorch Documentation](https://pytorch.org/docs/)  
3. [Reinforcement Learning: An Introduction](http://incompleteideas.net/book/the-book-2nd.html)  

---

## **Contributing**  

Contributions are welcome! Feel free to open issues or submit pull requests to improve the project.  

---
  

Enjoy exploring Reinforcement Learning! 🚀  