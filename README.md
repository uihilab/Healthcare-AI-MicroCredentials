# Healthcare AI Micro-Credentials: An Open-Source Curriculum Initiative 🏥🤖

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)
[![License: AGPL v3](https://img.shields.io/badge/License-AGPL%20v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)

Welcome to the collaborative curriculum repository for the **Healthcare AI Micro-Credentialing** cyberinfrastructure. 

As predictive algorithms and decision-support tools are rapidly integrated into clinical and administrative workflows, there is an urgent need to train the healthcare workforce on AI safety, algorithmic bias, and clinical oversight. Traditional multiple-choice assessments are insufficient for evaluating the nuanced clinical reasoning required in the age of AI. 

This repository serves as the central hub for crowdsourcing, developing, and peer-reviewing an open-access, role-specific curriculum designed to be deployed on our logic-based, AI-assisted credentialing platform.

## 🎯 Project Vision

Our cyberinfrastructure utilizes a node-based visual editor, localized Large Language Models (LLMs), and mandatory "rationale assessments" to evaluate a learner's underlying thought process when interacting with clinical AI. 

However, the technology is only as good as the clinical expertise behind it. Our goal is to build a massive, globally searchable repository of high-fidelity, peer-reviewed clinical simulations spanning the entire hospital ecosystem.

## 👥 Who We Are Looking For

We are issuing an open call to the global medical education community. We need subject matter experts to help us author branching scenarios for the following functional domains:

* **Physicians & Medical Providers** (Surgical, Medical, Intensive Care, Diagnostics)
* **Advanced Practice & Midlevel Providers** (NPs, PAs, CNMs)
* **The Nursing Workforce** (Inpatient, Outpatient, ICU, Informatics)
* **Allied Health & Therapeutics** (PT/OT, Respiratory, Pharmacy)
* **Imaging, Radiology, & Laboratory Services**
* **Health Information, Billing, & Revenue Cycle**
* **Quality, Safety, Compliance, & Hospital Operations**

# Clinical Scenarios

There are currently **19 scenarios**. Contributions are welcome — see [Contributing](#contributing) below.

## Scenarios

| Scenario | Topic | Focus | Decisions | Endings |
|---|---|---|---|---|
| [Case Study: Early Deterioration and Conflicting AI Signals](unit1-recognizing-risks/README.md) | unit1-recognizing-risks | Navigate a realistic clinical scenario involving patient Mr. Allen to learn about automation bias, over-reliance, and workflow integration. | 5 | 7 |
| [The Drowning Heart](heart-failure/README.md) | Heart Failure | acute and chronic management of Heart Failure | 6 | 4 |
| [The 40-Week Clock](prenatal-care/README.md) | prenatal care | screening windows and preventative protocols | 4 | 3 |
| [The Missing Milestone](primary-amenorrhea/README.md) | primary amenorrhea | Evaluation and diagnosis | 7 | 7 |
| [Time is Brain](ischemic-stroke/README.md) | ischemic stroke | acute management of an ischemic stroke | 4 | 5 |
| [The Growing Pains](pediatric-developmental-milestones/README.md) | pediatric developmental milestones | Evaluation and parent education | 4 | 4 |
| [The Golden Hourglass](neonatal-jaundice/README.md) | neonatal jaundice | Diagnois and management | 4 | 5 |
| [The Breathless Traveler](pulmonology-and-emergency-triage/README.md) | pulmonology and emergency triage | Pulmonary Embolism (PE) | 5 | 5 |
| [The Morning Ache](rheumatoid-arthritis/README.md) | Rheumatoid Arthritis | Rheumatology | 5 | 5 |
| [The 48-Hour Window](substance-withdrawal/README.md) | substance withdrawal | Psychiatry and Addiction Medicine | 5 | 5 |
| [The Waddell Impact](emergency-care-surgery/README.md) | Emergency care/Surgery | Multi-system trauma | 5 | 5 |
| [The Peripheral Shadow](lung-cancer/README.md) | Lung cancer | Oncology | 5 | 5 |
| [The Black Eschar](sinusitis/README.md) | Sinusitis | ENT | 5 | 5 |
| [The Restaurant Reaction](anaphylaxis/README.md) | Anaphylaxis | Allergy and Immunology | 5 | 5 |
| [The Winter Crisis](sickle-cell-anemia/README.md) | Sickle cell anemia | Hematology | 5 | 5 |
| [The Daycare Diarrhea Dilemma](diarrhea/README.md) | Diarrhea | Infectious disease/GI | 5 | 5 |
| [The Vascular Toll](diabetes-mellitus/README.md) | Diabetes Mellitus | Endocrinology | 5 | 5 |
| [The Ring-Enhancing Dilemma](hiv/README.md) | HIV | Infectious disease | 5 | 5 |
| [The Gradient Collapse](electrolytes-and-drug-interaction/README.md) | Electrolytes and drug interaction | Pharmacology/Multi-systems | 5 | 5 |

## What's in each scenario folder

```
<scenario-name>/
├── <scenario-name>.json   # the scenario graph: nodes, edges, viewport
├── README.md              # the scenario told as a story, with a flowchart
└── images/                # images shown in the scenario
```

The JSON file is a graph of nodes connected by edges. Each node has a `type`:

| Node type | What it is |
|---|---|
| `informationNode` | A story page: what is happening to the patient. The first page has `hideTopHandle: true`. |
| `decisionNode` | A decision point where the learner chooses what to do. |
| `choiceNode` | One option at a decision, labelled `A`, `B`, `C`… and marked `correct` or `misstep`. |
| `terminationNode` | An ending: `checkpoint` (a concept learned) or `fail` (try again). |

## 🛠️ How to Contribute

You do not need to be a software developer to contribute! We are looking for **clinical logic and scenario narratives**. 

### Suggest a scenario or report a problem

Open an **issue** to:

- propose a new scenario topic, or volunteer to write one
- report a clinical inaccuracy, outdated guideline, typo or broken image
- suggest a better choice, explanation or ending for an existing scenario

Please include the scenario name and, for clinical corrections, a reference to the source guideline.

### Add a new scenario

1. Fork this repository and create a branch.
2. Add a new folder under `scenarios/`, named in lowercase with hyphens (for example `septic-shock/`).
3. Inside it, add:
   - `<folder-name>.json`: the scenario graph, following the structure of the existing scenarios
   - `README.md`: an overview and the story told in order, like the existing READMEs
   - `images/`: any images the scenario uses, listed under the node's `data.images`
4. Add a row for your scenario to the table above.
5. Open a **pull request** describing the scenario, its learning goals and the sources you used.

### Guidelines

- **No real patient data.** All cases must be fictional or fully de-identified.
- **Images must be yours or openly licensed.** Note the source and license in the scenario README.
- **Every path should end.** Each choice must lead somewhere, and every branch should finish in a checkpoint or a fail ending.
- **Explain the misses.** A fail ending should say what went wrong and what the better choice would have been.
- **Cite your sources.** Base clinical content on current guidelines and list them in the README.

## 📚 About the Platform

The scenarios developed here will be integrated into a web-based cyberinfrastructure featuring:
* **No-Code Visual Authoring:** Transforming your text-based logic into interactive branching simulations.
* **Local Sovereign AI Engines:** Protecting institutional data and evaluating learner logic in real-time.
* **Adaptive Delivery:** Delivering your scenarios via classic text, interactive Socratic chat, or immersive visual environments.

## 📝 Citation and License

The curriculum content generated in this repository is licensed under the [GNU Affero General Public License v3.0](https://www.gnu.org/licenses/agpl-3.0.html).

If you use this framework or platform architecture in your research, please cite our upcoming publication:

> Vald, G., Sermet, Y., & Demir, I. (Upcoming). *Scalable Micro-Credentials for AI Literacy in Healthcare: An Open-Source Framework and Call for Collaborative Curriculum Development.* International Journal of Educational Technology in Higher Education.

## 📬 Contact

For institutional partnerships or questions regarding the cyberinfrastructure deployment, please reach out via GitHub Issues or contact the research team at Tulane University.

**Core Team:** Gabriel Vald, Yusuf Sermet, Ibrahim Demir 
(School of Science and Engineering,
School of Medicine,
Tulane University)
