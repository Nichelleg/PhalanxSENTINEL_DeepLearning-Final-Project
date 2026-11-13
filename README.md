# 🛡️ PhalanxSENTINEL
### AI-Powered Cybersecurity for Robotic Warehouse Operations

#### **Developed by Phalanx AI:** Robert Thompson, Njeh Ababio, Olis Bahari, Nichelle Graf

#### Final Project  |  ITAI 2376 - Deep Learning  |  Fall 2026

#### **Houston City College**

**Project Status:** Development and Prototype Testing

---

## Project Overview

**PhalanxSENTINEL** is a proposed AI-powered cybersecurity monitoring system designed to help protect robotic warehouse environments against network threats, security vulnerabilities, and unauthorized robotic activity.

As warehouses increasingly depend on interconnected robots, industrial control systems, and automated communications, cybersecurity incidents can potentially disrupt operations, compromise equipment integrity, and create physical safety risks.

PhalanxSENTINEL explores how specialized AI detection agents can work together to identify suspicious activity and support cybersecurity monitoring in these environments.

The project combines machine learning, synthetic cybersecurity data, threat simulation, and performance evaluation to investigate the capabilities and limitations of AI-assisted warehouse security.

## Proposed System Architecture

PhalanxSENTINEL incorporates three specialized cybersecurity detection functions.

### Agent 1 — Network Anomaly Detection
Monitors network traffic patterns to identify potentially malicious activity, including denial-of-service (DoS) attacks.

**Detection technology:** XGBoost machine learning classifier.

### Agent 2 — Vulnerability Assessment
Evaluates and prioritizes potential cybersecurity vulnerabilities to support risk assessment and security decision-making.

**Detection technology:** To be documented as the team's implementation develops.

### Agent 3 — Robot Integrity Monitoring
Analyzes robotic telemetry, command sources, timing, and movement behavior to identify potentially unauthorized commands or abnormal robot operations.

**Detection technology:** Random Forest machine learning classifier.

Together, these functions form the foundation of the proposed cybersecurity monitoring system.

The complete system architecture and agent integration strategy remain under development.

---

## Dynamic Threat Simulation and Evaluation

An important part of developing PhalanxSENTINEL is determining how effectively its detection models recognize simulated cybersecurity threats.

The project includes an interactive **Dynamic Threat Simulation and Detection Evaluation** notebook developed by Nichelle Graf.

This testing environment allows users to generate new synthetic cybersecurity scenarios and evaluate existing trained detection models without modifying their underlying architectures.

### Supported Simulations

**Network Security Testing — Agent 1**
- Gradual DoS attacks
- Sudden DoS attacks
- Configurable attack duration and intensity
- Adjustable detection thresholds

**Robot Integrity Testing — Agent 3**
- T0855 unauthorized command simulations
- Simulated abnormal robot movement
- Unauthorized command-source activity
- Configurable attack timing and intensity

### Interactive Testing Capabilities

Users can configure simulation parameters through an interactive interface, including:

- Detection agent and attack type
- Simulation duration
- Attack start and end times
- Attack intensity
- Random seed
- Detection threshold

Each simulation generates synthetic observations, processes them through the appropriate feature-engineering pipeline, and evaluates the selected detection model.

### Performance Evaluation

Detection performance is measured using:

| Metric | Purpose |
|---|---|
| Precision | Measures the proportion of alerts that correctly identify attacks |
| Recall | Measures the proportion of actual attacks detected |
| F1 Score | Balances precision and recall |
| False-Positive Rate | Measures incorrect alerts during normal activity |
| Miss Rate | Measures attacks that remain undetected |
| Confusion Matrix | Summarizes correct and incorrect classifications |

Detection timelines and visualizations help illustrate how model behavior changes under different simulated threat conditions.

Initial experiments have demonstrated successful dynamic scenario generation and evaluation for Agents 1 and 3. Further validation is necessary before drawing conclusions about real-world cybersecurity performance.

---

## Technologies and Development Tools

The project currently uses or evaluates the following technologies:

| Technology | Application |
|---|---|
| Python | Simulation, data processing, and evaluation |
| Google Colab / Jupyter Notebook | Development and interactive experimentation |
| NumPy | Synthetic data generation and numerical operations |
| Pandas | Data preparation and analysis |
| Scikit-learn | Machine learning evaluation and classification metrics |
| XGBoost | Network anomaly detection |
| Random Forest | Robot integrity detection |
| Matplotlib | Detection timelines and performance visualization |
| ipywidgets | Interactive simulation controls |
| GitHub | Version control and project documentation |

Additional technologies supporting the complete multi-agent architecture will be documented as the project progresses.

---

## Repository Organization

The repository will be organized as development continues.

```text
PhalanxSENTINEL-DeepLearning-Final/
│
├── README.md
├── requirements.txt
│
├── notebooks/
│   └── PhalanxSENTINEL_Dynamic_Threat_Simulation.ipynb
│
├── docs/
│   ├── Project_Proposal.pdf
│   └── Evaluation_Strategy.md
│
└── team_contributions/
```

Some files and directories may not be available during the initial repository setup.

---

## Development and Execution

The dynamic simulation notebook is designed to execute in Google Colab.

The evaluation notebook uses existing detection models and feature-engineering pipelines developed separately for a related robotic warehouse cybersecurity capstone project.

These source components are maintained independently from this Deep Learning final project.

### Running the Simulation Notebook

1. Open the notebook in Google Colab.
2. Execute the notebook cells sequentially to initialize the environment and required dependencies.
3. Generate the synthetic datasets and prepare the detection models.
4. Execute the evaluation experiments.
5. Navigate to the interactive simulation section.
6. Select an agent and configure a new threat scenario.
7. Click **RUN SIMULATION** to generate and evaluate the selected scenario.

The notebook includes documentation, evaluation metrics, and visualizations to support interpretation of the results.

**Note:** Initial setup may require generating synthetic datasets and training detection models before interactive testing can begin.

---

## Evaluation Objectives

The project aims to investigate the following questions:

1. Can AI-based detection models identify simulated cybersecurity threats affecting robotic warehouse operations?
2. How effectively can the models distinguish malicious activity from normal network and robotic behavior?
3. How do changing attack characteristics influence detection performance?
4. What trade-offs exist between successful threat detection and false-positive alerts?
5. How can controlled simulation and quantitative evaluation support the development of more reliable cybersecurity monitoring systems?

These questions guide the project's experimental design and performance evaluation strategy.

---

## Project Scope and Limitations

PhalanxSENTINEL is an academic research and prototype development project.

Current testing uses synthetic network and robot telemetry rather than live industrial systems.

The simulation environment evaluates model predictions under controlled conditions and does not provide autonomous cybersecurity intervention or physical robot control.

The project does not currently establish operational readiness, real-world detection reliability, or compliance with industrial cybersecurity standards.

Additional validation, system integration, and security testing would be required before any commercial deployment.

---

## Development Team

**Phalanx AI**  
Houston City College  
ITAI 2376 — Deep Learning  
Fall 2026

**Documented contribution:**

**Nichelle Graf** — Dynamic Threat Simulation, Detection Evaluation, Interactive Testing, and Evaluation Methodology.

Additional team member responsibilities and contributions will be documented as the project develops.

---

## Academic Project Statement

PhalanxSENTINEL is being developed as part of the Fall 2026 Deep Learning course at Houston City College.

The project investigates applications of artificial intelligence and machine learning to cybersecurity challenges involving automated warehouse environments.

The current implementation is intended for educational research, simulation, and demonstration purposes.
