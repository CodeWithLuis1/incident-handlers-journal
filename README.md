# 📓 Incident Handler's Journal

> A log of cybersecurity incident analysis. This project documents the study of a security incident using a structured template (date, description, tools, the 5 W's of the incident, and additional notes).

**Author:** _[Luis González C., Eng., M.Sc.]_
**Context:** Hands-on cybersecurity project — incident response analysis.

---

## 🗂️ Entry #1 — Ransomware attack on a healthcare clinic

| Field | Detail |
|---|---|
| **Date** | _[9/19/2026]_ |
| **Entry #** | 1 |

### 📝 Description

A small U.S. healthcare clinic specializing in primary care services experienced a **ransomware attack**. On a Tuesday morning, around 9:00 a.m., several employees were unable to access their computers or critical files such as patient medical records. A **ransom note** appeared on their screens stating that the files had been encrypted and demanding a large sum of money in exchange for the decryption key. The incident brought the organization's operations to a complete halt and forced a shutdown of its computer systems.

### 🛠️ Tools used

No specific investigation tools were documented for this incident, as it corresponds to an initial analysis exercise of the event.

Tools that would be **relevant** in a real investigation of this type:

- **SIEM** (Security Information and Event Management) — to correlate logs and detect anomalous activity.
- **EDR / antivirus** — to identify and contain the malware on endpoints.
- **Email security / anti-phishing tools** — to trace the entry vector.
- **Network analysis tools** (e.g., packet capture) — to review suspicious communications.

### 🔎 The 5 W's of the incident

| | Question | Answer |
|---|---|---|
| **Who** | Who caused the incident? | An organized group of unethical hackers, known for targeting organizations in the **healthcare and transportation** sectors. |
| **What** | What happened? | The attackers sent **targeted phishing emails** with a malicious attachment. Once downloaded, it installed malware that gave them access to the network. They then deployed **ransomware**, which encrypted critical files. A ransom note demanded money in exchange for the decryption key. |
| **When** | When did it occur? | On a **Tuesday morning, at approximately 9:00 a.m.** |
| **Where** | Where did it happen? | On the healthcare clinic's **network and computers**: employee workstations and the systems storing patient medical records. |
| **Why** | Why did it happen? | **Financial** motivation: to extort the company for a ransom. The attackers exploited the **human factor** through phishing to gain initial access. |

### 🗒️ Additional notes

- **Entry vector:** targeted phishing email with a malicious attachment → highlights the need for **security awareness training** for employees.
- **Impact:** complete disruption of operations and loss of access to sensitive patient data (possible regulatory implications, e.g., **HIPAA** in the U.S.).
- **Initial response:** the company shut down its systems and contacted external organizations to report the incident and receive technical assistance.
- **Open question:** were there isolated (offline) backups that would allow data restoration without paying the ransom?
- **Takeaway:** this case shows how a single phishing email can escalate to a full organizational shutdown, and the importance of layered defenses (backups, network segmentation, EDR, training).

