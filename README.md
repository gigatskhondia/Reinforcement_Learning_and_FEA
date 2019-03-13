# Engineering Design by Reinforcement Learning and Finite Element Analysis
Models in repository aim to optimize design of a structure via combining finite element analysis and reinforcement learning. The finite element model represents an environment to which an agent applies actions and from which it gets observations and rewards. Agent uses neural network policy gradient algorithm. The algorithm optimizes the parameters of a policy by following the gradients toward higher rewards. The end result of the modeling is an optimal (in terms of displacements) design of a structure.

For more information see the manual.

## 1. Simple finite element analysis optimized by reinforcement learning 

  A bar is subjected to axial tensile force. The model optimizes by altering cross-sectional area and material of the bar in order to keep the maximum displacement in the 1D structure within acceptable limit.  An action, in this case, is altering parameters of cross-sectional area and Young's modulus in a certain way.  If an action leads to alleviation of displacements, measured by FEA, the agent gets a reward.


## 2. Design of a bridge by reinforcement learning

  The model optimizes positions of joints in order to minimize vertical displacement in middle node of the bridge like 2D truss structure. The agent gets a reward if the middle node displacement is reduced due to change in position of truss joints. 


## 3. Spool design by plane frame element and reinforcement learning

  This model optimizes geometry in order to minimize maximum displacement in a “spool”. The agent gets a reward if the maximum nodal displacement is reduced due to change in the spool geometry. The FE model uses a plane frame element.

## 4. Generative design of bionic partition for airplane cabin interiors by reinforcement learning and finite element analysis

  The model optimizes geometry in order to maximize strength and “minimize” weight of bionic partition.
