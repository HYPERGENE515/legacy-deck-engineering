# 🧠 Legacy Deck Engineering Framework

A structured system for analyzing, modeling, and optimizing Legacy decks using an **engine-based framework**.

---

## 🎯 Purpose

This project aims to:

- Formalize deck construction as **interacting engines**
- Standardize matchup analysis
- Enable scalable comparison across multiple decks
- Serve as a foundation for **AI-assisted decision making**

---

## 🧱 Project Structure


legacy-deck-engineering/

│

├── framework/ # Core definitions & schemas

├── decks/ # Individual deck data

├── scripts/ # Automation tools

├── data/ # Cross-deck data (meta, matrix)

└── .github/ # CI / validation


---

## 🧩 Framework Concept

### 🔹 Engine-Based Design

Each deck is modeled as a combination of:

- **Mana Engine** – resource acceleration
- **Card Engine** – card advantage / filtering
- **Lock Engine** – opponent restriction
- **Win Engine** – closing mechanism

---

### 🔹 DT / OT Model

- **DT (Deterministic Turn)**  
  → Stabilization phase

- **OT (Output Turn)**  
  → Winning phase

---

## 📦 Deck Structure

Each deck lives under:


decks/<deck-name>/


Example:


decks/blue-collar-workers/
├── engine_graph.json
├── source_data.json
├── matchup_profiles.json
└── versions/


---

## 🔵 Example: Blue Collar Workers

### Engine Composition

```json
{
  "core_engines": [
    "ManaEngine",
    "LockEngine",
    "CardEngine"
  ]
}
Matchup Profile
{
  "UR_Tempo": {
    "role": "Control",
    "DT_priority": "High",
    "OT_plan": "Kappa finish"
  }
}
⚙️ Automation

Scripts are located in:

scripts/

Main features:

Update JSON via GitHub API
Validate data structure
Manage versioning
🔐 Security

Sensitive data (tokens, secrets) must NOT be committed.

Use:

.env

And ensure .gitignore includes:

.env
🚀 Workflow
1. Generate JSON (ChatGPT)
2. Update via script
3. Push to GitHub
4. Analyze / iterate
📊 Future Extensions
Matchup Matrix (all decks vs all decks)
Meta analysis engine
AI decision support
Simulation environment
🧠 Philosophy

"Decks are not lists. They are systems."

This framework treats decks as dynamic systems of interacting components, enabling deeper understanding beyond traditional decklists.

📌 Status

🚧 Work in progress
Contributions and extensions welcome

👤 Author
HYPERGENE515
