---
license: other
tags:
  - lora
  - age-progression
  - age-slider
  - face-editing
  - stylized
pipeline_tag: text-to-image
---

# 🔵 Simple_Age-S — Artistic Age Progression Slider LoRA
**ZIT compatible · Safe · Stylized age-morphing**

---

## ⚡ Quick Links

| Version | Weights | Preview |
|--------|---------|---------|
| **Soft** | [/ZiT/Soft/Age_S.safetensors](https://huggingface.co/dmsnoa/Age_S/resolve/main/ZiT/Soft/Age_S.safetensors) | <img src="https://huggingface.co/dmsnoa/Age_S/resolve/main/ZiT/Soft/026-02-09-10-28-10-g.png" width="120"> <img src="https://huggingface.co/dmsnoa/Age_S/resolve/main/ZiT/Soft/09-15-.png" width="120"> |
| **MiD** | [/ZiT/MiD/Age_S.safetensors](https://huggingface.co/dmsnoa/Age_S/resolve/main/ZiT/MiD/Age_S.safetensors) | <img src="https://huggingface.co/dmsnoa/Age_S/resolve/main/ZiT/MiD/2026-01-06-12.png" width="120"> <img src="https://huggingface.co/dmsnoa/Age_S/resolve/main/ZiT/MiD/2026-01-12-13.png" width="120"> |

---

## 🔍 Overview
**Simple_Age-S** is an artistic age-progression LoRA that adjusts the **stylized perceived age** of a face without altering:

- identity  
- ethnicity  
- personality  
- facial bone structure  

All transformations remain within **safe, non-realistic, stylized anatomy**.

---

## ⏳ How the Slider Works

Move `network_multiplier` into negative or positive ranges:

| Multiplier | Effect |
|-----------:|--------|
| `-2 → -0.7` | younger · softened features |
| `-0.6 → -0.2` | mild de-aging |
| `0` | neutral |
| `+0.2 → +0.7` | mature · light aging |
| `+0.8 → +2` | strong stylized elder look |

The LoRA modifies **only perceived age cues**, keeping identity intact.

---

## 🧩 Example Usage (ComfyUI / AITS Toolkit)

```yaml
lora:
  name: "dmsnoa/jix/Age_S"
  multiplier: 0.6   # subtle mature age
```

### Recommended Base Prompt
```
portrait, solo, looking at camera,
neutral expression, soft light,
realistic skin texture, photorealistic
```

💡 No need to mention age — the slider applies changes automatically.

---

## 🔐 Safety Notice
- Artistic age stylization only  
- Does NOT alter real identity  
- Not for biometric, forensic, or medical tasks  
- Produces stylized, non-identifiable results  
- Commercial + non-commercial usage allowed under license  

---


## 🧾 License
**CreativeML OpenRAIL-M**

---

## ✏️ Author  
Created by **dmsnoa / jix**

⭐ If this model helped you — consider starring the repository!
