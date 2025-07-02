# -LLM-schema-annotation-
Schema-driven annotation tool for medical text labeling using Pydantic and Panel
# LLM Schema Annotation

This project is a simple tool to help label medical reports like colonoscopy notes.  
It uses a **Pydantic schema** to build the form, and **Panel** to show the form in a web interface.

---

## What This Tool Can Do

- Builds the form automatically from a Python schema (no manual UI code)
- Lets the user enter:
  - Why the colonoscopy was done (indication)
  - How clean the bowel was (prep quality)
  - Number of polyps found
- Exports the form data to a `.json` file
- Adds `"schema_version"` to the output file
- Lets user name the output file (like `patient_003.json`)

---

## 📁 Files in This Project

| File Name | What It Is |
|-----------|------------|
| `annotationLLM.ipynb` | Main notebook that runs the form |
| `cancer 1 stage.json` | A sample JSON output created by filling the form |

---

##  What I Plan to Add Next

- Ability to load a saved `.json` file back into the form (edit mode)
- Compare two different label files (from two doctors)
- Connect this small tool to the full app (`app_v3.py`)
- Possibly use Docker or Label Studio later
