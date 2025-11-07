# NetworkAware-AgentPy

[![Python Version](https://img.shields.io/badge/python-3.9%2B-blue)](https://www.python.org/)
[![License](https://img.shields.io/github/license/yomex96/NetworkAware-AgentPy)](https://github.com/yomex96/NetworkAware-AgentPy/blob/main/LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/yomex96/NetworkAware-AgentPy?style=social)](https://github.com/yomex96/NetworkAware-AgentPy/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/yomex96/NetworkAware-AgentPy?style=social)](https://github.com/yomex96/NetworkAware-AgentPy/network/members)

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

## What Makes It Novel

| Feature | Why It Matters |
|--------|----------------|
| **Network-aware agent interactions** | Moves beyond idealized simulations |
| **Resilience and robustness metrics** | Evaluates failure recovery strategies |
| **Emergent behavior observation** | Supports large-scale system analysis |
| **Reproducible experiment pipelines** | Enables fair comparison across models |

This framework is designed to support **research reproducibility**, benchmarking, and experiment scaling.

---

## Example Simulation (Demo)

**Notebook:** `notebooks/demo_simulation.ipynb`

Scenario:
- Autonomous agents (e.g., vehicles or drones) navigate and coordinate actions.
- Communication is limited by latency + packet loss.
- Performance is evaluated under increasing network stress.

---

## Installation

```bash
git clone https://github.com/yomex96/NetworkAware-AgentPy.git
cd NetworkAware-AgentPy
pip install -r requirements.txt

```bash
jupyter notebook notebooks/demo_simulation.ipynb

```
```bash
NetworkAware-AgentPy/
│
├── agent_models/           # Agent definitions & behaviors
├── network/                # Network graph and communication constraints
├── experiments/            # Experiment runner + metrics
├── notebooks/              # Example simulations and visualization notebooks
└── requirements.txt
```





# Research Metrics Supported

Communication Success Rate

Coordination Efficiency

Resilience Under Failure

Emergent Behavior Patterns


Example snippet:
```bash
success_rate = successful_transmissions / total_transmissions
print("Communication Success Rate:", success_rate)
```

# Citation

```bash
Onawole, A.R. (2025). NetworkAware-AgentPy: A network-aware multi-agent simulation framework. GitHub. https://github.com/yomex96/NetworkAware-AgentPy
```

# License

This project is released under the MIT License.






