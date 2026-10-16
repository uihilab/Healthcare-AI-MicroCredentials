# The Morning Ache

> Rheumatology

## Overview

| | |
|---|---|
| **Scenario key** | `Rheumatoid Arthritis` |
| **Scenario ID** | `71974c48-4339-4007-9a4c-c389ec95ca49` |
| **Story pages** | 14 |
| **Decision points** | 5 (12 choices) |
| **Endings** | 5 (0 checkpoint, 5 fail) |
| **Concepts** | `Diagnostic Anchoring & Irreversible Joint Destruction`, `Diagnostic Parsimony & Financial Toxicity`, `Disease Modification vs. Symptom Control`, `Pharmacokinetics & Bridge Therapy`, `Surgical Clearance & Silent Subluxation` |
| **Graph file** | [`rheumatoid-arthritis.json`](rheumatoid-arthritis.json) |

This is a branching case study. The learner reads each story page, then at every decision point picks one of the choices. A *misstep* leads to a fail ending that sends the learner back to try again; the *correct* path continues the story and reaches checkpoint endings that mark the concepts learned.

## Flowchart

```mermaid
flowchart TD
    n0["1. The Morning Ache"]
    n1{"2. The Initial Assessment & Bedside Manner"}:::decision
    n2["3. The Dismissive Reassurance"]
    n3["4. The Lesson:"]
    n4(["5. Terminal Outcome: The Pannus Progression"]):::fail
    n5{"6. The Alarm Remedy"}:::decision
    n6["7. The Diagnostic Stubbornness"]
    n7["8. The lesson"]
    n8(["9. Terminal Outcome: The Financial Toxicity"]):::fail
    n9{"10. The Pharmacological Bridge (Time: 1 Wee…"}:::decision
    n10["11. The Monotherapy Trap"]
    n11["12. The Lesson:"]
    n12(["13. Terminal Outcome: The Silent Erosion"]):::fail
    n13{"14. The DMARD Remedy"}:::decision
    n14["15. The Toxic Escalation"]
    n15["16. The Lesson:"]
    n16(["17. Terminal Outcome: The Hepatic Hit"]):::fail
    n17{"18. The Pre-Operative Clearance (Time: 5 Ye…"}:::decision
    n18["19. The Routine Clearance"]
    n19["20. The Lesson:"]
    n20(["21. Terminal Outcome: The Intubation Injury"]):::fail
    n21["22. The Cervical Precaution"]
    n22["23. The Standard of Care"]
    n23["24. The Objective Empathy"]
    n0 --> n1
    n1 -->|"A. The Dismissive Reassurance"| n2
    n1 -->|"B. The Oncologic Alarm"| n5
    n1 -->|"C. The Autoimmune Suspicion"| n23
    n2 --> n3
    n3 --> n4
    n5 -->|"A. The Diagnostic Stubbornness"| n6
    n5 -->|"B. Remedy Choice"| n9
    n6 --> n7
    n7 --> n8
    n9 -->|"A. The Monotherapy Trap"| n10
    n9 -->|"B. The Unprotected DMARD"| n13
    n9 -->|"C. The Standard of Care"| n22
    n10 --> n11
    n11 --> n12
    n13 -->|"A. The Toxic Escalation"| n14
    n13 -->|"B. Remedy Choice"| n17
    n14 --> n15
    n15 --> n16
    n17 -->|"A. The Routine Clearance"| n18
    n17 -->|"B. The Cervical Precaution"| n21
    n18 --> n19
    n19 --> n20
    n22 --> n17
    n23 --> n9
    classDef decision fill:#fde68a,stroke:#b45309,color:#111
    classDef fail fill:#fecaca,stroke:#b91c1c,color:#111
    classDef checkpoint fill:#a7f3d0,stroke:#047857,color:#111
```

## The Story

<a id="information-node-0"></a>
### 1. The Morning Ache

Patient Profile: Sarah, a 35-year-old woman.


Initial State: She presents to your clinic with joint stiffness and pain in her hands and wrists that has progressively worsened over the last two months. She is exhausted, reporting fatigue and an unintentional 15-pound weight loss. During your interview, she emphasizes that her symptoms are most severe when she wakes up—with stiffness lasting well over an hour—and gradually improve in the afternoon. On physical exam, you note distinct swelling and tenderness at her metacarpophalangeal (MCP) and proximal interphalangeal (PIP) joints .

![The Morning Ache](images/ab39fdf3-e1e4-46e6-a550-ecb1ceda60f5.jpeg)

**Next:** [2. The Initial Assessment & Bedside Manner](#decision-node-1)

---

<a id="decision-node-1"></a>
### 2. Decision: The Initial Assessment & Bedside Manner

Sarah is highly anxious. "My grandmother had osteoarthritis, but she was 80," she says. "Because I'm losing weight and so tired, my husband read online that this could be bone cancer. Is it?"

![The Initial Assessment & Bedside Manner](images/eb2706d3-cb3f-417d-b056-f9387ace0ddc.jpeg)

**What do you do?**

- **A. The Dismissive Reassurance** _(wrong)_ — Chuckle and tell her not to trust the internet. Reassure her that it is likely just early-onset osteoarthritis from typing too much, prescribe rest, and send her home. → [3. The Dismissive Reassurance](#information-node-3)
- **B. The Oncologic Alarm** _(misstep)_ — Validate her fear. Because she has constitutional symptoms (weight loss, fatigue), immediately order a full-body CT scan and refer her to oncology to rule out a malignancy. → [6. The Alarm Remedy](#decision-node-7)
- **C. The Autoimmune Suspicion** _(correct)_ — Empathize with her fear, explicitly reassuring her that her specific joint pattern points away from cancer. Explain that morning stiffness lasting > 1 hour, combined with MCP and PIP swelling, is the classic presentation of an inflammatory autoimmune process . You order Rheumatoid Factor (RF), anti-CCP antibodies, ESR, CRP, and baseline radiography of her hands and wrists → [24. The Objective Empathy](#information-node-14)

---

<a id="information-node-3"></a>
### 3. The Dismissive Reassurance

You send Sarah home with a diagnosis of osteoarthritis. Over the next two years, the uninhibited T- and B-cell response in her joints causes massive pannus formation . The pannus aggressively destroys her adjacent cartilage and bone. She eventually presents to another physician with irreversible ulnar deviation of her fingers and severe swan neck deformities . She has permanently lost significant functional capacity in her hands.

![The Dismissive Reassurance](images/f6eaf243-a921-4cf2-8ea6-08178a43d9e0.jpeg)

**Next:** [4. The Lesson:](#information-node-4)

---

<a id="information-node-4"></a>
### 4. The Lesson:

Osteoarthritis (wear-and-tear) typically worsens with use throughout the day and classically involves the Distal Interphalangeal (DIP) joints. Rheumatoid Arthritis is an inflammatory synovitis that causes prolonged morning stiffness (> 1 hour) and classically involves the MCP and PIP joints, sparing the DIPs . Dismissing constitutional symptoms (weight loss, fatigue)  and the specific joint distribution leads to a catastrophic delay in treatment.

**Next:** [5. Terminal Outcome: The Pannus Progression](#termination-node-5)

---

<a id="termination-node-5"></a>
### 5. Ending: Terminal Outcome: The Pannus Progression

> **Result:** fail · **Concept:** `Diagnostic Anchoring & Irreversible Joint Destruction`

Final Outcome: Failure / Delayed Diagnosis and Irreversible Damage

The Flaw: Failing to recognize the classic diagnostic criteria for RA (morning stiffness > 1 hour, MCP/PIP involvement) and dismissing the patient's valid concerns.

Actionable Improvement: Memorize the mechanical vs. inflammatory joint pain paradigms. Inflammatory pain is worse in the morning and improves with use.

_End of this path._

---

<a id="decision-node-7"></a>
### 6. Decision: The Alarm Remedy

The insurance company rejects your prior authorization for the full-body CT scan, stating that bilateral hand pain does not warrant pan-scanning for cancer.

![The Alarm Remedy](images/fd19b280-cf90-4dac-8726-b836d1ea74c7.jpeg)

**What do you do?**

- **A. The Diagnostic Stubbornness** _(wrong)_ — You bypass insurance, forcing Sarah to pay out-of-pocket for the full-body CT scan to hunt for a tumor. → [7. The Diagnostic Stubbornness](#information-node-9)
- **B. Remedy Choice** _(correct)_ — You review the clinical criteria, realize that symmetric PIP/MCP swelling with morning stiffness is a hallmark of RA, and order the correct localized X-rays and autoantibody labs (RF, anti-CCP) instead . → [10. The Pharmacological Bridge (Time: 1 Week Later)](#decision-node-36)

---

<a id="information-node-9"></a>
### 7. The Diagnostic Stubbornness

Sarah pays thousands of dollars out-of-pocket for the scan. It returns completely negative for malignancy. By the time you finally circle back to an autoimmune workup months later, she has suffered through severe, unmanaged pain, and her baseline hand X-rays now show early periarticular bony erosions. You violated the principle of diagnostic parsimony, inflicting severe financial toxicity and delaying disease-modifying treatment.

![The Diagnostic Stubbornness](images/6a5a9198-e10c-4fc7-87c4-dc4437a8bbb0.jpeg)

**Next:** [8. The lesson](#information-node-44)

---

<a id="information-node-44"></a>
### 8. The lesson

Diagnostic parsimony is critical. When a patient presents with classic criteria for an autoimmune etiology—such as symmetric morning stiffness lasting > 1 hour and specific PIP/MCP joint involvement —blindly hunting for an unlikely malignancy with expensive, high-radiation imaging violates the principle of "do no harm" (both physically and financially). Rheumatoid arthritis is diagnosed based on clinical presentation and targeted laboratory studies (RF, anti-CCP, ESR, CRP) alongside localized radiography , not whole-body pan-scanning.

**Next:** [9. Terminal Outcome: The Financial Toxicity](#termination-node-11)

---

<a id="termination-node-11"></a>
### 9. Ending: Terminal Outcome: The Financial Toxicity

> **Result:** fail · **Concept:** `Diagnostic Parsimony & Financial Toxicity`

Final Outcome: Failure / Iatrogenic Financial Harm & Delayed Treatment

The Flaw: Refusing to pivot a differential diagnosis based on a classic clinical presentation and forcing unnecessary, expensive testing.

Actionable Improvement: Recognize the classic RA presentation. Start with targeted, high-yield tests (RF, anti-CCP, CRP, ESR, hand/wrist XR) before jumping to "zebra" diagnoses like occult malignancy.

_End of this path._

---

<a id="decision-node-36"></a>
### 10. Decision: The Pharmacological Bridge (Time: 1 Week Later)

Sarah's labs return. Her ESR and CRP are markedly elevated . Her Rheumatoid Factor (an IgM antibody targeting the Fc portion of IgG) is positive, and her anti-CCP is highly positive . Her baseline hand X-rays show diffuse osteopenia but no erosions yet.You diagnose her with Rheumatoid Arthritis. She is currently in tears due to the severe pain in her hands.

![The Pharmacological Bridge (Time: 1 Week Later)](images/45b6596e-72c4-4547-863c-bff5ca95206e.jpeg)

**What do you do?**

- **A. The Monotherapy Trap** _(wrong)_ — Since her disease is early, you prescribe daily NSAIDs (Ibuprofen) for pain control and tell her to follow up in six months. → [11. The Monotherapy Trap](#information-node-18)
- **B. The Unprotected DMARD** _(misstep)_ — You correctly recognize the need to stop disease progression. You prescribe Methotrexate immediately. You tell her to take it and send her home without any other medications. → [14. The DMARD Remedy](#decision-node-38)
- **C. The Standard of Care** _(correct)_ — You prescribe Methotrexate, explaining it is the initial Disease-Modifying Antirheumatic Drug (DMARD) used to retard disease-associated damage . You simultaneously prescribe a short course of oral glucocorticoids and NSAIDs, explaining these will provide immediate symptomatic control while you wait weeks for the Methotrexate to take effect . → [23. The Standard of Care](#information-node-21)

---

<a id="information-node-18"></a>
### 11. The Monotherapy Trap

Sarah feels great on the high-dose NSAIDs. Her pain is masked. However, beneath the surface, Th1 cells are releasing interferon-$\gamma$ to activate macrophages, and her synovial plasma cells continue to produce antibodies against her joints . Six months later, she returns. Despite her pain being "controlled," her repeat X-rays show severe joint space narrowing and permanent periarticular bony erosions .

![The Monotherapy Trap](images/c7e14e20-7286-4fca-a541-2dc6d4df2394.jpeg)

**Next:** [12. The Lesson:](#information-node-19)

---

<a id="information-node-19"></a>
### 12. The Lesson:

NSAIDs and glucocorticoids provide excellent symptomatic control, but they do absolutely nothing to stop the underlying autoimmune destruction of the joint. In Rheumatoid Arthritis, Disease-Modifying Antirheumatic Drugs (DMARDs) like Methotrexate must be initiated to prevent, stop, or retard disease-associated damage .

**Next:** [13. Terminal Outcome: The Silent Erosion](#termination-node-20)

---

<a id="termination-node-20"></a>
### 13. Ending: Terminal Outcome: The Silent Erosion

> **Result:** fail · **Concept:** `Disease Modification vs. Symptom Control`

Final Outcome: Failure / Progression of Autoimmune Disease

The Flaw: Failing to initiate a DMARD (Methotrexate) upon confirming an RA diagnosis.

Actionable Improvement: Never treat RA with NSAIDs or steroids as monotherapy for long-term management. DMARDs are mandatory to save the joints.

_End of this path._

---

<a id="decision-node-38"></a>
### 14. Decision: The DMARD Remedy

Sarah calls the clinic three days later, sobbing. "I've been taking the Methotrexate, but my hands still hurt so badly I can't hold my coffee mug. The medicine isn't working!"

![The DMARD Remedy](images/fb7c736c-5e58-440b-8cdb-dc8221fab177.jpeg)

**What do you do?**

- **A. The Toxic Escalation** _(wrong)_ — You tell her that her disease must be incredibly aggressive. You drastically increase her Methotrexate dose to force an acute analgesic effect. → [15. The Toxic Escalation](#information-node-26)
- **B. Remedy Choice** _(correct)_ — You realize Methotrexate takes several weeks to reach therapeutic efficacy. You apologize for not providing bridge therapy and immediately call in a prescription for NSAIDs/glucocorticoids for symptomatic control while waiting for the DMARD response . → [18. The Pre-Operative Clearance (Time: 5 Years Later)](#decision-node-41)

---

<a id="information-node-26"></a>
### 15. The Toxic Escalation

Methotrexate is an immunosuppressant and disease-modifier, not an acute analgesic. Increasing the dose to toxic levels provides zero immediate pain relief for Sarah. Instead, she presents to the ER a week later with severe oral ulcers, macrocytic anemia, and fulminant hepatotoxicity (classic side-effects of high-dose Methotrexate) . You have poisoned your patient due to a fundamental misunderstanding of pharmacological kinetics.

![The Toxic Escalation](images/59eb29da-752e-4df6-b0e8-0097e10251b5.jpeg)

**Next:** [16. The Lesson:](#information-node-28)

---

<a id="information-node-28"></a>
### 16. The Lesson:

Disease-Modifying Antirheumatic Drugs (DMARDs) like Methotrexate alter the underlying disease process by retarding associated damage, but they take weeks to months to achieve clinical efficacy. They are not acute analgesics. Escalating an immunosuppressant to toxic doses in an attempt to force immediate pain relief displays a fundamental misunderstanding of pharmacokinetics. Acute RA flares must be bridged with fast-acting anti-inflammatories (NSAIDs or glucocorticoids) for symptomatic control while waiting for the DMARD response .

**Next:** [17. Terminal Outcome: The Hepatic Hit](#termination-node-32)

---

<a id="termination-node-32"></a>
### 17. Ending: Terminal Outcome: The Hepatic Hit

> **Result:** fail · **Concept:** `Pharmacokinetics & Bridge Therapy`

Final Outcome: Fatal Deficit / Drug Toxicity

The Flaw: Using a long-acting DMARD as an acute analgesic and overdosing the patient into hepatotoxicity.

Actionable Improvement: Memorize the bridge protocol. Always initiate NSAIDs or short-course steroids for immediate symptom control while waiting for DMARDs (Methotrexate) to take effect .

_End of this path._

---

<a id="decision-node-41"></a>
### 18. Decision: The Pre-Operative Clearance (Time: 5 Years Later)

Sarah is now 40 years old. Her RA has been well-controlled on Methotrexate and a TNF-inhibitor (Adalimumab) . She comes to your clinic because she is scheduled for an elective laparoscopic cholecystectomy (gallbladder removal) next week requiring general anesthesia and intubation. She needs you to sign off on her pre-operative clearance.

![The Pre-Operative Clearance (Time: 5 Years Later)](images/548da91c-ee23-4f48-93c6-bdd23de28510.jpeg)

**What do you do?**

- **A. The Routine Clearance** _(wrong)_ — You listen to her heart and lungs, note her stable vitals, and sign the clearance paperwork. She is young and her cardiovascular risk is low. → [19. The Routine Clearance](#information-node-29)
- **B. The Cervical Precaution** _(correct)_ — You recognized a silent, deadly complication of chronic RA. The neck X-ray is required to rule out atlantoaxial ligament laxity before any procedure requiring intubation. The X-ray shows stability, and you safely clear her for surgery. → [22. The Cervical Precaution](#information-node-45)

---

<a id="information-node-29"></a>
### 19. The Routine Clearance

You clear Sarah for surgery. In the OR, the anesthesiologist pushes paralytics and hyperextends her neck to visualize her vocal cords. Because you did not screen for atlantoaxial subluxation, the manipulation of her neck causes a catastrophic spinal cord compression . Sarah wakes up from her successful gallbladder surgery with hyporeflexia and irreversible quadriplegia .

![The Routine Clearance](images/17f8c75e-084d-493c-8465-23a52ac9c9f0.jpeg)

**Next:** [20. The Lesson:](#information-node-34)

---

<a id="information-node-34"></a>
### 20. The Lesson:

Rheumatoid Arthritis frequently causes inflammation and destruction of the transverse ligament of the atlas in the cervical spine, leading to atlantoaxial subluxation. This is often asymptomatic. During general anesthesia, the anesthesiologist must manipulate and hyperextend the neck to insert the endotracheal tube. If the atlantoaxial joint is unstable, this manipulation can drive the dens of the axis directly into the spinal cord.

**Next:** [21. Terminal Outcome: The Intubation Injury](#termination-node-33)

---

<a id="termination-node-33"></a>
### 21. Ending: Terminal Outcome: The Intubation Injury

> **Result:** fail · **Concept:** `Surgical Clearance & Silent Subluxation`

Final Outcome: Fatal Deficit / Iatrogenic Paralysis

The Flaw: Failing to screen a chronic RA patient for cervical spine instability prior to general anesthesia/intubation.


Actionable Improvement: Any patient with long-standing Rheumatoid Arthritis must have a cervical spine X-ray to rule out atlantoaxial subluxation before undergoing procedures that require manipulation of the neck .

_End of this path._

---

<a id="information-node-45"></a>
### 22. The Cervical Precaution

You recognized a silent, deadly complication of chronic RA. The neck X-ray is required to rule out atlantoaxial ligament laxity before any procedure requiring intubation. The X-ray shows stability, and you safely clear her for surgery.

![The Cervical Precaution](images/e53535e4-ab53-4cd7-ab8e-94108a4e7970.jpeg)

---

<a id="information-node-21"></a>
### 23. The Standard of Care

You successfully treated both the underlying pathophysiology (preventing cartilage destruction) and the patient's acute suffering.

![The Standard of Care](images/5510b215-a6a0-4055-9e64-ff6140bf3369.jpeg)

**Next:** [18. The Pre-Operative Clearance (Time: 5 Years Later)](#decision-node-41)

---

<a id="information-node-14"></a>
### 24. The Objective Empathy

You successfully de-escalated her anxiety with objective clinical reasoning. Anti-CCP is highly specific for rheumatoid arthritis, and baseline X-rays are crucial for tracking disease progression.

![The Objective Empathy](images/38965f7d-83c7-44fb-9acb-3bacc5057e4e.jpeg)

**Next:** [10. The Pharmacological Bridge (Time: 1 Week Later)](#decision-node-36)

---
