## 1. Project Summary
In this assignment, my team and I advanced our agricultural system, **"AI-Powered Predictive Analytics for Optimised Crop Yield and Risk Mitigation"**, by structuring it as a dynamic Intelligent Agent. The core objective was to design how the AI interacts with its environment to achieve its goals of maximizing crop yield and minimizing losses due to extreme weather.

To formalize the agent's architecture, we utilized the **PEAS Model** (Performance, Environment, Actuators, Sensors):
*   **Performance Measure:** The success of the agent is evaluated by its ability to maintain a crop survival rate above 90%, ensure high prediction accuracy, and maximize overall crop yield and quality.
*   **Environment:** The agent operates in a highly dynamic and unpredictable agricultural setting, monitoring farm plots, shifting weather conditions, crop growth stages, and flood risk zones.
*   **Actuators:** The agent affects the environment (and the user) through interactive interfaces, sending automated mobile alerts, generating yield prediction graphs, and displaying explicit harvest recommendations. 
*   **Sensors:** The system ingests data using both local physical sensors (Soil Moisture Sensors) and long-range digital sensors (Weather Forecast APIs and Flood Warning APIs).

We developed five detailed Proof of Concept (PoC) scenarios to demonstrate the agent's behavior. For example, if the soil is dry but the Weather API predicts heavy rain within 24 hours, the agent will logically prioritize waiting over immediate irrigation to prevent water waste. Alternatively, if market prices peak while crops are mature, the agent triggers a "Suggest Full Harvest" action to maximize profit.

---

## 2. Reflection

### What I Have Learnt

* By strictly applying the **PEAS Model**, I learned how to define an AI's boundaries. I realized that an AI agent is effectively blind and paralyzed without properly defined Sensors and Actuators. 
* Designing the Proof of Concept UI mockups taught me how an AI system communicates its reasoning to human users. For instance, when the agent recommends a "Full Harvest," it doesn't just display a binary command; it provides the context (e.g., "Market prices peaked +15% and weather conditions favorable"). This reinforced my understanding that AI transparency and user interface design are critical for building user trust, especially in traditional industries like farming.
* A significant improvement would be connecting the agent's actuators directly to automated IoT farming equipment. For example, instead of just sending a "Need More Water" notification, the agent could automatically trigger smart sprinkler systems.