================
Quickstart Guide
================

Follow these steps to evaluate your model’s openness using the Model Openness Tool (MOT).

Step 1: Gather Your Components
-----------------------------
Prepare your model release package with relevant artifacts, such as:

- Model card & data card
- Training and test datasets (or links to them)
- Code: preprocessing, training, evaluation, inference
- Model checkpoints & hyperparameters
- Documentation (README, research paper, diagrams)
- License files for each component

Refer to the :doc:`intro/mof` page for the definitive list of 16 MOF components.

Step 2: Open the Evaluation Form
--------------------------------
Visit:

https://mot.isitopen.ai/model/evaluate

Here’s what you’ll encounter:

1. **Model Details** – name, version, producer, contact, type  
2. **Global Licenses** – apply default licenses to code, data, and documentation across components  
3. **Component Overrides** – override any global license per component (e.g., a dataset with a different license)

Step 3: Submit & Analyze
------------------------
After form submission, MOT:

- Checks which of the 16 MOF components are included  
- Validates if each uses an appropriate open license (based on MOF’s license rules)  
- Assigns openness class (I–III) combining completeness and license compliance :contentReference[oaicite:1]{index=1}

You’ll receive:

- A component-by-component breakdown (✅ open / ⚠️ restrictive / ❌ unreleased)  
- Your MOF class score (1, 2, or 3)  
- Downloadable files:
  - `MOF.json` manifest
  - Embed-ready openness badge

Step 4: Publish Your Model
--------------------------------------
To add your model to MOT’s public catalog:

1. Fork the GitHub repo `lfai/model_openness_tool`  
2. Add your model’s metadata and `MOF.json` under `models/`  
3. Create a Pull Request for community review

Once merged, your model appears on the live catalog.

Step 5: Promote Your Openness
-----------------------------
Embed the badge and link back to your public MOT page:

- In your documentation (README, website, Hugging Face card)  
- It signals transparency and licensure clarity to users and collaborators

For a detailed walkthrough including screenshots, see :doc:`../evaluate/case_walkthrough`.
