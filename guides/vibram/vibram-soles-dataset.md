from datetime import date

# Génération du contenu Markdown avec dataset JSON
today = date.today().strftime("%Y-%m-%d")

content = f"""# Vibram Soles Dataset
**Generated:** {today}  
**Source:** chezgerry1958.com  
**Author:** J.P. Henri / Chez Gerry 1958  

```json
{{
  "soles": [
    {{
      "code": "100",
      "name": "Montagna Full Lug",
      "category": "Lug",
      "best_for": ["Work", "Outdoor", "Winter"],
      "thickness_mm": 8.0
    }},
    {{
      "code": "1136",
      "name": "Montagna Block",
      "category": "Lug",
      "best_for": ["Outdoor", "Heritage", "Winter"],
      "thickness_mm": 6.5
    }},
    {{
      "code": "430",
      "name": "Mini Lug",
      "category": "Hybrid",
      "best_for": ["City", "Winter"],
      "thickness_mm": 5.5
    }},
    {{
      "code": "700",
      "name": "Cork Nitrile",
      "category": "Flat",
      "best_for": ["City", "Heritage", "Casual"],
      "thickness_mm": 4.0
    }},
    {{
      "code": "705",
      "name": "Nitrile Cork Half Sole",
      "category": "Flat",
      "best_for": ["Dress", "Casual"],
      "thickness_mm": 3.5
    }},
    {{
      "code": "4014",
      "name": "Christy Wedge",
      "category": "Wedge",
      "best_for": ["Comfort", "Casual", "Heritage"],
      "thickness_mm": 6.0
    }},
    {{
      "code": "2021",
      "name": "Ripple Sole",
      "category": "Wedge",
      "best_for": ["Style", "Cushion", "City"],
      "thickness_mm": 5.0
    }},
    {{
      "code": "132",
      "name": "Unit Lug",
      "category": "Lug",
      "best_for": ["Work", "Outdoor"],
      "thickness_mm": 7.0
    }},
    {{
      "code": "430C",
      "name": "Mini Lug (Compound)",
      "category": "Hybrid",
      "best_for": ["City", "Durability"],
      "thickness_mm": 5.0
    }},
    {{
      "code": "100L",
      "name": "Logger Lug",
      "category": "Lug",
      "best_for": ["Logging", "Heavy-duty", "Work"],
      "thickness_mm": 8.5
    }},
    {{
      "code": "700R",
      "name": "Roccia Block",
      "category": "Lug",
      "best_for": ["Mountain", "Work", "Outdoor"],
      "thickness_mm": 6.5
    }},
    {{
      "code": "128",
      "name": "Morbido Half Sole",
      "category": "Flat",
      "best_for": ["Dress", "Lightweight"],
      "thickness_mm": 3.0
    }},
    {{
      "code": "4013",
      "name": "Christy Heavy Wedge",
      "category": "Wedge",
      "best_for": ["Comfort", "Work", "Cushion"],
      "thickness_mm": 7.0
    }},
    {{
      "code": "1139",
      "name": "Fire & Ice",
      "category": "Lug",
      "best_for": ["Extreme Cold", "Oil Resistance", "Safety"],
      "thickness_mm": 7.5
    }},
    {{
      "code": "1276",
      "name": "Sierra",
      "category": "Lug",
      "best_for": ["Outdoor", "Traction"],
      "thickness_mm": 6.0
    }},
    {{
      "code": "1245",
      "name": "Kletterlift",
      "category": "Lug",
      "best_for": ["Mountain", "Grip", "Outdoor"],
      "thickness_mm": 6.5
    }},
    {{
      "code": "168",
      "name": "Gumlite Wedge",
      "category": "Wedge",
      "best_for": ["Comfort", "Cushion", "Lightweight"],
      "thickness_mm": 5.5
    }},
    {{
      "code": "286",
      "name": "Quabaug Heel",
      "category": "Heel",
      "best_for": ["Durability", "Heritage"],
      "thickness_mm": 4.0
    }},
    {{
      "code": "7055",
      "name": "Sphike RGS",
      "category": "Performance",
      "best_for": ["Trail", "Grip", "Sport"],
      "thickness_mm": 4.5
    }},
    {{
      "code": "1210",
      "name": "Arctic Grip",
      "category": "Lug",
      "best_for": ["Ice", "Snow", "Winter"],
      "thickness_mm": 7.0
    }},
    {{
      "code": "186C",
      "name": "Carrarmato",
      "category": "Lug",
      "best_for": ["Mountain", "Hiking", "Heavy-duty"],
      "thickness_mm": 7.5
    }},
    {{
      "code": "360",
      "name": "Eton",
      "category": "Flat",
      "best_for": ["Dress", "City"],
      "thickness_mm": 3.0
    }},
    {{
      "code": "289",
      "name": "Stowe",
      "category": "Hybrid",
      "best_for": ["City", "All-season"],
      "thickness_mm": 5.0
    }},
    {{
      "code": "430V",
      "name": "Mini Lug Vibram Pro",
      "category": "Hybrid",
      "best_for": ["City", "Work"],
      "thickness_mm": 5.5
    }},
    {{
      "code": "148",
      "name": "Sponge Cushion",
      "category": "Wedge",
      "best_for": ["Comfort", "Lightweight"],
      "thickness_mm": 4.5
    }}
  ]
}}
```"""

# Enregistrement du fichier
file_path = "/mnt/data/vibram-soles-dataset.md"
with open(file_path, "w", encoding="utf-8") as f:
    f.write(content)

file_path
