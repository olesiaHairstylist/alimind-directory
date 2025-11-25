# GOVERNMENT.md  
Government section specification (GOV)

---

# Purpose
Contains all official government institutions of Alanya.

---

# Included organizations

- Municipality (Belediye)
- Police (Emniyet)
- Jandarma
- Migration Office (Göç)
- Tax Office (Vergi Dairesi)
- Land Registry (Tapu)
- PTT (Post)
- SGK Social Insurance
- ASAT Water
- Akdeniz Elektrik
- Hotlines (155, 112, 156, 153)

---

# File
```
data/gov.json
```

---

# Rules

- All organizations sorted by importance
- Neutral language
- 2–3 sentence description
- No duplication
- ID format: `GOV_01`, `GOV_02`, ...

---

# Example

```json
[
  {
    "id": "GOV_01",
    "category": "gov",
    "name": "Alanya Belediyesi",
    "type": "Municipality",
    "status": "standard",
    "address": "Güllerpınarı Mah., Şevket Tokuş Cd. 45, Alanya",
    "google_maps": "https://maps.google.com/?q=Alanya+Belediyesi",
    "phone": "+90 242 444 82 07",
    "whatsapp": "+90 552 444 82 07",
    "languages": ["TR", "EN"],
    "description": "Main municipal office providing public services, documents, applications and local administration support."
  }
]
```

