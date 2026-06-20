## 1. Project Summary

For this assignment, my team and I conceptualized the logical foundation for a smart agriculture forecasting system titled **"AI-Powered Predictive Analytics for Optimised Crop Yield and Risk Mitigation"**. The core objective was to design an intelligent decision-making framework that helps farmers determine the optimal times to plant, harvest, or wait, thereby maximizing yield and minimizing losses due to unpredictable weather like floods.

To achieve this, we translated real-world agricultural expertise into machine-readable logic using **Production Rules** and **Predicate Logic (First-Order Logic or FOL)**. 
*   **Predicates:** We defined 11 distinct predicates to evaluate farm conditions, including crop status (e.g., `HarvestableAge()`, `OptimalAge()`), environmental threats (e.g., `FloodRiskHigh()`), and actionable outputs (e.g., `SuggestEarlyHarvest()`, `CheckYieldModel()`).
*   **Production Rules & FOL:** We developed five core rules to govern the AI agent's behaviour:
    1.  **Emergency Harvest:** Triggers an early harvest alert if the crop is of harvestable age and flood risk is high (`∀crop[HarvestableAge(crop) ∧ FloodRiskHigh() → SuggestEarlyCrop()]`).
    2.  **Optimal Harvest:** Suggests harvesting for maximum yield when the crop reaches the perfect age and weather risks are low.
    3.  **Predicted Yield:** Links harvesting recommendations to a machine learning yield prediction model.
    4.  **Optimal Planting:** Advises farmers to plant seeds only when the plot is empty and humidity is optimal.
    5.  **Wait / No Action:** A fallback safety rule advising farmers to wait if conditions are neither critical nor optimal.

---

## 2. Reflection

### What I Have Learnt

* I learned that an AI does not inherently "understand" agriculture; it only understands logic and math. By explicitly defining scenarios through Predicate Logic (e.g., using logical operators like AND `∧`, OR `∨`, and IMPLIES `→`), I learned how to give an AI the ability to reason mathematically. 
* I gained a deep appreciation for **Production Rules**. We specifically chose this method because it provides transparent reasoning—if the system tells a farmer to execute an emergency harvest, the farmer can clearly see it was because `HarvestableAge = True` and `FloodRiskHigh = True`. This modularity also ensures that new rules (like drought warnings) can be added later without breaking the entire system.
* A major improvement to this system would be integrating **Fuzzy Logic**. Instead of a strict `FloodRiskHigh()` being either True or False, Fuzzy Logic would allow the AI to process percentages (e.g., an 85% chance of severe flooding vs. a 40% chance of mild flooding), allowing for more nuanced decision-making and weighted recommendations.