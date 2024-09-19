## 📈 Market Swarm Agents 🚀

Welcome to the **Market Swarm Agents** – an open-source toolkit designed to bring the power of advanced AI agents to your financial market strategies. Imagine having a swarm of virtual analysts, each with their own unique trading style, working tirelessly to decode market signals and identify opportunities in real-time. Well, now you can!

![image](https://github.com/user-attachments/assets/c19adab6-5f59-4660-b323-1f9df221e45d)



### 🧠 What Is It?
This platform leverages advanced machine learning models and customizable trading strategies under a unified framework. It allows you to simulate and optimize a diverse set of agents:

- **Scalper Agent**: Specializes in high-frequency trading, executing quick entries and exits to capture small market movements.
- **Trend Follower Agent**: Identifies and rides long-term trends in the market, aiming to maximize profits from sustained price movements.
- **Correlation Agent**: Analyzes the relationships between various market assets to make informed trading decisions.

The **Master Agent** oversees all these agents, ranks their performance, allocates resources, and ensures optimal operation across the swarm.

### 🔥 Key Features
- **Hierarchical Agent Management**: The Master Agent supervises individual agents, tracks their performance, and allocates resources dynamically based on their effectiveness.
- **Integrated Short and Long Strategies**: Each agent can independently execute short and long strategies as part of its trading logic.
- **Live Monitoring and Performance Tracking**: Monitor the live status, performance metrics, and positions of each agent in real-time.
- **Dynamic Resource Allocation**: The Master Agent adjusts resources based on the performance and market conditions.
- **QuantStats Integration**: Analyze backtesting results with comprehensive performance reports generated by `quantstats`.
- **Scalable and Extensible**: Easily add or modify agents, strategies, and resource management rules.

### 📋 File Structure
- **`data/`**: Contains shared market data and a central event data stream.
  - **`shared_data/`**: Market data accessible to all agents.
  - **`events_data/`**: Central event log collecting all agent insights.
- **`master_agent/`**: Contains the Master Agent logic, performance tracking, and resource allocation.
  - **`master_agent.py`**: MasterAgent class with all management and oversight logic.
- **`agents/`**: Each agent has its own file with integrated methods for short and long strategies, training, and performance tracking.
  - **`base_agent.py`**: BaseAgent class with shared logic.
  - **`scalper_agent.py`**: ScalperAgent class with all related functionality.
  - **`trend_follower_agent.py`**: TrendFollowerAgent class with all related functionality.
  - **`correlation_agent.py`**: CorrelationAgent class with all related functionality.
- **`shared/`**: Shared utilities and data handling.
  - **`data_handler.py`**: DataHandler class for data loading/processing.
  - **`feature_extractor.py`**: FeatureExtractor class for feature extraction.
  - **`event_stream.py`**: Event stream handler.
- **`cli.py`**: Command-line interface for managing agents and strategies.
- **`utils.py`**: Common utilities like logging, configuration, etc.
- **`config.py`**: Configuration file for global parameters.
- **`run_market_swarm.py`**: Main entry point to run all agents.

### 🛠️ Getting Started
1. **Clone the Repository**: 
   ```bash
   git clone https://github.com/your-repo/multi-agent-market-analysis.git
   ```
2. **Install Dependencies**: 
   ```bash
   pip install -r requirements.txt
   ```
3. **Configure Agents and Master Agent**: Adjust the agent and master parameters in `config.py` to match your requirements.
4. **Run the Platform**: Start the agents under the supervision of the Master Agent using:
   ```bash
   python cli.py run
   ```
5. **Train and Backtest Agents**: Use the individual `train()` methods in each agent's class to backtest strategies with historical data:
   ```bash
   python cli.py train -agent scalper -data data/shared_data/historical_data.csv
   ```

### 📡 Data Providers
To ensure accurate and reliable market data, the platform can integrate with various data providers. Below are some recommended providers:

| Logo                                    | Name                  | Visit Link                        | Price      |
|-----------------------------------------|-----------------------|-----------------------------------|------------|
| ![Alpha Vantage](https://www.alphavantage.co/favicon.ico) | **Alpha Vantage**    | [Visit Alpha Vantage](https://www.alphavantage.co/) | Free/Pro   |
| ![Quandl](https://www.quandl.com/favicon.ico) | **Quandl**            | [Visit Quandl](https://www.quandl.com/)             | Variable   |
| ![IEX Cloud](https://iexcloud.io/static/favicon.ico) | **IEX Cloud**        | [Visit IEX Cloud](https://iexcloud.io/)           | Free/Pro   |
| ![Polygon](https://polygon.io/favicon.ico) | **Polygon.io**        | [Visit Polygon.io](https://polygon.io/)           | Variable   |
| ![Tiingo](https://www.tiingo.com/favicon.ico) | **Tiingo**            | [Visit Tiingo](https://www.tiingo.com/)           | Subscription |

### 🖥️ Platforms
Deploy this platform on various environments to suit your development or live trading needs. Below are some recommended platforms:

| Logo                                      | Name               | Visit Link                         | Price                                    |


### 🤝 Contribute & Collaborate
This project is a community effort! Feel free to open issues, suggest features, or submit pull requests. Let's build something amazing together and push the boundaries of market analysis with AI!

### 📬 Stay in Touch
Join our [Discord](#) community for discussions, updates, and more. Share your ideas, ask questions, and connect with fellow market enthusiasts.

---

Unleash the power of AI agents on the financial markets and see where the future of trading can take you! 🌐💡✨

---

### License
This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.


