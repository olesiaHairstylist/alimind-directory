# DATA_STRUCTURE.md  
Directory and file structure for AliMind Directory 2025

This document defines the correct layout of all JSON files, folders, and data modules.

---

# 1. Root project structure


---

# 3. Description of each file

### **districts.json**
List of main districts of Alanya + sub-areas.  
Used for filtering all other categories.

### **gov.json**
Government institutions: municipality, police, migration, SGK, tax, registry, PTT, utilities (ASAT/Akdeniz Elektrik), hotlines.

### **med.json**
Clinics, pharmacies, dental services, medical centers, duty pharmacies.

### **beauty.json**
Beauty salons, hair stylists, cosmetology, nail services.

### **translator.json**
Translators, sworn interpreters, notarial assistance.

### **sport.json**
Sports clubs, boxing, personal trainers, gyms.

### **transfer.json**
Airport transfers, taxi, drivers, transport services.

### **products.json**
AliMind ecosystem services, internal products, subscriptions.

### **misc.json**
Banks, currency exchange, entertainment, shops, other useful services.

---

# 4. JSON rules for all files

- All files MUST contain an **array** of objects  
- Each object MUST follow `DATA_FORMAT.md`  
- IDs MUST be unique across the whole project  
- Categories MUST match the filename  
- No extra keys allowed  
- All data MUST be neutral and factual  

Example:

```json
[
  {
    "id": "MED_01",
    "category": "med",
    "name": "Example Clinic",
    "type": "Clinic",
    "status": "standard",
    "address": "Mahmutlar, Barbaros Cd.",
    "google_maps": "https://maps.google.com/...",
    "phone": "+90 555 123 45 67",
    "whatsapp": "",
    "languages": ["TR", "RU", "EN"],
    "description": "Example medical center."
  }
]
