## 🚀 Projects

### 📊 [Top up - Software Developer - Database — DISC Profiles API](https://github.com/HarunHursid/Mandatory-2-DB)
A full-stack **multi-database ASP.NET Core Web API** for managing DISC personality profiles across an organization — built as a mandatory database exam project. The system stores and mirrors data across three different database engines simultaneously: **SQL Server**, **MongoDB**, and **Neo4j**.
[![DB Report](https://img.shields.io/badge/AI_Report-View_PDF-red?style=for-the-badge&logo=adobeacrobatreader&logoColor=white)](DB - Disc Rapport.pdf)

📚 About DISC
**DISC** is a behaviour assessment model identifying four personality types:
| Type | Colour | Trait |
|------|--------|-------|
| **D** — Dominance | 🔴 Red | Results-oriented, direct |
| **I** — Influence | 🟡 Yellow | Enthusiastic, social |
| **S** — Steadiness | 🟢 Green | Supportive, calm |
| **C** — Conscientiousness | 🔵 Blue | Analytical, detail-oriented |


This system helps organisations match employees to projects and social events based on their personality type.


## 📦 Tech Stack
| Layer | Technology |
|-------|------------|
| API Framework | ASP.NET Core 8 |
| ORM | Entity Framework Core |
| Relational DB | SQL Server |
| Document DB | MongoDB Atlas |
| Graph DB | Neo4j |
| Auth | JWT ****** |
| Mapping | AutoMapper |
| API Docs | Swagger / OpenAPI |
| Env Config | DotNetEnv |


## ✨ Features
🔐 **JWT Authentication** — register, login, role-based authorization (`Admin` / `Employee`)
- 🗄️ **SQL Server** — full relational model with Entity Framework Core
- 🍃 **MongoDB Atlas** — mirrored document store for all entities
- 🔗 **Neo4j** — graph database mirroring employee relationships, projects, DISC profiles
- 🔍 **Cross-database search** — unified `/api/search` endpoint querying SQL, MongoDB and Neo4j simultaneously
- 🔄 **Data migration tools** — standalone migrators to sync SQL → MongoDB and SQL → Neo4j
- 🖥️ **Built-in frontend** — static HTML pages (login, employee dashboard, admin panel, profile page)
- 📄 **Swagger UI** — interactive API documentation with JWT support

![C#](https://img.shields.io/badge/C%23-239120?style=flat&logo=csharp&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=flat&logo=mongodb&logoColor=white)
![Neo4j](https://img.shields.io/badge/Neo4j-008CC1?style=flat&logo=neo4j&logoColor=white)

<br>
<br>
<br>


## 📊 [Top up - Software Developer - AAI](https://github.com/HarunHursid/AI_Eksamen)

[![AI Report](https://img.shields.io/badge/AI_Report-View_PDF-red?style=for-the-badge&logo=adobeacrobatreader&logoColor=white)](HSB-Cars.pdf)

## 🏎️ AI Eksamen — Autonomous Racing Car
An AI exam project comparing three learning strategies for training a self-driving racing car in a custom **Pygame** simulation: a **Genetic Algorithm (NEAT)**, a **Deep Reinforcement Learning (DDQN)** agent, and a **Hybrid** approach that combines both.


## 🎬 Overview
A car equipped with 5 radar sensors learns to navigate a closed race track through 10 checkpoints and back to the finish line. Three separate AI approaches are trained independently and then evaluated head-to-head on a separate test track.


## ✨ Approaches

### 🧬 GA — NEAT (Neuro-Evolution of Augmenting Topologies)
- Evolves neural network **topology and weights** simultaneously using the `neat-python` library
- Population of 50 cars per generation, up to 130 generations
- Fitness = checkpoint bonuses − step penalty − crash penalty + finish bonus
- Stagnation detection removes cars that stop making progress
- Best genome saved to `ga_best_genome.pkl`

### 🤖 RL — Double Deep Q-Network (DDQN)
- Custom **Gymnasium-style** `RacingEnv` built in Pygame
- 6 discrete actions, 5 radar inputs
- Experience replay buffer + target network updated every 50 episodes
- 10 000 training episodes, epsilon greedy (ε: 1.0 → 0.1)
- Best model saved to `rl_best_model.keras`

### ⚗️ Hybrid — NEAT-seeded DDQN
- Uses the GA's best genome to **initialise the DDQN weights**
- The GA provides a good starting point; DDQN then fine-tunes with gradient descent
- Combines the exploration strength of evolution with the sample efficiency of deep RL
- Best models saved to `hybrid_best_ddqn.keras` and `hybrid_best_genome.pkl`


## 📦 Tech Stack
| Component | Technology |
|-----------|-----------|
| Simulation | Pygame |
| NEAT / GA | neat-python |
| Deep RL | Keras + TensorFlow |
| Numerical ops | NumPy |
| Image processing | scikit-image |
| Package manager | uv |
| Language | Python ≥ 3.13 |

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white).
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat&logo=tensorflow&logoColor=white).
![Keras](https://img.shields.io/badge/Keras-D00000?style=flat&logo=keras&logoColor=white).
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white).
![Pygame](https://img.shields.io/badge/Pygame-000000?style=flat&logo=pygame&logoColor=white).
![NEAT](https://img.shields.io/badge/NEAT--Python-76B900?style=flat&logo=dna&logoColor=white).
![Matplitlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat&logo=matplotlib&logoColor=white)

<br>
<br>

