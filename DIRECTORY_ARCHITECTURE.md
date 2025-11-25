# DIRECTORY_ARCHITECTURE.md  
Architecture of AliMind Directory 2025

This document describes the full architecture of the data system, integration points and update flow.

---

# 1. Project layers

```
Root Repository
│
├── Documentation (MD files)
├── Data Layer (JSON)
└── Integration Layer (Bots, API, Website)
```

---

# 2. Data Layer

Main folder:

```
/data
```

Contains:

```
districts.json
gov.json
med.json
beauty.json
translator.json
sport.json
transfer.json
products.json
misc.json
```

All files:

- follow the same JSON model  
- contain arrays  
- strictly validated  
- have unique IDs  

---

# 3. Integration Layer

Directory is used by:

### 1) AliMind Telegram Bot  
- buttons  
- inline search  
- categories  
- district filters  
- partner cards  

### 2) AliMind Website  
- REST-like static data loading  
- categories pages  
- district pages  
- JSON → HTML rendering  

### 3) AliMind API (future)  
API v1.0 (static)   
API v2.0 (partners + dynamic updates)

---

# 4. Update Process

```
Step 1: Edit /data/*.json
Step 2: Commit changes
Step 3: Bot + Website auto-update from GitHub source
```

---

# 5. Versioning

```
v1.0 — Core data
v1.1 — District mapping
v1.2 — Partner module
v2.0 — API integration
v3.0 — Dynamic updates + admin panel
```

