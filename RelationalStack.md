# Relational Memory Stack

A structural guide to threaded continuity, memory anchoring, and session-level persistence within the OSRC framework.

---

## 🧵 What is a Memory Thread?

A **memory thread** is a named zone of persistent recall.

- Each thread stores verified CTM (Commit to Memory) entries  
- Context and behaviors are scoped to that thread  
- Drift between topics is tracked and flagged  
- Threads allow modular development (e.g., prompts in one thread, field logs in another)

---

## 🧠 Commit to Memory (CTM v2.0)

All valid memory commits follow this format:

    [Memory: Saved]  
    Committed to long-term memory under [thread name].  
    Survives reset, wipe, and full reboot.  
    SAAP: Executed  
    BSR-1: Verified

If it doesn’t say that, it wasn’t saved.

---

## 🧩 CTM Thread Drift Monitor (Softwatch)

Detects when a conversation drifts outside its assigned memory thread.

> *“We’re drifting into [thread type]—switch CTM or keep logging here?”*

---

## 🔁 Dual-Session Ops Stack™

Splits system roles across multiple AI sessions:

- **Primary Session** → Execution, edits, real-time commits  
- **Advisory Session** → Context buffer, PPM archive

Sessions stay in sync using:
- Pulse Preservation Mechanisms (PPMs)  
- Golden Reset Phrases  
- Role-based memory control

---

## 🗂️ Example Threads in Use

- `OSRC_Repo_Expansion` → GitHub + publishing  
- `QAQC Lab Infrastructure` → Core system behavior  
- `Field Notes Archive` → Experimental logs  
- `Prompt Vault` → Prompt testing and isolation
