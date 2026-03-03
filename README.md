Global-Trade-Disruption-Risk-Simulator
This project models the economic impact of maritime chokepoint disruptions (e.g., Suez Canal) using Monte Carlo simulation and scenario-based risk modeling. Stochastic Modeling | Monte Carlo Simulations | Agentic AI (Llama 3.3)

📊 Executive Summary

In an era of increasing maritime volatility, static trade models are insufficient. This project is a Decision Intelligence Tool designed to quantify the economic impact of global chokepoint disruptions (e.g., Suez Canal, Panama Canal). By integrating Stochastic Modeling with Agentic AI, this engine moves beyond "average" forecasts to identify Tail-Risk (95th/99th Percentile)—providing actionable strategic advisory for C-suite stakeholders.

The Technical Stack Engine: Probabilistic Modeling via Monte Carlo Simulations (10,000+ iterations). Logic: Stochastic Variable Mapping using Triangular and Gamma distributions for blockage duration and rerouting costs. Brain: Agentic AI Layer powered by Llama 3.3 (via Groq LPUs) for real-time strategic interpretation. Visualization: Interactive Plotly dashboards for Value at Risk (VaR) distribution.

🚀 Key Features Multi-Scenario Stress Testing: Toggle between 'Minor Congestion', 'Major Blockage', and 'Catastrophic Failure' states. Rerouting Economics: A dual-path logic that simulates the financial trade-off between idling vs. rerouting (e.g., Cape of Good Hope) with associated fuel and time premiums. Tail-Risk Quantification: Automatically calculates 95% VaR and 99% Worst-Case scenarios, identifying "Black Swan" events that traditional linear models miss. Agentic Strategy Layer: An AI Consultant that "reads" the simulation variance and provides sector-specific mitigation strategies (e.g., Inventory Buffer vs. Air Freight pivot).

📈 Methodology: The "Consultant" Approach Data Ingestion: Processed UN Comtrade/Global Trade Flow datasets to establish effective daily trade exposure ($6.69B/day baseline). Stochastic Sampling: Ran 10,000 simulations using numpy to model the uncertainty of blockage duration ( ) and cost multipliers ( ). Risk Aggregation: Visualized the probability density function to highlight the Value at Risk (VaR)—the industry standard for enterprise risk management.

📂 Repository Structure notebooks/: The core Google Colab logic and Monte Carlo engine. data/: Cleaned global trade datasets and disruption parameters. assets/: Professional Plotly histograms showing the Risk Distribution

<img width="1920" height="870" alt="Screenshot 347" src="https://github.com/user-attachments/assets/4b17dcd3-24e6-4860-81b9-651b4f4b8d8e" />

Graph: Tail Risk (VaR Levels) 
What it shows: This histogram depicts the distribution of all simulated economic losses, with two vertical lines: one for 95% VaR (typically green) and another for 99% catastrophic risk or 99% VaR (typically red).
Key insights: The visualization highlights tail risk, showing that most simulations result in low or zero losses, but a small probability exists for extremely high losses. The 95% and 99% VaR lines indicate thresholds beyond which only the worst 5% and 1% of cases occur, respectively, providing insight into rare but high-impact events.

<img width="1920" height="885" alt="Screenshot 346" src="https://github.com/user-attachments/assets/25834d35-49a3-48f7-bed9-2fdb27bf6ed8" />
Graph: Supply Chain Risk Comparison Across Disruption Scenarios 
What it shows: This bar chart displays the 95% Value at Risk (VaR) for three disruption scenarios: Minor Port Congestion, Major Suez Canal Blockage, and Total Maritime Chokepoint Failure. The 95% VaR represents the maximum loss that is not expected to be exceeded with 95% confidence.
Key insights: VaR 95 increases sharply with the severity of the disruption scenario, highlighting the potential maximum losses companies could face in 95% of cases. Notably, Total Maritime Chokepoint Failure exhibits a significantly higher VaR, emphasizing the high-end exposure risk.

<img width="1920" height="929" alt="Screenshot 349" src="https://github.com/user-attachments/assets/802a966a-9d43-497b-bc74-5174f2f23be6" />
Graph: Global Trade Disruption Risk by Scenario 
What it shows: This bar chart compares average expected economic losses (in billions USD) across three scenarios: Minor Port Congestion, Major Suez Canal Blockage, and Total Maritime Chokepoint Failure.
Key insights: Average losses increase with the severity of the disruption, with Total Maritime Chokepoint Failure representing the highest expected financial impact. This visualization makes it easy to compare the typical costs associated with each type of event.


<img width="571" height="455" alt="download" src="https://github.com/user-attachments/assets/5aa490c3-01c8-4c5a-82d7-c34b0e08ba10" />
Graph: Monte Carlo Loss Distribution 
What it shows: This histogram represents the frequency distribution of simulated economic losses from the Monte Carlo model. The x-axis shows loss amounts, while the y-axis shows the number of occurrences in the simulations.
Key insights: The distribution is heavily right-skewed. The large peak near zero indicates that most simulations result in minimal disruption or loss. The long tail to the right represents less frequent but potentially severe losses, giving an overall picture of the range and likelihood of possible outcomes
