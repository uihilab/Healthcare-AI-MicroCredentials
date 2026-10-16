# Clinical Scenarios

A collection of branching clinical case studies from the Healthcare AI Training Platform. In each scenario you step into a realistic patient encounter, read how the case unfolds, and make decisions at key moments. Good choices move the case forward; missteps lead to an outcome that explains what went wrong, so you can go back and try a different path.

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
