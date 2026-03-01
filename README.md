 # Global-Trade-Disruption-Risk-Simulator
 This project models the economic impact of maritime chokepoint disruptions (e.g., Suez Canal) using Monte Carlo simulation and scenario-based risk modeling.
 Stochastic Modeling | Monte Carlo Simulations | Agentic AI (Llama 3.3)
+
 📊 Executive Summary
+
 In an era of increasing maritime volatility, static trade models are insufficient. This project is a Decision Intelligence Tool designed to quantify the economic impact of global chokepoint disruptions (e.g., Suez Canal, Panama Canal). By integrating Stochastic Modeling with Agentic AI, this engine moves beyond "average" forecasts to identify Tail-Risk (95th/99th Percentile)—providing actionable strategic advisory for C-suite stakeholders.
- The Technical Stack
+
+ The Technical Stack 
 Engine: Probabilistic Modeling via Monte Carlo Simulations (10,000+ iterations).
 Logic: Stochastic Variable Mapping using Triangular and Gamma distributions for blockage duration and rerouting costs.
 Brain: Agentic AI Layer powered by Llama 3.3 (via Groq LPUs) for real-time strategic interpretation.
 Visualization: Interactive Plotly dashboards for Value at Risk (VaR) distribution.
+
 🚀 Key Features
 Multi-Scenario Stress Testing: Toggle between 'Minor Congestion', 'Major Blockage', and 'Catastrophic Failure' states.
 Rerouting Economics: A dual-path logic that simulates the financial trade-off between idling vs. rerouting (e.g., Cape of Good Hope) with associated fuel and time premiums.
 Tail-Risk Quantification: Automatically calculates 95% VaR and 99% Worst-Case scenarios, identifying "Black Swan" events that traditional linear models miss.
 Agentic Strategy Layer: An AI Consultant that "reads" the simulation variance and provides sector-specific mitigation strategies (e.g., Inventory Buffer vs. Air Freight pivot).
+
 📈 Methodology: The "Consultant" Approach
 Data Ingestion: Processed UN Comtrade/Global Trade Flow datasets to establish effective daily trade exposure ($6.69B/day baseline).
 Stochastic Sampling: Ran 10,000 simulations using numpy to model the uncertainty of blockage duration and cost multipliers.
 Risk Aggregation: Visualized the probability density function to highlight the Value at Risk (VaR)—the industry standard for enterprise risk management.
+
 📂 Repository Structure
 notebooks/: The core Google Colab logic and Monte Carlo engine.
 data/: Cleaned global trade datasets and disruption parameters.
