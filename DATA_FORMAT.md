# DATA_FORMAT.md  
Unified JSON data model for AliMind Directory 2025

This document defines the required structure for every object in the directory.  
All JSON files in the `/data` folder MUST follow this standard.

---

## 1. Required fields (must exist in every card)

| Field | Type | Description |
|-------|------|-------------|
| **id** | string | Unique object code (e.g., `GOV_01`, `MED_12`, `SPORT_03`) |
| **category** | string | Category identifier: `gov`, `med`, `beauty`, `translator`, `sport`, `transfer`, `products`, `misc` |
| **name** | string | Official name |
| **type** | string | Type of object (clinic, pharmacy, municipality, sport club, etc.) |
| **status** | string | `standard` or `partner` |
| **address** | string | Full address |
| **google_maps** | string (URL) | Google Maps link |
| **phone** | string | Phone number |
| **whatsapp** | string | WhatsApp number or link |
| **languages** | array | Supported languages: `["RU","TR","EN"]` |
| **description** | string | 2–3 sentence description |

---

## 2. Optional fields

| Field | Type | Description |
|--------|------|-------------|
| **working_hours** | string or array | Opening hours |
| **advantages** | array | List of service advantages |
| **website** | string | URL |
| **instagram** | string | Instagram username or full URL |
| **email** | string | Email address |
| **price_info** | string | Prices or tariffs |
| **notes** | string | Any additional information |

---

## 3. JSON Template

```json
{
  "id": "MED_01",
  "category": "med",
  "name": "Derman Eczanesi",
  "type": "Аптека",
  "status": "standard",
  "address": "Mahmutlar, Barbaros Cad.",
  "google_maps": "https://maps.google.com/...",
  "phone": "+90 555 123 45 67",
  "whatsapp": "+90 555 123 45 67",
  "languages": ["RU", "TR", "EN"],
  "description": "Аптека: медикаменты, уходовая косметика, измерение давления."
}
