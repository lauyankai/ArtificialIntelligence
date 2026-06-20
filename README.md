# SECJ3553 Artificial Intelligence

## 1. Project Title
**AI-Powered Predictive Analytics for Optimised Crop Yield and Risk Mitigation**

## 2. Project Overview
This repository contains a collection of assignments for the Artificial Intelligence course, detailing the progressive conceptualisation and design of a Smart Agriculture Forecasting System. The core business problem addressed is the agricultural sector's vulnerability to unpredictable weather patterns, such as droughts and sudden floods, which cause significant yield losses. 

To solve this, our team proposed an AI-based forecasting system designed to predict the ideal weather for planting, determine the optimal time for harvesting based on environmental risks, and calculate anticipated crop output. The project evolves from initial design thinking to logic formulation, state space mapping, intelligent agent design, and finally, a visual Proof of Concept (PoC).

## 3. Team Members
*   **Lau Yan Kai** (A23CS0098)
*   **Sabrina Heng Wei Qi** (A23CS0265)
*   **Chew Chiu Xian** (A23CS0061)
*   **Najma Shakirah Binti Shahrulzaman** (A23CS0140)

---

## 4. Repository Contents (Assignments)

### 📄 [Phase 1: Design Thinking & Empathy]
*   **Topic:** Identifying User Needs and AI Solutions.
*   **Summary:** We utilized Design Thinking to empathize with farmers struggling with unpredictable rainfall and financial instability. We defined core user needs: determining optimal planting times, identifying the best harvest times to maximize yield, and receiving data-driven crop management advice. The proposal established the foundation for using AI methods like Knowledge Representation and State Space Search.

### 🧠 [Phase 2: Knowledge Representation]
*   **Topic:** Production Rules and First-Order Logic (FOL).
*   **Summary:** We translated agricultural expertise into machine-readable logic by defining 11 distinct predicates (e.g., `HarvestableAge()`, `FloodRiskHigh()`, `PlotEmpty()`). We developed core Production Rules and represented them in Predicate Logic, such as the **Emergency Harvest Suggestion**, which alerts farmers to harvest early if the crop is mature enough and flood risks are high (`∀crop[HarvestableAge(crop) ∧ FloodRiskHigh() → SuggestEarlyCrop()]`) [15-17]. This method ensures transparent reasoning and modularity.

### 🌳 [Phase 3: State Space Search]
*   **Topic:** Algorithm Decision Trees and Path Costs.
*   **Summary:** We mapped out the AI's decision-making capabilities across four state space modules:
    1.  **Planting Phase Optimisation:** Navigating from an empty plot to a planted state under optimal humidity.
    2.  **Emergency Risk Mitigation:** Detecting flood risks and triggering early harvests to reach a "Crop Saved" goal.
    3.  **Normal Harvest Optimisation:** Balancing market prices against declining crop health to maximize profits.
    4.  **Resource & Growth Monitoring:** Sequentially evaluating water, nutrient, and sunlight levels to achieve healthy growth.

### 🤖 [Phase 4: Intelligent Agent]
*   **Topic:** AI Agent Architecture and the PEAS Model.
*   **Summary:** We formalized the system as a dynamic Intelligent Agent using the PEAS framework. 
    *   **Performance:** Maximizing crop yield, survival rate (>90%), and prediction accuracy.
    *   **Environment:** Dynamic farm plots, weather conditions, and flood risk zones.
    *   **Actuators:** Alerts, yield prediction graphs, and harvest recommendation interfaces.
    *   **Sensors:** Weather Forecast APIs, soil moisture sensors, and crop age calculators.

### 📱 [Phase 5: Proof of Concept]
*   **Topic:** UI Mockups and Explainable AI (XAI).
*   **Summary:** We translated the agent's logic into high-fidelity mobile dashboard mockups to demonstrate how the AI interacts with the farmer. The PoC covers 5 scenarios:
    1.  **Critical Flood Risk:** Plotting red danger zones on the map based on 48-hour rainfall predictions.
    2.  **Harvest Optimisation:** Triggering a "Suggest Full Harvest" alert when market corn prices rise by 15%.
    3.  **Environmental Care:** Generating action lists (e.g., "Recommend Put Shader") when sensors detect harmful sunlight intensity.
    4.  **Low Humidity:** Warning the farmer to wait for optimal conditions before harvesting.
    5.  **Performance & Yield Prediction:** Visualizing 90-day estate health trends alongside estimated yield forecasts (e.g., 2,450 tons).