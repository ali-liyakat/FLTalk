# FLTalk

FLTalk is a lightweight federated learning framework developed to simplify the deployment and experimentation of federated learning systems. It provides an easy-to-use architecture for configuring clients, servers, machine learning models, and federated aggregation algorithms with minimal setup.

## Features

- Multiple federated clients
- Central federated server
- REST API-based communication
- Multiple machine learning models
- Multiple federated aggregation algorithms
- Web-based experiment interface
- Support for custom datasets
- FedDeepSMOTE integration for imbalanced data experiments

## Project Structure

```
FLTalk/
├── backend/             # Server, models, and FL algorithms
├── FLTalk_Clients/      # Federated clients
├── FLTalk_Server/       # Federated aggregation server
├── frontend/            # Web interface
├── Run_Expt.md          # Execution guide
└── README.md
```

## Getting Started

Clone the repository:

```bash
git clone https://github.com/ali-liyakat/FLTalk.git
cd FLTalk
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Follow the instructions in **Run_Expt.md** to start the server and clients.

## Research

This framework was developed as part of a Master's research project on Federated Learning. It is designed to support rapid experimentation and includes a case study using FedDeepSMOTE for handling imbalanced data in federated environments.

## License

This project is intended for academic and research purposes.
