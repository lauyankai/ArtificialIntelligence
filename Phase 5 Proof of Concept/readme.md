## 1. Project Summary
In this final AI assignment, my team and I developed a visual Proof of Concept (PoC) for our proposed system: **"AI-Powered Predictive Analytics for Optimised Crop Yield and Risk Mitigation"**. The core objective was to translate our previously designed AI logic, PEAS models, and state space searches into a tangible, user-friendly mobile application interface for farmers. 

We designed high-fidelity UI mockups to demonstrate how the AI agent would practically communicate its reasoning to the user across five distinct real-world scenarios:
1.  **Critical Flood Risk Management:** The agent ingests weather API data, detects heavy rainfall expected within 48 hours, and actively plots a red danger zone on the farmer's map to minimize crop loss.
2.  **Harvest Optimisation Strategy:** To maximize profit, the agent tracks market data. When the market price for corn jumps by 15% while the crop is fully mature, it explicitly triggers a "Suggest Full Harvest" recommendation.
3.  **Environmental Care & Recommendation:** When local sensors detect abnormal environmental readings, such as low water, declining nutrients, and harmful UV sunlight intensity, the agent generates an immediate task list (e.g., "Need More Water" or "Recommend Put Shader").
4.  **Low Humidity Action:** To maintain high crop quality, the agent alerts the farmer if they attempt to harvest during a low humidity zone, advising them to wait for optimal conditions.
5.  **Performance Analysis & Yield Prediction:** A comprehensive dashboard tracks 90-day environmental trends (temperature, rainfall, wind speed) and visualizes estimated future yields, such as a projected 2,450 tons for the next season.

---

## 2. Reflection

### What I Have Gained

* It taught me the vital importance of **Explainable AI (XAI)** and User Experience (UX) design. I learned that having a highly accurate predictive model is useless if the end-user (in this case, a traditional farmer) does not understand or trust it. 
* By designing interfaces that provide explicit reasoning, such as telling the farmer *why* they should harvest today ("Market corn price is up 15%") rather than just giving a binary command, I realized that building user trust is just as important as building the underlying algorithm.
* A major improvement would be to design an **IoT Automation Layer** within the app. Instead of just notifying the farmer, the app could feature an "Approve Action" button that communicates directly with smart irrigation systems or automated greenhouse shaders, closing the loop between AI prediction and physical execution.