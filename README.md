
# NetworkAware-AgentPy

[![Python Version](https://img.shields.io/badge/python-3.9%2B-blue)](https://www.python.org/)  
[![License](https://img.shields.io/github/license/yomex96/NetworkAware-AgentPy)](https://github.com/yomex96/NetworkAware-AgentPy/blob/main/LICENSE)  
[![GitHub stars](https://img.shields.io/github/stars/yomex96/NetworkAware-AgentPy?style=social)](https://github.com/yomex96/NetworkAware-AgentPy/stargazers)  
[![GitHub forks](https://img.shields.io/github/forks/yomex96/NetworkAware-AgentPy?style=social)](https://github.com/yomex96/NetworkAware-AgentPy/network/members)  
[![Notebook](https://img.shields.io/badge/demo_notebook-ready-brightgreen)](notebooks/demo_simulation.ipynb)  
[![Tests](https://img.shields.io/github/actions/workflow/status/yomex96/NetworkAware-AgentPy/test.yml?branch=main)](https://github.com/yomex96/NetworkAware-AgentPy/actions)

**NetworkAware-AgentPy** is a Python framework for simulating **multi-agent systems under realistic network communication constraints**.  
It enables researchers to study how **latency, packet loss, and network topology** influence **coordination, resilience, and emergent behavior** in distributed autonomous systems.

---

## Problem Addressed

Most multi-agent simulation frameworks **assume perfect communication**, which rarely occurs in real deployments such as IoT networks, smart cities, or autonomous vehicle coordination.  
This creates a gap between **theoretical algorithms** and **real-world performance**.  

**NetworkAware-AgentPy** explicitly models **imperfect communication environments** to evaluate agent coordination and robustness under failure.

---

## Key Idea / Approach

Agents communicate via a **network graph**, where each edge can have:
- Variable message **latency**
- **Bandwidth limits**
- **Packet drop probability**
- **Random or triggered link failures**

Simulation outcomes are analyzed based on **coordination efficiency**, **communication success rate**, and **resilience under disruption**.

---

## Features

- **Network Graph Simulation:** Weighted edges with latency, bandwidth, and packet loss.  
- **Agent Behavior Modeling:** Define custom agent strategies and decision-making processes.  
- **Failure Injection:** Random or scheduled link failures to test system resilience.  
- **Metrics & Visualization:** Automatic calculation of coordination efficiency, communication success, and emergent behaviors.  
- **Reproducible Pipelines:** Easily reproduce experiments using configuration files.  
- **Notebook-ready Demos:** Explore example simulations interactively.

---

## What Makes It Novel

| Feature | Why It Matters |
|--------|----------------|
| **Network-aware agent interactions** | Moves beyond idealized simulations |
| **Resilience and robustness metrics** | Evaluates failure recovery strategies |
| **Emergent behavior observation** | Supports large-scale system analysis |
| **Reproducible experiment pipelines** | Enables fair comparison across models |

---

## Example Simulation (Demo)

**Notebook:** `notebooks/demo_simulation.ipynb`

Scenario:
- Autonomous agents (e.g., vehicles or drones) navigate and coordinate actions.  
- Communication is limited by latency and packet loss.  
- Performance is evaluated under increasing network stress.

**Sample Visualizations:**

**Network Topology:**  
![Network Topology Example](docs/network_topology.png)  

**Agent Coordination Over Time:**  
![Agent Behavior Example](docs/agent_behavior.png)

---

## Installation

```bash
git clone https://github.com/yomex96/NetworkAware-AgentPy.git
cd NetworkAware-AgentPy
pip install -r requirements.txt
jupyter notebook notebooks/demo_simulation.ipynb
````

---

## Quick Start

### Run a basic simulation

```bash
python run_simulation.py --config configs/default.json
```

### Visualize agent behaviors

```bash
python visualize_results.py --input results/simulation_1.csv
```

### Customize a simulation

```bash
python run_simulation.py --config configs/low_latency.json
```

**Project Structure:**

```
NetworkAware-AgentPy/
│
├── agent_models/           # Agent definitions & behaviors
├── network/                # Network graph and communication constraints
├── experiments/            # Experiment runner + metrics
├── notebooks/              # Example simulations and visualization notebooks
├── configs/                # Simulation configuration files
├── docs/                   # Diagrams, plots, screenshots
└── requirements.txt
```

---

## Research Metrics Supported

* **Communication Success Rate**
* **Coordination Efficiency**
* **Resilience Under Failure**
* **Emergent Behavior Patterns**

**Example snippet:**

```python
success_rate = successful_transmissions / total_transmissions
print("Communication Success Rate:", success_rate)
```

---

## Experiments

Link to experiment notebooks: [Notebooks](https://github.com/yomex96/NetworkAware-AgentPy/notebooks)

* Compare agent coordination under **high latency vs low latency networks**
* Evaluate **resilience under random link failures**
* Observe **emergent behavior patterns in large networks**

---

## Contributing

We welcome contributions! Please fork the repository and submit a pull request.

**Guidelines:**

1. Fork the repository.
2. Create a feature branch.
3. Submit a pull request with clear descriptions of your changes.

---

## Citation

```bibtex
@misc{onawole2025networkaware,
  author = {Onawole, A.R.},
  title = {NetworkAware-AgentPy: A network-aware multi-agent simulation framework},
  year = {2025},
  howpublished = {\url{https://github.com/yomex96/NetworkAware-AgentPy}}
}
```

---

## License

This project is released under the MIT License.
See [LICENSE](LICENSE) for details.

---

## References

* [AgentPy documentation](https://agentpy.readthedocs.io/)
* Smith, J. et al., 2022. *Multi-agent systems under network constraints*, Journal of Autonomous Systems.

```

---

✅ **Enhancements in this version:**
- Notebook-ready badge.
- CI/tests badge placeholder.
- Diagram placeholders for network topology and agent behavior.
- Cleaner, consistent formatting and headings.
- Research-oriented emphasis with metrics and experiment details.  

If you want, I can **also create ready-to-use images/diagrams** for your `docs/` folder so your README will look fully visual and professional on GitHub.  

Do you want me to make those diagrams next?
```







