
# 🧠 Analysing Palliative Care Concerns: Exploring Patient and Carer Narratives with GPT-3.5  
*A 4D Picture Project Tool*

This repository contains code and resources for extracting key concerns from palliative care narratives using **GPT-3.5**. It is part of the **4D Picture Project**, focused on understanding the needs, challenges, and emotional realities of patients and carers dealing with advanced illness and end-of-life care.

---

## 🎯 Objective

To automatically identify and categorize recurring concerns in patient and caregiver narratives, such as:

- Need for better support tools
- Access to care
- Educational resources for family carers
- Family support
- Emotional support

The goal is to support qualitative research, improve service design, and better inform person-centered care strategies.

---

## 📄 Sample Input Narrative

```text
When my father entered the final stage of his illness, I felt completely overwhelmed. The hospital staff were kind, but I often wished there were better tools or systems in place to guide families like ours through this process. We had so many questions, and it felt like we were constantly searching online for answers we should have received in person.

One of the biggest struggles was just getting access to consistent palliative care. Some services were only available during the week, and weekends were especially hard. There were days when I didn’t know who to call or whether anyone would come.

I also found myself unprepared for what caring for someone at the end of life truly meant. I wish there had been more educational resources designed specifically for family carers...

Emotionally, it was exhausting. I wish there had been more attention given to emotional support—not just for my dad, but for me and the rest of the family too.
````

---

## ✅ Example Output

The model extracts structured concern categories like:

```json
[
  {
    "label": "Need for better support tools",
    "evidence": [
      "I often wished there were better tools or systems in place to guide families like ours through this process."
    ]
  },
  {
    "label": "Access to care",
    "evidence": [
      "One of the biggest struggles was just getting access to consistent palliative care.",
      "Some services were only available during the week, and weekends were especially hard."
    ]
  },
  {
    "label": "Educational resources for family carers",
    "evidence": [
      "I wish there had been more educational resources designed specifically for family carers..."
    ]
  },
  {
    "label": "Emotional support",
    "evidence": [
      "Emotionally, it was exhausting.",
      "I wish there had been more attention given to emotional support..."
    ]
  }
]
```

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/palliative-care-concerns-gpt.git
cd palliative-care-concerns-gpt
```

### 2. Install dependencies

```bash
pip install openai
```

---

## 🧠 Concern Categories

| Label                                   | Description                                                             |
| --------------------------------------- | ----------------------------------------------------------------------- |
| Need for better support tools           | Calls for structured tools, guidance systems, digital or print aids     |
| Access to care                          | Issues around availability, responsiveness, and consistency of services |
| Educational resources for family carers | Requests for preparatory material and practical caregiving information  |
| Family support                          | Mentions of uneven burden or need for shared responsibilities           |
| Emotional support                       | Expressions of distress, burnout, or need for psychological support     |

---

## 🤝 Contributing

We welcome contributions in the form of:

* Improved prompting or fine-tuning
* New narrative datasets
* Integration into visualization tools

---

## 📬 Contact

For questions, collaboration, or feedback, contact \[Dr. Daisy Monika Lal] at \[[d.m.lal@lancaster.ac.uk](mailto:your.email@example.com)]

---

## 📚 Citation

```bibtex
@article{doi:10.1177/02692163251335482,

title ={The 19th World Congress of the European Association for Palliative Care 29 – 31 May 2025 Helsinki, Finland},

journal = {Palliative Medicine},
volume = {39},
number = {2\_suppl},
pages = {1-490},
year = {2025},
doi = {10.1177/02692163251335482},

URL = { 
    
        https://doi.org/10.1177/02692163251335482
    
},
eprint = { 
    
        https://doi.org/10.1177/02692163251335482

}

}  
