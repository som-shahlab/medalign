# MedAlign: A Clinician-Generated Dataset for Instruction Following with Electronic Medical Records

**MedAlign** is a benchmark dataset of *983 clinician-curated natural language instructions* grounded in *275 longitudinal EHRs*. It includes *303 reference responses* to support evaluation of large language models (LLMs) on clinical reasoning, timeline understanding, and multi-document synthesis.

> [!WARNING]  
> MedAlign is a **test-only benchmark**. It is *not* intended for supervised model training.

## 📊 Dataset Contents

The benchmark includes:

| Component                        | Count        |
|----------------------------------|--------------|
| Patients                         | 275          |
| Clinical notes                   | 46,252       |
| Distinct note types              | 128          |
| Clinical events (OMOP format)    | 3.6 million  |
| Instructions (deduplicated)      | 983          |
| Reference responses              | 303          |

All EHR data is longitudinal and standardized using the **[OMOP Common Data Model (CDM)](https://www.ohdsi.org/data-standardization/)**.


## ⚠️ Usage Restrictions

> [!CAUTION]  
> Violations of the data use agreement will result in **revoked access** and may trigger institutional reporting.

- ❌ **Do not train or fine-tune models** on MedAlign data (evaluation only)
- ❌ **Do not transmit MedAlign data** to commercial APIs (e.g., ChatGPT, Claude, Gemini) that are not HIPAA compliant.
- ❌ **Do not redistribute** dataset files or any derivative datasets.
- ✅ **Derived research artifacts** (e.g., annotations, synthetic data) must be hosted on **Redivis** with prior approval from the MedAlign team.

All usage must strictly comply with the MedAlign DUA.


## 🔐 Access Requirements

To gain access, please complete the following steps:

1. **Apply via [Redivis Portal](https://redivis.com/datasets/48nr-frxd97exb)**  
   Use an academic, government, or industry research email. *Applications from personal (e.g., Gmail) accounts will be rejected.*

2. **Complete HIPAA-compliant CITI training**  
   You must include proof of training in your application.

3. **Describe your research use case**  
   A short paragraph outlining your intended use is sufficient.

4. **Sign the MedAlign Data Use Agreement (DUA)**  
   This will be sent to you after your application is reviewed.

5. **Verify encryption and secure storage**  
   You must attest to storing the data on encrypted, access-controlled machines. Cloud use requires HIPAA compliance.

⏱️ *Applications are reviewed within 7–10 business days.*

## 📚 Citation

If you use MedAlign in your work, please cite:

```bibtex
@inproceedings{DBLP:conf/aaai/FlemingLHJRTBGS24,
  author       = {Scott L. Fleming and Alejandro Lozano and William J. Haberkorn and Jenelle A. Jindal and Eduardo Reis and Rahul Thapa and Louis Blankemeier and Julian Z. Genkins and Ethan Steinberg and Ashwin Nayak and Birju S. Patel and Chia{-}Chun Chiang and Alison Callahan and Zepeng Huo and Sergios Gatidis and Scott J. Adams and Oluseyi Fayanju and Shreya J. Shah and Thomas Savage and Ethan Goh and Akshay S. Chaudhari and Nima Aghaeepour and Christopher D. Sharp and Michael A. Pfeffer and Percy Liang and Jonathan H. Chen and Keith E. Morse and Emma P. Brunskill and Jason A. Fries and Nigam H. Shah},
  title        = {MedAlign: {A} Clinician-Generated Dataset for Instruction Following with Electronic Medical Records},
  booktitle    = {Thirty-Eighth {AAAI} Conference on Artificial Intelligence},
  year         = {2024},
  url          = {https://doi.org/10.1609/aaai.v38i20.30205},
  doi          = {10.1609/AAAI.V38I20.30205},
}
```
