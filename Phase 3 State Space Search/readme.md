## 1. Project Summary
In this assignment, my team and I advanced the logic of our agricultural forecasting system, **"AI-Powered Predictive Analytics for Optimised Crop Yield and Risk Mitigation"**, by mapping its decision-making capabilities using **State Space Search**. The core objective was to map out all possible environmental conditions and actions to algorithmically find the optimal path from an initial state to a desired goal state.

We structured the complex agricultural lifecycle into four distinct state space modules:
1.  **Planting Phase Optimisation:** The AI navigates variables like soil humidity and flood risks starting from a "Plot Empty" state. It evaluates path costs (where waiting adds time cost) to successfully reach the "Planted" goal state under ideal conditions.
2.  **Emergency Risk Mitigation:** Starting from a "Growing Phase", the AI monitors for sudden threats. If a high flood risk is detected, the agent checks if the crop is of "Harvestable Age"; if true, it executes an "Early Harvest" action to reach the "Crop Saved" goal, preventing total loss.
3.  **Normal Harvest Optimisation:** This module focuses on profitability. Starting from a "Mature Crop" state, the AI evaluates market prices. If prices are low, the AI will suggest "Delay Harvest", but it continuously monitors "Crop Health Declining" to ensure crops are selectively harvested before spoiling.
4.  **Resource & Growth Monitoring:** The AI sequentially checks environmental conditions, starting with Water Level, moving to Nutrient Level, and finally Sunlight Level. It recommends specific actions (e.g., "Recommend Put Shader" for high sunlight) to ultimately reach the "Healthy Growth" goal.

---

## 2. Reflection

### What I Have Learnt 

* By explicitly defining the four components of a State Space Search, the Initial State, the Actions (Set of action-state pairs), the Goal Test, and the Path Cost, I learned how to quantify decision-making. 
* For example, in the Normal Harvest Optimisation module, I learned how to represent lost profit and increased crop risk as a measurable "Path Cost". Every time the system chooses to "Delay Harvest" to wait for better market prices, the path cost increases due to the risk of crop deterioration. This taught me that AI doesn't just look for *any* solution; it evaluates the cost of different routes to find the most efficient and profitable sequence of actions.
* We would need to implement advanced heuristic search algorithms, such as **A* (A-Star) Search**. Rather than just following strict True/False paths, a heuristic function could dynamically estimate the exact financial cost of moving from one state to another, allowing the AI to process vastly more complex, non-linear environments.